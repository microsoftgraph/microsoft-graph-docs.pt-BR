---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ec02890bbc3c38ed23ade3f9e0a2e89085a78b9c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61026287"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

servicePrincipalId := "servicePrincipal-id"
appRoleAssignmentId := "appRoleAssignment-id"
graphClient.ServicePrincipalsById(&servicePrincipalId).AppRoleAssignmentsById(&appRoleAssignmentId).Delete(options)


```