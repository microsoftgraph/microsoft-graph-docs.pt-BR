---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 71384c832f492e4a35c517c63a71596b8cc1a26d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100723"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
calendarPermissionId := "calendarPermission-id"
graphClient.UsersById(&userId).Calendar().CalendarPermissionsById(&calendarPermissionId).Delete(options)


```