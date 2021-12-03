---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 98b4154096847aefa5e94c22b5655f82dd9f0c7b
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286262"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().CalendarGroups().Get(nil)


```