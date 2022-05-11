---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e8fc29032013ae6041b08450809835956eb909b8
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325238"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

caseId := "case-id"
custodianId := "custodian-id"
userSourceId := "userSource-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).CustodiansById(&custodianId).UserSourcesById(&userSourceId).Delete()


```