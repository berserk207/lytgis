Code review
===========

This guide tackles the things to consider before, during and after a code review, from documents to practices and approaches.

Guidelines
----------

Definition and Requirements
~~~~~~~~~~~~~~~~~~~~~~~~~~~

A code review is a part of the development process wherein the code developer and his/her co-workers sit down to examine codes line by line for possible improvements and/or cause of future defects.

In order to have a properly conducted code review, all the participants must
- have the proper understanding on how code reviews should be done,
- know what documents should be prepared / created and metrics to be tracked,
- have an established coding standard, and
- most importantly have the right attitude when conducting it.

Goals
~~~~~

Code reviews are primarily geared towards the identification of possible defects for them to be prevented even before a project is launched, however this goal is not enough. What good is a team with a good code review practice that can prevent 99% of defects but have the worst team dynamics? Thus, aside from technical goals, code reviews should have goals that promote team harmony and process efficiency. Below is a list of common goals for code reviews:

- Help the developer improve his/her coding skills.
- Identify lines of code that may be improved or may cause future defects.
- Give co-members an idea on the project at hand for awareness and promote interchangeability among team members.
- Show a different perspective that is not biased to the author of the code.
- Promote consistency of design and implementation to a certain level which addresses the problem of having recurring defect causes in the long run.
- Produce / Suggest process improvements at the end of every code review session.

From these goals, other goals may be added to improve team dynamics and code review process, or boost the confidence of the developers.

Benefits
~~~~~~~~

- To spot and fix defects early in the process.
- Better-shared understanding of the code base as team members learn from each other
- Helps to maintain a level of consistency in design and implementation.
- Helps to identify common defects across the team thus reducing rework.
- Uniformity in understanding will help interchangeability of team members in case of non-availability of any one of them.
- "Another set of eyes" adds objectivity. Similar to the reason for separating your coding and testing teams, peer reviews provide the distance needed to recognize problems.
- Team cohesiveness. Working together helps draw team members closer. It also provides a brief respite from the isolation that coding often brings.

Tips For Participants
~~~~~~~~~~~~~~~~~~~~~

Before conducting a code review, a participant should have the right mindset. Participants can be separated into two types: the author of the code and the reviewer.

**For Authors:**

- **Be the primary reviewer of your code**. First and foremost, the author should be sure that he/she knows his/her code and make sure that his/her code complies to the standards as much as he/she is aware of the things to be checked when he/she review the code of other developers.
- **Uphold the coding standards.** Follow it religiously as much as possible and avoid making your own style or rules. Aside from annotations, the standards serve as a common ground in understanding each other's code. No one wants to read bad-looking and inconsistent code. And while you're at it, give suggestions on how to improve the coding standards.
- **You are not your code.** This is an issue which concerns a developer's pride in his creation. If problems are found in your code, you can fight for your belief on your implementation but be humble enough to know that defeat is sometimes inevitable and we can't be the perfect developer. On the other hand, we feel rewarded when someone praises our code, but relying on praises and making it a basis of skill is not a good practice.
- **You are not the best so learn to consider the opinion of other developers.** Sometimes, we tend to think that we are superior but let's no forget that in another context we can be the inferior one. Be open to the suggestions of your teammates, don't disregard them. What is the purpose of code reviews if you just want to show your elegant code? Better call it code presentation rather than review.
- **Never rewrite code without permission.** Consult the original author of a code before manipulating it. There must be a reason why they implemented it as such so don't assume. You wouldn't want other person messing with your code either, anyway.

**For Reviewers:**

- **Critique the code, not the coder.** Make it a practice to give positive reinforcements that aims to improve the code. Limit your comment to code technicality such as coding standards and possible optimization. You must also understand that there is no single way of implementing code, but there should be a standard approach.
- **Ask instead of making a statement.** Avoid making statements or asking "Why" questions because they are mostly interpreted as accusatory or an attack to the developer. To keep a harmonious mood, try to properly ask for more information to understand the approach rather than push an approach that you think is better making the author feel guilty for his/her implementation. "What is your reason for using this kind of approach?" is better than saying "You should have used this approach."
- **Remember to praise.** Give praises to boost the confidence of the author or your co-reviewer wherever it is due, but not too much. It won't hurt to give praises. Some developers take this as an assurance that he/she is doing well in the task the he/she performs.
- **Conduct code reviews promptly.** Code review sessions are parts that most developers like the least because it is tedious and time-consuming. Therefore, many suggest that code reviews should be done for 200-400 lines of code (LOC) at a time and be conducted in 90 minutes or less. Reviewers become less productive and miss out more past the 400LOC or 90-minute mark.
- **"Another set of eyes" adds objectivity.** The keyword is "objectivity", do not make suggestions just for the sake of "making suggestions".

**For Both Authors and Reviewers:**

- **Code Reviews are NOT problem solving meetings.** While it's purpose is to find problems, solving it is not one of its goals.
- **Stick to the coding standards.** Make sure to follow a coding standard. Having none will lead to wasted time and messed up / unorganized reviews.
- **Cultivate a harmonious mood.** Having the right mindset, code reviews can be fun and insightful.

Documents Needed
~~~~~~~~~~~~~~~~

Code reviews needs the following documents for it to proceed smoothly (but these are just suggestions, so it may still expand) :

- **A well-annotated code.** Required. This helps the reviewer understand the code faster and better. Use the proper format stated in your coding standards.
- **A Code Review Checklist.** Required. This document makes sure that all important points are covered in a code review session. Never conduct a review without one.
- **A Fix checklist.** Required. This helps in keeping track of the fixes or improvements found and whether they are already finished or not.
- **A Common mistakes checklist.** Optional, but helpful. Write down all things that developers tend to miss out most of the time.
- **A Metrics sheet.** Optional, but helpful. This keeps track of the code review efficiency. Are we getting faster in reviewing? Are we in the right pace? Do we identify more issues? If yes, does it have any significant relation to the pace or length of the review?
A Severity-Priority matrix. Optional, but helpful. This serves as reference in prioritizing fixes / improvements.

Output
~~~~~~

It is expected that after a code review, the following minimal outputs are given:

- Improvement suggestions to improve the code review process, and
- The fix checklist with prioritization for the reference of the participants, especially the developers.

Final Notes
~~~~~~~~~~~

This guideline should help us have the right mindset when it comes to conducting code reviews. The code review aims to improve the quality of the product by identifying the possible improvements, prevent future defects and help the developer grow in terms of coding skills. This is not an avenue for blaming and it does not aim to create a battleground to know who the best developer is. We are the ones who will benefit from these reviews so we should commit to making it work well for us::


    Just remember these lines:
    The entire point of a review is to find problems,
    and problems will be found.
    You are not your code.
    Don’t take it personally when one is uncovered.


Checklist
---------

This a checklist that you follow when you are doing a code review

General
~~~~~~~

1. Is all the code easily understood?
#. Does it conform to your agreed coding conventions? These will usually cover location of braces, variable and function names, line length, indentations, formatting, and comments.
#. Is there any redundant or duplicate code?
#. Is the code as modular as possible?
#. Does it adhre to mvc standards?
#. Is there any commented out code?
#. Do loops have a set length and correct termination conditions?
#. Can any of the code be replaced with php functions? ie. a block of code that can be done using php's native function like array_merge()
#. Can any logging or debugging code be removed?
#. Are all data inputs checked (for the correct type, length, format, and range) and encoded?
#. Are errors being caught?
#. Are output values checked and encoded?
#. Are invalid parameter values handled?
#. Do comments exist and describe the intent of the code?
#. Are all functions commented?
#. Is any unusual behavior or edge-case handling described? (based on QA's scenarios; if none, skip)
#. Is the use and function of third-party libraries documented? (ie. WideImage, S3, etc)
#. Is there any incomplete code? If so, should it be removed or flagged with a suitable marker like ‘TODO’? ie // TODO

Testing
~~~~~~~

1. Is the code testable? i.e. don’t add too many or hide dependencies, unable to initialize objects, test frameworks can use methods etc.
#. Do tests exist and are they comprehensive? i.e. has at least your agreed on code coverage.
#. Do unit tests actually test that the code is performing the intended functionality?
#. Are arrays checked for ‘out-of-bound’ errors?


Coding standards
----------------

This should be considered the standard coding elements that are required to ensure a high level of technical interoperability between shared PHP code.

General
~~~~~~~

Files must use only <?php

- Files must use only UTF-8 without BOM for PHP code.
- Constants must be declared in all upper case with underscore separators.
- Do not use include, require, include_once, and require_once in classes::

    <?php
    // Make use of Yii's autloading mechanism
    // Instead set this once, better to set this in config/main.php (MainConfig.php)
    Yii::setPathOfAlias('commonPH', dirname(__FILE__).'/../../../common_ph/');
    // Load it whenever you need it
    Yii::import('commonPH.db.RJ_PDO');
    class MyClass
    {
        public function init()
        {
            $pdo = new RJ_PDO;
        }
    }
    // also see "How to import components from RJPH Project" for more details regarding this

- Opening braces for classes and methods must go on the next line, and closing braces must go on the next line after the body::

    <?php
    class MyClass
    { // next line of class
        public function __construct()
        { // next line of function

        } // after the body of function
    } // after the body of class

- Visibility must be declared on all properties and methods; abstract and final must be declared before the visibility; static must be declared after the visibility. "var" keyword must not be used to declare a property::

    <?php
    class MyClass
    {
        // Good
        public $user = array();
        public static $data = array();
        abstract public function createUser() {}
        final public static function deleteUser {}

        // Bad
        var $user = array();
        static $data = array();
        function createUser() {}
    }

- The PHP constants true, false, and null must be in lower case.
- Use docblocks to document classes and functions. We will provide an api generator (PhpDocumentor / ApiGen) to further document these classes for SDD's use. This will promote code reusability and consistency.
- Variables

    * Names should be in camelCase.
    * Private variables should start with "_"
    * Exception: CActiveRecord model's attributes are named based on the column name ie. student.student_status_id (Student::model()->student_status_id
    * Use meaningful names for variables. Variable name must define the exact explanation of its content.
    * Do not use very long names as this defeats the purpose of readability ie. $userDataThaTWasGeneratedViaCurl

- Do not use var_dump, echo, print_r

    * Use Yii::log(), this is safer especially when deploying to production.

- Strings

    * Use single quotes. Double-quotes will force php to parse the string to check if there are any variables inside it.
    * if you concatenate strings, a space must be inserted before and after the dot for better readability
    * You may break a string into multiple lines if you use the dot operator. You'll have to indent each following line to mark them as part of the value assignment
    * Optional: You should also consider using a PHP function such as sprintf() to concatenate strings to increase readability::

        <?php
        $message = 'Hey ' . $name . ', you look ' . $appearance . ' today!';

        $message = 'Hello everybody ' 
            . 'this is a multiline concatenation '
            . 'take not of the placements of the dots and spaces'
            ;

        $message = sprintf('Hey %s, you look %s today!', $name, $appearance);

    * Never use the shut-up operator @ to suppress error messages (as much as possible). It makes debugging harder, is dirty style and slow as hell
    * Prefer strict comparisons whenever possible, to avoid problems with truthy and falsy values that might behave different than what you expect::

        <?php
        if ($template)             // BAD
        if (isset($template))      // GOOD
        if ($template !== null))   // GOOD
        if ($template !== ''))     // GOOD
        if (strlen($template) > 0) // BAD! strlen("-1") is greater than 0
        if (is_string($template) && strlen($template) > 0) // BETTER
        if ($foo == $bar)          // BAD, avoid truthy comparisons
        if ($foo != $bar)          // BAD, avoid falsy comparisons
        if ($foo === $bar))        // GOOD
        if ($foo !== $bar))        // GOOD

Class
~~~~~

- Class names must be declared in StudlyCaps.
- Class constants must be declared in all upper case with underscore separators.
- In classes / models, omit php closing tab "?>"
- Filenames should be the same as class name

Class methods
~~~~~~~~~~~~~

- Method names must be declared in camelCase.
- Private methods should start with "_". (Based on Yii framework codes)::

    <?php
    class MyClass
    {
        public function createUser() {}
        private function _deleteUser() {}
    }

- Method arguments with default values must go at the end of the argument list::

    <?php
    class MyClass
    {
        public function createUser($name, $age, $status = false) {} // good
        public function deleteUser($data = array(), $id) {} // bad
    }

- Argument lists may be split across multiple lines, where each subsequent line is indented once. When doing so, the first item in the list must be on the next line, and there must be only one argument per line::

    <?php
    class MyClass
    {
        public function createUser(
            $name, 
            $age, 
            $status = false
        ) {
            ...code...
        }
        
        // same when calling the method
        $class = new MyClass;
        echo $class->createUser(
            'Robin',
            30,
            true
        );
    }

- Make method names descriptive. The name must specify the exact action of the method and for most cases must start with a verb ie. createPasswordHash().
- It returns true/false, naming should be like a question ie. isStudentApproved() -- this adds readability in the codes.
- Do not use very long names as this defeats the purpose of readability ie. saveUserDataViaCurlOnRjphServer()


Coding style
~~~~~~~~~~~~

- Code must use 4 spaces for indenting, not tabs
- Opening braces for classes must go on the next line, and closing braces must go on the next line after the body::

    <?php
    class MyClass 
    { 
        public function createSample() {} 
    }

- Control structure keywords must have one space after them. Opening braces for control structures must go on the same line, and closing braces must go on the next line after the body. Opening parentheses for control structures must not have a space after them, and closing parentheses for control structures must not have a space before::

    <?php
    // The keyword "elseif" should be used instead of 
    // "else if" so that all control keywords look like single words.
    if ($a === $b) {
        ...code...
    } elseif ($a > $b) {
        ...code...
    } else {
        ...code...
    }

    switch ($expr) {
        case 0: 
            ...code...
            break;
        case 1: 
            ...code...
            break;
        default: 
            ...code...
    }

    while ($expr) {
        ...code...
    }

    do {
        ...code...
    } while ($expr);

    for ($i = 0; $i  $value) {
        ...code...
    }

    try {
        ...code...
    } catch (PDOException$e) {
        ...code...
    } catch (Exception $e) {
        ...code...
    }


MVC
~~~

- Model

    * should contain properties to represent specific data;
    * should contain business logic (e.g. validation rules) to ensure the represented data fulfills the design requirement;
    * may contain code for manipulating data. For example, a SearchForm model, besides representing the search input data, may contain a search method to implement the actual search.
    * Use FormModel if user input is needed, don't use the CActiveRecord model directly::

        <?php
        class UserForm extends CFormModel
        {
            public function rules()
            {
                return CMap::mergeArray(User::model()->rules(), array(
                    ...your custom rules...
                ));
                // this way, the basic User model rules 
                // are always linked/sync'd with your UserForm 
                // do this if only applicable
            }
        }

    * As much as possible, use CActiveRecord models especially when saving data. This promotes consistency of data being saved (due to the validation rules and other business logic in the model).
    * If your project is using helpers, a good way of implementing it would be to create a component, ie. Yii::app()->helpers->hashString(), this will promote consistency in a team and code reusability.

- View

    * should mainly contain presentational code, such as HTML, and simple PHP code to traverse, format and render data;
    * should avoid containing code that performs explicit DB queries. Such code is better placed in models.
    * should avoid direct access to $_GET, $_POST, or other similar variables that represent the end user request. This is the controller's job. The view should be focused on the display and layout of the data provided to it by the controller and/or model, but not attempting to access request variables or the database directly.
    * may access properties and methods of controllers and models directly. However, this should be done only for the purpose of presentation.

- Controller

    * may access $_GET, $_POST and other PHP variables that represent user requests;
    * may create model instances and manage their life cycles. For example, in a typical model update action, the controller may first create the model instance; then populate the model with the user input from $_POST; after saving the model successfully, the controller may redirect the user browser to the model detail page. Note that the actual implementation of saving a model should be located in the model instead of the controller.
    * should avoid containing embedded SQL statements, which are better kept in models.
    * should avoid containing any HTML or any other presentational markup. This is better kept in views.

- CRON

    * Use Yii's console command to create cron tasks. This is very convenient because it exposes your existing models thus promoting code reusability. This is also more secure than our current process where we curl into the link (this link is open to the world, it may require some password or token but nevertheless it's still a link that we can put in an address bar). We already have a few console commands that are being used for cron jobs

        * http://192.168.11.51/svn/backend/production_biz/rjph/rjPhProtected/commands/ChatterRandomCheckCommand.php
        * Cron rule: * /15 * * * * cd /var/www/html/path-to-rjph/rjPhProtected && php yiic.php chatterRandomCheck initiateCheck
        * 5.4.1.2 http://192.168.11.51/svn/backend/shque01/rjph/rjPhProtected/commands/EmailQueueCommand.php
        * Cron rule: * * * * * cd /var/www/html/path-to-rjph/rjPhProtected && php yiic.php emailqueue send

    * Check :ref:`yiicronjob` for more details
