---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 169ad4e5e0b755e4d7b7ebc667495162eb16bbd9
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087930"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

plannerBucketId := "plannerBucket-id"
result, err := graphClient.Planner().BucketsById(&plannerBucketId).Get(options)


```