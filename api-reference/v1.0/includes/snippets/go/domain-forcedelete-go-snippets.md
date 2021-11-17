---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 327358c8eb0fc5b56c9b8d428abfc0be89ae7776
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60973924"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
disableUserAccounts := true
requestBody.SetDisableUserAccounts(&disableUserAccounts)
options := &msgraphsdk.ForceDeleteRequestBuilderPostOptions{
    Body: requestBody,
}
domainId := "domain-id"
graphClient.DomainsById(&domainId).ForceDelete().Post(options)


```