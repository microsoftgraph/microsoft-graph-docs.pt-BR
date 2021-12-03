---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9f40f9ba8adde739c282f3d378c1502ed89301d3
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287316"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
appRoleAssignmentId := "appRoleAssignment-id"
graphClient.GroupsById(&groupId).AppRoleAssignmentsById(&appRoleAssignmentId).Delete(nil)


```