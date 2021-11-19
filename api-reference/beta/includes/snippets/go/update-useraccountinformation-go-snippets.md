---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 75e11b4628cb6cd491c987997e6b1ee47d3f5597
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086859"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUserAccountInformation()
countryCode := "NO"
requestBody.SetCountryCode(&countryCode)
options := &msgraphsdk.UserAccountInformationRequestBuilderPatchOptions{
    Body: requestBody,
}
userAccountInformationId := "userAccountInformation-id"
graphClient.Me().Profile().AccountById(&userAccountInformationId).Patch(options)


```