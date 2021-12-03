---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8733eb94a6560477c2e1a547f9f2102b63b7e02f
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286031"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
calendarPermissionId := "calendarPermission-id"
result, err := graphClient.UsersById(&userId).Calendar().CalendarPermissionsById(&calendarPermissionId).Get(nil)


```