---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7645d57d519af38b84ae3b9276221612cb4bf49a
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287433"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

programId := "program-id"
graphClient.ProgramsById(&programId).Delete(nil)


```