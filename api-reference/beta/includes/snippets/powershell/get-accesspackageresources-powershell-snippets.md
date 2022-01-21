---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 490ce94f222cfea44bef48d1eef7e28cce5851f4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62091103"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

Get-MgEntitlementManagementAccessPackageCatalogAccessPackageResource -AccessPackageCatalogId $accessPackageCatalogId -Filter "resourceType eq 'Application'" -ExpandProperty "accessPackageResourceScopes" 

```