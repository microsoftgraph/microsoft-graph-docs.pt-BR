---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1944173406cf7a5eb9817e0261e51c0ed39350f9
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694613"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
directoryObjectId := "directoryObject-id"
graphClient.GroupsById(&groupId).OwnersById(&directoryObjectId).$ref().Delete()


```