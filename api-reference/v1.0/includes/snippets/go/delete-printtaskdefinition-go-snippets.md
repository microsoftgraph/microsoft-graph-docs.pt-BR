---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6911331522bbff4bc64cdb1df46ca18555e334d4
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60983986"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

printTaskDefinitionId := "printTaskDefinition-id"
graphClient.Print().TaskDefinitionsById(&printTaskDefinitionId).Delete(options)


```