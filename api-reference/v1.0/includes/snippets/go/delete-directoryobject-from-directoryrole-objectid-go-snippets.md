---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de661e8208bff23d90ad2b51d0592fa51f676c6f
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694627"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

directoryRoleId := "directoryRole-id"
directoryObjectId := "directoryObject-id"
graphClient.DirectoryRolesById(&directoryRoleId).MembersById(&directoryObjectId).$ref().Delete()


```