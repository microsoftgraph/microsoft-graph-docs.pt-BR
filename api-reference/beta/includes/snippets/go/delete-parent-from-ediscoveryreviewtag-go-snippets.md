---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 429d25dd0c071c2d41e504d7213e240ea7d18799
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095348"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

ediscoveryCaseId := "ediscoveryCase-id"
ediscoveryReviewTagId := "ediscoveryReviewTag-id"
graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).TagsById(&ediscoveryReviewTagId).Delete()


```