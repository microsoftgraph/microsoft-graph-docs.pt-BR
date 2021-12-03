---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb5224f38071a443b2bde4c0912924a629646e99
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286328"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Planner().RecentPlans().Get(nil)


```