---
title: Tipo de recurso domainIdentitySource
description: O tipo domainIdentitySource identifica um domínio não locatário como uma fonte de identidade para uma organização conectada.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 6fe969759e07e14af08d3d69e90726dce8512445
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242209"
---
# <a name="domainidentitysource-resource-type"></a>Tipo de recurso domainIdentitySource

Namespace: microsoft.graph


Usado nas fontes de identidade de [uma connectedOrganization](connectedOrganization.md). O `@odata.type` valor indica que esse tipo identifica um domínio como uma fonte de identidade para uma organização `#microsoft.graph.domainIdentitySource` conectada.

Ao criar uma nova [connectedOrganization](../api/entitlementmanagement-post-connectedorganizations.md), se o chamador fornece na coleção identitySources um domainIdentitySource e o domínio corresponde a um domínio registrado de um locatário do Azure Active Directory, a organização conectada resultante criada terá uma coleção identitySources contendo um único membro do tipo [azureActiveDirectoryTenant.](azureactivedirectorytenant.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome da fonte de identidade, normalmente também o nome de domínio. Somente leitura. |
|domainName|Cadeia de caracteres|O nome de domínio. Somente leitura. |

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.domainIdentitySource",
  "baseType": "microsoft.graph.identitySource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.domainIdentitySource",
  "domainName": "String",
  "displayName": "String"
}
```

