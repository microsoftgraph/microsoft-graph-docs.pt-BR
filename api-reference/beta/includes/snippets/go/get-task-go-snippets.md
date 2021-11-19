---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b92847a233516fb9b6c61695ec444a783be99f62
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102455"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printTaskDefinitionId := "printTaskDefinition-id"
printTaskId := "printTask-id"
result, err := graphClient.Print().TaskDefinitionsById(&printTaskDefinitionId).TasksById(&printTaskId).Get(options)


```