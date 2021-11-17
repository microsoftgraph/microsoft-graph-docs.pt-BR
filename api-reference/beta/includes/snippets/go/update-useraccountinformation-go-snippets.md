---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4790d90a27eceb02bdb8b862284d73879f2eae66
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60984875"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewUserAccountInformation()
countryCode := "NO"
requestBody.SetCountryCode(&countryCode)
options := &msgraphsdk.UserAccountInformationRequestBuilderPatchOptions{
    Body: requestBody,
}
userAccountInformationId := "userAccountInformation-id"
graphClient.Me().Profile().AccountById(&userAccountInformationId).Patch(options)


```