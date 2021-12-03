---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eee0418a34a4639d120877f5a36f266284e8c40f
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287066"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
result, err := graphClient.UsersById(&userId).Planner().RosterPlans().Get(nil)


```