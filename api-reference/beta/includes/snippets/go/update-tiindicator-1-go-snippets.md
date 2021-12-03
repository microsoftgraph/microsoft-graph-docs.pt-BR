---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 062cdcf2ebfe5ee3676c859291f1cd525dc8bb52
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287061"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

tiIndicatorId := "tiIndicator-id"
graphClient.Security().TiIndicatorsById(&tiIndicatorId).Patch(nil)


```