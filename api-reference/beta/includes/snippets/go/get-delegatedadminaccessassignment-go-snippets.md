---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e29534ca596581ba1c7df87cebe7611edc7fc058
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323801"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

delegatedAdminRelationshipId := "delegatedAdminRelationship-id"
delegatedAdminAccessAssignmentId := "delegatedAdminAccessAssignment-id"
result, err := graphClient.TenantRelationships().DelegatedAdminRelationshipsById(&delegatedAdminRelationshipId).AccessAssignmentsById(&delegatedAdminAccessAssignmentId).Get()


```