# How to submit questions
You may submit questions in one of three ways:
## 1. By submitting an issue with your question

Submit a [proposed question issue](https://github.com/robfentress/was-practice/issues/new?assignees=&labels=proposed+question&template=proposed-question.md&title=%5BQUESTION%5D). The requirements for the question are as follows:

* It should be a multiple choice question 
  * with four possible answers and 
  * only one correct answer.  
* It should be written in [GIFT format](https://docs.moodle.org/37/en/GIFT_format#Multiple_choice).  Please use the [GIFT Question Editor](https://fuhrmanator.github.io/GIFT-grammar-PEG.js/docs/editor/editor.html) to validate that your question can be parsed correctly before submitting.
* It should not include a title

Precede your questions with comments that include:
* The numbered _"study task"_ listed in the [Web Accessibility Specialist Body of Knowledge](https://iaap.membershipsoftware.org/files/IAAP%20WAS%20BOK%202018.docx) that your question relates to.  If there is no study task, include the section of the CPACC your question relates to.
* A reference to any source materials you are basing the question on

***

An example submission would be something like this:

### Question
```
// Study task: I:A.1.a Understand the relationship between principles, guidelines, success criteria, and their related success/failure techniques.

// Sources:
// The [Web Accessibility Specialist Body of Knowledge](https://iaap.membershipsoftware.org/files/IAAP%20WAS%20BOK%202018.docx)
// [Understanding Conformance](https://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html)

In order for content to be considered to conform to WCAG, which of the following must not be violated?
{
  ~Success/Failure Techniques
  ~Guidelines
  ~Principles
  =Success Criteria
}
```
## 2. By forking repository and submitting a pull request

[GitHub Standard Fork & Pull Request Workflow](https://gist.github.com/Chaser324/ce0505fbed06b947d962)

## 3. If a contributor, by creating a branch and submitting a pull request

If you are regularly submitting questions, you can request to be added as a contributor.  All contributors added to the project should have already passed the WAS exam. As a contributor, you won't have to fork the project.  Rather, you can just create a branch in the base repository and make a pull request from that branch.  Also, as a contributor, you'll be able to make comments on other's pull requests to help in the peer review of questions.  Just open a [contributor request issue](https://github.com/robfentress/was-practice/issues/new?assignees=&labels=&template=contributor-request.md&title=).

## License

By contributing questions, you confirm that what you have submitted is not otherwise copyrighted material and agree to license your contribution under the terms of the [Creative Commons Attribution Share Alike 4.0 International](https://github.com/robfentress/was-practice/blob/master/LICENSE)
