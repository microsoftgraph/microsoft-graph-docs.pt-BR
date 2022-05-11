---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: efb4db0d0af51a39d20d3a047de27b19d6f3c8aa
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325030"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printerShareId := "printerShare-id"
graphClient.Print().SharesById(&printerShareId).Delete()


```