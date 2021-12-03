---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e783be60dd18265ad0f6a09a6d0efb1eefe6d26c
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286558"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

setId := "set-id"
termId := "term-id"
graphClient.TermStore().SetsById(&setId).TermsById(&termId).Delete(nil)


```