---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5676e5cc5a33f04aeec990b62f10042f1254bc97
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322280"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printTaskDefinitionId := "printTaskDefinition-id"
printTaskId := "printTask-id"
result, err := graphClient.Print().TaskDefinitionsById(&printTaskDefinitionId).TasksById(&printTaskId).Get()


```