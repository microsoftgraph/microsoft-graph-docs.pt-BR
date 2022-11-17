---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2823b77b32fec07598de9c06a9416794bc96afc5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60985371"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Me().Planner().RecentPlans().Get(options)


```