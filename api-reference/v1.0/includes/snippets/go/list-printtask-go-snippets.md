---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9a194fcba1c79e65165c176e4d0b12d4ecfa3383
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287155"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printTaskDefinitionId := "printTaskDefinition-id"
result, err := graphClient.Print().TaskDefinitionsById(&printTaskDefinitionId).Tasks().Get(nil)


```