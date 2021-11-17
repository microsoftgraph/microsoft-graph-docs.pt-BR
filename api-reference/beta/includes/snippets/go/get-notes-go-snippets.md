---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d1c13f9d57be123b2ea69d5350b9b31dbbf098b3
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019400"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Me().Profile().Notes().Get(options)


```