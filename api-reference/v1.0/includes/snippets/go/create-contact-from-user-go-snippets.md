---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c8e388e7afb23837045d34b7873eb78d52089772
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323729"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewContact()
givenName := "Pavel"
requestBody.SetGivenName(&givenName)
surname := "Bansky"
requestBody.SetSurname(&surname)
requestBody.SetEmailAddresses( []EmailAddress {
    msgraphsdk.NewEmailAddress(),
    SetAdditionalData(map[string]interface{}{
        "address": "pavelb@fabrikam.onmicrosoft.com",
        "name": "Pavel Bansky",
    }
}
requestBody.SetBusinessPhones( []String {
    "+1 732 555 0102",
}
result, err := graphClient.Me().Contacts().Post(requestBody)


```