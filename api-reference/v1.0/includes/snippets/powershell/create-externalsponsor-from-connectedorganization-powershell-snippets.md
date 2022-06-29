---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1ab59139fb09ae4b27d7c218903c6ba5f341eb86
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437804"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    "@odata.id" = "https://graph.microsoft.com/v1.0/users/{id}"
}

New-MgEntitlementManagementConnectedOrganizationExternalSponsorByRef -ConnectedOrganizationId $connectedOrganizationId -BodyParameter $params

```