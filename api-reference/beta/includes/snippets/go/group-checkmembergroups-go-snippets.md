---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9100427db73782cdef7b120785835acdc7e60725
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61020856"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetGroupIds( []String {
    "groupIds-value",
}
options := &msgraphsdk.CheckMemberGroupsRequestBuilderPostOptions{
    Body: requestBody,
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).CheckMemberGroups().Post(options)


```