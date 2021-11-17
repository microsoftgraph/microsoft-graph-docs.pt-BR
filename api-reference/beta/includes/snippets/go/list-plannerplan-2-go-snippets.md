---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 354cc4b9b0cf232a74ea76c9d59264b6db7f45d5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60989859"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

userId := "user-id"
result, err := graphClient.UsersById(&userId).Planner().RosterPlans().Get(options)


```