---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cc84a6555e3c86bba3f52f378d04808d512a3954
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324248"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUser()
accountEnabled := true
requestBody.SetAccountEnabled(&accountEnabled)
displayName := "Adele Vance"
requestBody.SetDisplayName(&displayName)
mailNickname := "AdeleV"
requestBody.SetMailNickname(&mailNickname)
userPrincipalName := "AdeleV@contoso.onmicrosoft.com"
requestBody.SetUserPrincipalName(&userPrincipalName)
passwordProfile := msgraphsdk.NewPasswordProfile()
requestBody.SetPasswordProfile(passwordProfile)
forceChangePasswordNextSignIn := true
passwordProfile.SetForceChangePasswordNextSignIn(&forceChangePasswordNextSignIn)
password := "xWwvJ]6NMw+bWH-d"
passwordProfile.SetPassword(&password)
result, err := graphClient.Users().Post(requestBody)


```