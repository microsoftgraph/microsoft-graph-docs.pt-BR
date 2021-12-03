---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d6d789288fcdc2a89d0d86dc91aa0931fcc091aa
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286757"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Schedule().SchedulingGroups().Get(nil)


```