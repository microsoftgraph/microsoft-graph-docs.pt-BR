---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cb4aeb9a283ea3a34763c7fca46787421aa58bd7
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097954"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Planner().RecentPlans().Get(options)


```