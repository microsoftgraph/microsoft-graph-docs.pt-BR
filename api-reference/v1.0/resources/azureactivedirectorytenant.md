---
title: Tipo de recurso do azureActiveDirectoryTenant
description: O tipo azureActiveDirectoryTenant identifica outro locatário Azure Active Directory como uma fonte de identidade para uma organização conectada.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 35c517d23b59756d59412e5b898e6b222cc0f8db
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242251"
---
# <a name="azureactivedirectorytenant-resource-type"></a>Tipo de recurso do azureActiveDirectoryTenant

Namespace: microsoft.graph


Usado nas fontes de identidade de [uma connectedOrganization](connectedOrganization.md). O valor indica que esse tipo identifica outro locatário Azure Active Directory como uma fonte de `@odata.type` identidade para uma organização `#microsoft.graph.azureActiveDirectoryTenant` conectada.

Ao criar uma nova [connectedOrganization](../api/entitlementmanagement-post-connectedorganizations.md), se o chamador fornece na coleção identitySources um domainIdentitySource e o domínio corresponde a um domínio registrado de um locatário do Azure Active Directory, a organização conectada resultante criada terá uma coleção identitySources contendo um único membro do tipo [azureActiveDirectoryTenant.](azureactivedirectorytenant.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome do Azure Active Directory locatário. Somente leitura. |
|tenantId|String|A ID do Azure Active Directory locatário. Somente leitura. |

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.azureActiveDirectoryTenant",
  "baseType": "microsoft.graph.identitySource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.azureActiveDirectoryTenant",
  "tenantId": "String",
  "displayName": "String"
}
```



