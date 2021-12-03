---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: db77d9b80a269584556d5aa7f401e4d88f91e9bf
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287384"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

setId := "set-id"
graphClient.TermStore().SetsById(&setId).Delete(nil)


```