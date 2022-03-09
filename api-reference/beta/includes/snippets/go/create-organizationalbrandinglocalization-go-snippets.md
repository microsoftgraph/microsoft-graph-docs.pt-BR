---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ad9dd07565cc3573b819659655f6592a5b3f3994
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63394793"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOrganizationalBrandingLocalization()
backgroundColor := "#00000F"
requestBody.SetBackgroundColor(&backgroundColor)
id := "fr-FR"
requestBody.SetId(&id)
signInPageText := " "
requestBody.SetSignInPageText(&signInPageText)
options := &msgraphsdk.LocalizationsRequestBuilderPostOptions{
    Body: requestBody,
}
organizationId := "organization-id"
result, err := graphClient.OrganizationById(&organizationId).Branding().Localizations().Post(options)


```