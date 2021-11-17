---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5cec55f9f2c3fdea58a34aae5545999a9fd1d0ce
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61031125"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
securityEnabledOnly := true
requestBody.SetSecurityEnabledOnly(&securityEnabledOnly)
options := &msgraphsdk.GetMemberGroupsRequestBuilderPostOptions{
    Body: requestBody,
}
directoryObjectId := "directoryObject-id"
result, err := graphClient.DirectoryObjectsById(&directoryObjectId).GetMemberGroups().Post(options)


```