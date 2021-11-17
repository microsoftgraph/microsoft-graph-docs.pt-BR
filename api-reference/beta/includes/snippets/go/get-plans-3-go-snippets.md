---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 479c1229f65802ade4e1dedeb34463d57e7981e9
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60989907"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Me().Planner().Plans().Get(options)


```