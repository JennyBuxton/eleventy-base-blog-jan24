---
layout: layouts/base.njk
eleventyNavigation:
  key: Form
  order: 3
---
# Form

<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-T3c6CoIi6uLrA9TneNEoa7RxnatzjcDSCmG1MXxSR1GAsXEV/Dwwykc2MPK8M2HN" crossorigin="anonymous">
</head>

<body>
  <div class="card text-bg-primary mb-3" style="max-width: 50rem;">

    <div class="card-body">
      <h5 class="card-title  text-center">Complete the form below</h5>

      <form class="row g-3" action="#" id="task4">
        <div class="col-md-6">
          <label for="inputFname" class="form-label">First Name</label>
          <input type="text" class="form-control" id="inputFname" placeholder='Enter a firstname' required>
        </div>

        <div class="col-md-6">
          <label for="inputSname" class="form-label">Surname</label>
          <input type="text" class="form-control" id="inputSname" Placeholder="Enter your Surname" required>
        </div>

        <div class="col-12">
          <label for="inputEmail" class="form-label">Email</label>
          <input type="email" class="form-control" id="inputEmail" placeholder="a@a.com" required>
        </div>

        <div class="col-12">
          <label for="inputMessage" class="form-label">Message</label>
          <input type="text" class="form-control" id="inputPhone" placeholder="Write message here" required>
        </div>



        <div class="col-md-6">
          <fieldset id='mail'>
            <legend>Terms and Conditions</legend>
            <div class="form-check">
              <label class="form-check-label" for="yes">
                Yes
              </label>
              <input class="form-check-input" type="checkbox" name="yes" id="yes" value= "Yes">
            </div>

            <div class="form-check">

              <label class="form-check-label" for="no"> No
              </label>
              <input class="form-check-input" type="checkbox" name="np" id="fno" value = "No" checked>

            </div>
          </fieldset>
        </div>
    </div>

    <div class="col">
      <div class="d-grid gap-2 col-4 mx-auto">
        <input class="btn btn-outline-light" type="submit" value='submit'>
      </div>
    </div>

    </form>
  </div>
  </div>

  <script>
    const task4Form = document.getElementById('task4')
    task4Form.addEventListener('submit', (e) => {
      e.preventDefault();
      const formElements = task4Form.elements;
      const inputs = {};
      for (let i = 0; i < 9; i++) {
        if (formElements[i].type !== 'checkbox') {
          if (formElements[i].type === 'fieldset') {
            // Put the value of the checked radio button
            inputs.mail = formElements['mail'].value;
          } else {
            inputs[formElements[i].name] = formElements[i].value;
            // Resets the form inputs
          }
        } else {
          // Resets the check box
          formElements[i].checked = formElements[i].id === 'no' ? true : false;
        }
      }
      console.log(inputs);
    });
  </script>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-C6RzsynM9kWDrMNeT87bh95OGNyZPhcTNXj1NW7RuBCsyN/o0jlpcV8Qyq46cDfL" crossorigin="anonymous"></script>
</body>

</html>

