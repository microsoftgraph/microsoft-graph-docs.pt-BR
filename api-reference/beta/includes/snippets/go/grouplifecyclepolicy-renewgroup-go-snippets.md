---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3208efe4be5978feb13ec8ec7fef69ff3cc7c709
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60986379"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
groupId := "ffffffff-ffff-ffff-ffff-ffffffffffff"
requestBody.SetGroupId(&groupId)
options := &msgraphsdk.RenewGroupRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.GroupLifecyclePolicies().RenewGroup().Post(options)


```