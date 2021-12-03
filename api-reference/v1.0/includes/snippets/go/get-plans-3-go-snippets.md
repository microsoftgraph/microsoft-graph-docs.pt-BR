---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 84962bb207e6c86078578cb04b5c4bddc4eebbf2
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286014"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Planner().Plans().Get(nil)


```