---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d6918ab6e1c89171094f3e29b2e3c005fddc3a2c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323795"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

caseId := "case-id"
custodianId := "custodian-id"
unifiedGroupSourceId := "unifiedGroupSource-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).CustodiansById(&custodianId).UnifiedGroupSourcesById(&unifiedGroupSourceId).Delete()


```