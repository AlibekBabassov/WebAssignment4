Babassov Alibek, IT-2503

Task0:
<img width="1512" height="982" alt="Снимок экрана 2026-10-08 в 15 27 28" src="https://github.com/user-attachments/assets/83843514-1726-4e4a-afa4-3ef462eb1194" />
Summary: I created a simple contact form using only plain HTML, with no Bootstrap classes. It has a text input for the name, an email input, a textarea for the message and a submit button. Each field has a `<label>` connected to its input with the `for` and `id` attributes, so clicking a label focuses the matching field.

Task1:
<img width="1512" height="982" alt="Снимок экрана 2026-10-08 в 15 32 22" src="https://github.com/user-attachments/assets/831c8172-191d-4e9e-b1e6-5ac0ffb5df93" />
Summary:I copied the contact form from Task 0 and added HTML5 validation attributes. All fields use `required`, so they can't be empty. The name and message have `minlength` and `maxlength` to limit the number of characters, and the email field uses `type="email"` so the browser checks the email format. I tested it by submitting an empty form and by entering an email without `@`. In both cases the browser blocked the submission and showed its own error message.

Task2:
<img width="1512" height="982" alt="Снимок экрана 2026-10-08 в 15 34 53" src="https://github.com/user-attachments/assets/3f12d9cf-03c2-4047-9d77-5d37ee515651" />
Summary: I recreated the contact form with Bootstrap. The inputs use `form-control`, the labels use `form-label`, and the button uses `btn btn-primary`. Name and Email are placed side by side with `row` and `col-md-6`, and on small screens they stack. I added placeholders to the fields and helper text with the `form-text` class under the name and email.


task3:
<img width="1512" height="982" alt="Снимок экрана 2026-10-08 в 15 40 23" src="https://github.com/user-attachments/assets/f1463750-cdcc-4955-bf15-036af33bffb5" />
Summary: I added Bootstrap validation to the form. I used the `novalidate` attribute to turn off the browser's own messages, and wrote a short JavaScript that runs when the form is submitted. For each field it calls `checkValidity()` and adds `is-valid` (green) or `is-invalid` (red). Under every input there are `valid-feedback` ("Looks good!") and `invalid-feedback` messages (for example, "Email is required"). I tested it with an empty form, a partly filled form and a fully correct form.

Task4:
<img width="1512" height="982" alt="Снимок экрана 2026-10-08 в 15 45 08" src="https://github.com/user-attachments/assets/396fc7fa-f493-4885-a145-acf4bdba542d" />
<img width="1512" height="982" alt="Снимок экрана 2026-10-08 в 15 45 58" src="https://github.com/user-attachments/assets/4d41590f-a362-4126-90b0-89ae907bbfa3" />
<img width="1512" height="982" alt="Снимок экрана 2026-10-08 в 15 47 26" src="https://github.com/user-attachments/assets/59cb8f32-687a-445f-967f-df74f6c134b1" />
<img width="1512" height="982" alt="Снимок экрана 2026-10-08 в 15 45 45" src="https://github.com/user-attachments/assets/ac72b6ff-a00e-475e-a453-163aeac7e45b" />

Summary: I built a full registration form. Bootstrap `row` and `col-md-6` classes make it responsive, so the fields sit side by side on wide screens and stack on phones. The form uses HTML5 validation: all main fields are `required`, the password has `minlength="8"`, and the email uses `type="email"`. Gender is a group of radio buttons with the same `name`, so only one can be selected, and hobbies are optional checkboxes. The country is a `select` dropdown with an empty first option, so the user has to choose one. For the confirm-password field I used `setCustomValidity()` in JavaScript to mark it invalid when the two passwords are different. Bootstrap feedback messages show errors in red and success in green. The Reset button clears the form and removes the validation colors.
