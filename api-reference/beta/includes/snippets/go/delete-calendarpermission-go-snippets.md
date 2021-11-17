---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 23c8ef03f43e128ebf27df2199c3f4c9734b753d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61012505"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

userId := "user-id"
calendarPermissionId := "calendarPermission-id"
graphClient.UsersById(&userId).Calendar().CalendarPermissionsById(&calendarPermissionId).Delete(options)


```