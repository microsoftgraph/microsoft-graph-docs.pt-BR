---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cd72716f12cab30c47edad3c5839bc9ef47af5c6
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287012"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

caseId := "case-id"
custodianId := "custodian-id"
unifiedGroupSourceId := "unifiedGroupSource-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).CustodiansById(&custodianId).UnifiedGroupSourcesById(&unifiedGroupSourceId).Delete(nil)


```