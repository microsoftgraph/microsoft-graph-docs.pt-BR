---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dee726c93ef5550d6f04eb3e7ed0e17118d1b8e4
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088370"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Planner().Tasks().Get(options)


```