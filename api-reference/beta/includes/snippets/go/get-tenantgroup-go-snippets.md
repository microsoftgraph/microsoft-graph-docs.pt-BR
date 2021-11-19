---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 86d2fa4482ae4d1303dcf100a4b6551733d46216
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089734"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

tenantGroupId := "tenantGroup-id"
result, err := graphClient.TenantRelationships().ManagedTenants().TenantGroupsById(&tenantGroupId).Get(options)


```