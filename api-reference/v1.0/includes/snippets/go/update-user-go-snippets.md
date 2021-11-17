---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9af9446e5ca57827746a037509d57fd1eb272ad9
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61008333"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewUser()
requestBody.SetBusinessPhones( []String {
    "+1 425 555 0109",
}
officeLocation := "18/2111"
requestBody.SetOfficeLocation(&officeLocation)
options := &msgraphsdk.MeRequestBuilderPatchOptions{
    Body: requestBody,
}
graphClient.Me().Patch(options)


```