---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7b98463c12cf84a3dcb8f2b6484d731f8c453e03
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286747"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

caseId := "case-id"
custodianId := "custodian-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).CustodiansById(&custodianId).UnifiedGroupSources().Get(nil)


```