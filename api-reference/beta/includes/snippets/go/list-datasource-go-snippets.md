---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 537d4d7c7ce9be8f32e391522958090e3eb3d115
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323897"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

caseId := "case-id"
noncustodialDataSourceId := "noncustodialDataSource-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).NoncustodialDataSourcesById(&noncustodialDataSourceId).DataSource().Get()


```