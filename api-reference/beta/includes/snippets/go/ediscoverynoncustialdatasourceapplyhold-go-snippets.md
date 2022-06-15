---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f8518cee5b124c70b8a75550a46e61c1859edac0
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092241"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

ediscoveryCaseId := "ediscoveryCase-id"
ediscoveryNoncustodialDataSourceId := "ediscoveryNoncustodialDataSource-id"
graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).NoncustodialDataSourcesById(&ediscoveryNoncustodialDataSourceId).ApplyHold(ediscoveryCase-id, ediscoveryNoncustodialDataSource-id).Post()


```