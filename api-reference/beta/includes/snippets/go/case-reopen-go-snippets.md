---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4c44a7594f4232dedd796a58189fd9d6aa9fda73
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324811"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

caseId := "case-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).Reopen(case-id).Post()


```