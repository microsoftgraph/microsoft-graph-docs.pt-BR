---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 63e5dc9163d514b8571602474590efda19c9b31a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61024922"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

domainId := "domain-id"
result, err := graphClient.DomainsById(&domainId).Verify().Post(options)


```