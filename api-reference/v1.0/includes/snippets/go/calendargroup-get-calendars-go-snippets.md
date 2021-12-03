---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6af68b5e8bc25759654a0b7307d3a54cff2bc9db
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287172"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

calendarGroupId := "calendarGroup-id"
result, err := graphClient.Me().CalendarGroupsById(&calendarGroupId).Calendars().Get(nil)


```