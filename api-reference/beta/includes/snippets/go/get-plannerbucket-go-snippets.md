---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 49d052ff59152fefbb3a7ad6d3bc715537dd3377
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323004"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

plannerBucketId := "plannerBucket-id"
result, err := graphClient.Planner().BucketsById(&plannerBucketId).Get()


```