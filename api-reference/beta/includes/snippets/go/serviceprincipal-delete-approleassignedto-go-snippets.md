---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 463a2c15094c0abee4f3219b6c89d3d0ca98c113
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287184"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

servicePrincipalId := "servicePrincipal-id"
appRoleAssignmentId := "appRoleAssignment-id"
graphClient.ServicePrincipalsById(&servicePrincipalId).AppRoleAssignedToById(&appRoleAssignmentId).Delete(nil)


```