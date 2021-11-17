---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5222b14b3f3f4be20e4fc149d5cb5f10358db995
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60975262"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

educationRubricId := "educationRubric-id"
graphClient.Education().Me().RubricsById(&educationRubricId).Delete(options)


```