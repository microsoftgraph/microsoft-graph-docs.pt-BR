---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1133c4a66320d8af913149bb50c25308caf1d587
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60987626"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Me().Analytics().ActivityStatistics().Get(options)


```