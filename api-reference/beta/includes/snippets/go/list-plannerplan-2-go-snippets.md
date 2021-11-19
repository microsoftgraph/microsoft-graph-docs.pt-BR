---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 22ae7a902fe646cfe389257508190803e9c7dbb3
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091836"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
result, err := graphClient.UsersById(&userId).Planner().RosterPlans().Get(options)


```