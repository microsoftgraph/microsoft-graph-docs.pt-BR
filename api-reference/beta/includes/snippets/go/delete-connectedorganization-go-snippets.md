---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fb5e9dc8cacf587d0bea1e67212caa7b483e72aa
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61005736"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

connectedOrganizationId := "connectedOrganization-id"
graphClient.IdentityGovernance().EntitlementManagement().ConnectedOrganizationsById(&connectedOrganizationId).Delete(options)


```