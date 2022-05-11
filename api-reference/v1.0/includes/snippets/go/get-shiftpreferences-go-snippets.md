---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 843f7af2e8f13476a9cc149042b624fecdbac59c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323381"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
result, err := graphClient.UsersById(&userId).Settings().ShiftPreferences().Get()


```