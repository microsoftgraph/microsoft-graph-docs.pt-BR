---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d0b10585721d4f0bf4b7f0274fc919a4003ead63
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325237"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

caseId := "case-id"
custodianId := "custodian-id"
userSourceId := "userSource-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).CustodiansById(&custodianId).UserSourcesById(&userSourceId).Get()


```