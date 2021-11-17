---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7620fe1c9339c5fa020491d0e141571e171fd81b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61005666"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

connectedOrganizationId := "connectedOrganization-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().ConnectedOrganizationsById(&connectedOrganizationId).InternalSponsors().Get(options)


```