---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1399491d35b026b73a4cb874e7b1629db23355d7
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287127"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printerShareId := "printerShare-id"
graphClient.Print().SharesById(&printerShareId).Delete(nil)


```