---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 10cd00f8b72aeec087b38a1a7247e82cddc70794
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286999"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
appRoleAssignmentId := "appRoleAssignment-id"
graphClient.UsersById(&userId).AppRoleAssignmentsById(&appRoleAssignmentId).Delete(nil)


```