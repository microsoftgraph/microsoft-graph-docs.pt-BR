---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 77ab95337dcf48d001fbfdfb0bfde98383a098e5
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49752791"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentPolicy accessPackageAssignmentPolicy = new AccessPackageAssignmentPolicy();
accessPackageAssignmentPolicy.id = "b2eba9a1-b357-42ee-83a8-336522ed6cbf";
accessPackageAssignmentPolicy.accessPackageId = "4c02f928-7752-49aa-8fc8-e286d973a965";
accessPackageAssignmentPolicy.displayName = "All Users";
accessPackageAssignmentPolicy.description = "All users can request for access to the directory.";
accessPackageAssignmentPolicy.canExtend = false;
accessPackageAssignmentPolicy.durationInDays = 365;
accessPackageAssignmentPolicy.expirationDateTime = CalendarSerializer.deserialize("null");
RequestorSettings requestorSettings = new RequestorSettings();
requestorSettings.scopeType = "AllExistingConnectedOrganizationSubjects";
requestorSettings.acceptRequests = true;
LinkedList<UserSet> allowedRequestorsList = new LinkedList<UserSet>();
requestorSettings.allowedRequestors = allowedRequestorsList;
accessPackageAssignmentPolicy.requestorSettings = requestorSettings;
ApprovalSettings requestApprovalSettings = new ApprovalSettings();
requestApprovalSettings.isApprovalRequired = true;
requestApprovalSettings.isApprovalRequiredForExtension = false;
requestApprovalSettings.isRequestorJustificationRequired = true;
requestApprovalSettings.approvalMode = "SingleStage";
LinkedList<ApprovalStage> approvalStagesList = new LinkedList<ApprovalStage>();
ApprovalStage approvalStages = new ApprovalStage();
approvalStages.approvalStageTimeOutInDays = 14;
approvalStages.isApproverJustificationRequired = true;
approvalStages.isEscalationEnabled = true;
approvalStages.escalationTimeInMinutes = 11520;
LinkedList<UserSet> primaryApproversList = new LinkedList<UserSet>();
GroupMembers primaryApprovers = new GroupMembers();
primaryApprovers.isBackup = true;
primaryApprovers.id = "d2dcb9a1-a445-42ee-83a8-476522ed6cbf";
primaryApprovers.description = "group for users from connected organizations which have no external sponsor";
primaryApproversList.add(primaryApprovers);
ExternalSponsors primaryApprovers1 = new ExternalSponsors();
primaryApprovers1.isBackup = false;
primaryApproversList.add(primaryApprovers1);
approvalStages.primaryApprovers = primaryApproversList;
approvalStagesList.add(approvalStages);
requestApprovalSettings.approvalStages = approvalStagesList;
accessPackageAssignmentPolicy.requestApprovalSettings = requestApprovalSettings;
AssignmentReviewSettings accessReviewSettings = new AssignmentReviewSettings();
accessReviewSettings.isEnabled = false;
accessPackageAssignmentPolicy.accessReviewSettings = accessReviewSettings;
LinkedList<AccessPackageQuestion> questionsList = new LinkedList<AccessPackageQuestion>();
AccessPackageMultipleChoiceQuestion questions = new AccessPackageMultipleChoiceQuestion();
questions.isRequired = false;
AccessPackageLocalizedContent text = new AccessPackageLocalizedContent();
text.defaultText = "what state are you from?";
LinkedList<AccessPackageLocalizedText> localizedTextsList = new LinkedList<AccessPackageLocalizedText>();
AccessPackageLocalizedText localizedTexts = new AccessPackageLocalizedText();
localizedTexts.text = "¿De qué estado eres?";
localizedTexts.languageCode = "es";
localizedTextsList.add(localizedTexts);
text.localizedTexts = localizedTextsList;
questions.text = text1;
LinkedList<AccessPackageAnswerChoice> choicesList = new LinkedList<AccessPackageAnswerChoice>();
AccessPackageAnswerChoice choices = new AccessPackageAnswerChoice();
choices.actualValue = "AZ";
AccessPackageLocalizedContent displayValue = new AccessPackageLocalizedContent();
LinkedList<AccessPackageLocalizedText> localizedTextsList1 = new LinkedList<AccessPackageLocalizedText>();
AccessPackageLocalizedText localizedTexts1 = new AccessPackageLocalizedText();
localizedTexts1.text = "Arizona";
localizedTexts1.languageCode = "es";
localizedTextsList1.add(localizedTexts1);
displayValue.localizedTexts = localizedTextsList1;
choices.displayValue = displayValue;
choicesList.add(choices);
AccessPackageAnswerChoice choices1 = new AccessPackageAnswerChoice();
choices1.actualValue = "CA";
AccessPackageLocalizedContent displayValue1 = new AccessPackageLocalizedContent();
LinkedList<AccessPackageLocalizedText> localizedTextsList2 = new LinkedList<AccessPackageLocalizedText>();
AccessPackageLocalizedText localizedTexts2 = new AccessPackageLocalizedText();
localizedTexts2.text = "California";
localizedTexts2.languageCode = "es";
localizedTextsList2.add(localizedTexts2);
displayValue1.localizedTexts = localizedTextsList2;
choices1.displayValue = displayValue1;
choicesList.add(choices1);
questions.choices = choicesList;
questions.allowsMultipleSelection = false;
questionsList.add(questions);
AccessPackageTextInputQuestion questions1 = new AccessPackageTextInputQuestion();
questions1.isRequired = false;
AccessPackageLocalizedContent text4 = new AccessPackageLocalizedContent();
text4.defaultText = "Who is your manager?";
LinkedList<AccessPackageLocalizedText> localizedTextsList3 = new LinkedList<AccessPackageLocalizedText>();
AccessPackageLocalizedText localizedTexts3 = new AccessPackageLocalizedText();
localizedTexts3.text = "por qué necesita acceso a este paquete";
localizedTexts3.languageCode = "es";
localizedTextsList3.add(localizedTexts3);
text4.localizedTexts = localizedTextsList3;
questions1.text = text5;
questions1.isSingleLineQuestion = false;
questionsList.add(questions1);
accessPackageAssignmentPolicy.questions = questionsList;

graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentPolicies("b2eba9a1-b357-42ee-83a8-336522ed6cbf")
    .buildRequest()
    .put(accessPackageAssignmentPolicy);

```