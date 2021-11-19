---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6810e228ed166f86f69ed4aa38fde2fe59fe3b8a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085346"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAgreement()
displayName := "MSGraph Sample"
requestBody.SetDisplayName(&displayName)
isViewingBeforeAcceptanceRequired := true
requestBody.SetIsViewingBeforeAcceptanceRequired(&isViewingBeforeAcceptanceRequired)
requestBody.SetFiles( []AgreementFileLocalization {
    msgraphsdk.NewAgreementFileLocalization(),
    SetAdditionalData(map[string]interface{}{
        "fileName": "TOU.pdf",
        "language": "en",
        "isDefault": true,
    }
}
options := &msgraphsdk.AgreementsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.IdentityGovernance().TermsOfUse().Agreements().Post(options)


```