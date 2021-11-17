---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c35415d7a16965f4fa7f453184324e2ed9e39c71
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61021577"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

printTaskDefinitionId := "printTaskDefinition-id"
printTaskId := "printTask-id"
result, err := graphClient.Print().TaskDefinitionsById(&printTaskDefinitionId).TasksById(&printTaskId).Get(options)


```