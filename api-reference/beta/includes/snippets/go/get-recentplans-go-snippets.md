---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 985f2742f6d01bd3a5624a3487fe8b9b68ea60e7
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323317"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Planner().RecentPlans().Get()


```