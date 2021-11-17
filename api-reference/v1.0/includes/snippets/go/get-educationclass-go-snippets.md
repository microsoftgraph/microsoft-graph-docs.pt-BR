---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 520b033bb8d290181b90cf36dec14018c74d6fab
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61025651"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

educationClassId := "educationClass-id"
result, err := graphClient.Education().ClassesById(&educationClassId).Get(options)


```