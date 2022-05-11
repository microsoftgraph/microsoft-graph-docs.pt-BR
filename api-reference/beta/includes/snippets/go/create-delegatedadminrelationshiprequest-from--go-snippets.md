---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 132ca2d0c9a5bdd494e66c1ce69364d32dbae3db
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324425"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDelegatedAdminRelationshipRequest()
action := "lockForApproval"
requestBody.SetAction(&action)
delegatedAdminRelationshipId := "delegatedAdminRelationship-id"
result, err := graphClient.TenantRelationships().DelegatedAdminRelationshipsById(&delegatedAdminRelationshipId).Requests().Post(requestBody)


```