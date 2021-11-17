---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f4d4a4f0db214d12d69399ad763890685f437fff
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61033029"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

plannerBucketId := "plannerBucket-id"
result, err := graphClient.Planner().BucketsById(&plannerBucketId).Tasks().Get(options)


```