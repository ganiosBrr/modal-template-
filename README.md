# modal-template-
Template of modal window with content.

Functions openModal() and closeModal() are responsible for to show and hide modal window content.
Function modal() is responsible for handle on which trigger we should call open and close modal functions.
This functions handles clicking on buttons that has [data-modal] attribute, also it handles window scroll event, 
it means if we scroll our page in some point of screen we show our modal window.
Also it handles closing modal window by clicking at X button or every other point beside modal window or escape keydown.
For example we can call timer() function like this:

    `const modalTimerId = setTimeout(() => openModal('.modal', modalTimerId), 50000);`
    Calling openModal after 50 seconds after page loads.

    `modal('[data-modal]', '.modal', modalTimerId);`