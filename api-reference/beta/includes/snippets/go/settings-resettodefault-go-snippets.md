---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 496d5f034ce47ec1c60ad4f14d1b8e730936b7b0
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286935"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

caseId := "case-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).Settings().ResetToDefault().Post(nil)


```