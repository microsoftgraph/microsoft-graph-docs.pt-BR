---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4dbd98027124979ff7b3eba1131f0033510fcfb4
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322530"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPasswordCredentialRequestBody()
passwordCredential := msgraphsdk.NewPasswordCredential()
requestBody.SetPasswordCredential(passwordCredential)
displayName := "Password friendly name"
passwordCredential.SetDisplayName(&displayName)
applicationId := "application-id"
result, err := graphClient.ApplicationsById(&applicationId).AddPassword(application-id).Post(requestBody)


```