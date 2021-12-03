---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1351c7a55d03b16a2463983f8ced6804e1ac3b21
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285919"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printerId := "printer-id"
graphClient.Print().PrintersById(&printerId).RestoreFactoryDefaults().Post(nil)


```