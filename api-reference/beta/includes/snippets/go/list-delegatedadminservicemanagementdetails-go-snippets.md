---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3afc8aa2b4f4e061332a4f510f5f016d592a0fc2
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323360"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

delegatedAdminCustomerId := "delegatedAdminCustomer-id"
result, err := graphClient.TenantRelationships().DelegatedAdminCustomersById(&delegatedAdminCustomerId).ServiceManagementDetails().Get()


```