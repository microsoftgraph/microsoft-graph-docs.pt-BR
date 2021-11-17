---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 27823091410cef2e2fd3fce9e46ce7d98efa3df1
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61006226"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

educationRubricId := "educationRubric-id"
result, err := graphClient.Education().Me().RubricsById(&educationRubricId).Get(options)


```