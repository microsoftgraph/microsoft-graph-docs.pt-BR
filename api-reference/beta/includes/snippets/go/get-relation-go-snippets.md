---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b2fd76c9198176fa6efb38bbcb504ff446684fc5
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287288"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

setId := "set-id"
result, err := graphClient.TermStore().SetsById(&setId).Relations().Get(nil)


```