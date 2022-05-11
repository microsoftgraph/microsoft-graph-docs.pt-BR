---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7da294b7ab69cc4097bc54b65dbfeac9072e1d60
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323454"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

caseId := "case-id"
noncustodialDataSourceId := "noncustodialDataSource-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).NoncustodialDataSourcesById(&noncustodialDataSourceId).Release(case-id, noncustodialDataSource-id).Post()


```