---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5f46b342b6bceb74014c40a1970ff1f543625229
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095830"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

ediscoveryCaseId := "ediscoveryCase-id"
ediscoveryCustodianId := "ediscoveryCustodian-id"
result, err := graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).CustodiansById(&ediscoveryCustodianId).Get()


```