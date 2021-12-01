---
title: Tipo de recurso externalDomainFederation
description: O tipo externalDomainFederation identifica um domínio não locatário com um provedor de identidade configurado como uma fonte de identidade para uma organização conectada.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: af47b7516e656ad85cbe1f8ef2fde3f0681ee89c
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242194"
---
# <a name="externaldomainfederation-resource-type"></a>Tipo de recurso externalDomainFederation

Namespace: microsoft.graph


Usado nas fontes de identidade de [uma connectedOrganization](connectedOrganization.md). O valor indica que esse tipo identifica um domínio com um provedor de identidade configurado como uma fonte de `@odata.type` identidade para uma organização `#microsoft.graph.externalDomainFederation` conectada.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome da fonte de identidade, normalmente também o nome de domínio. Somente leitura. |
|domainName|Cadeia de caracteres|O nome de domínio. Somente leitura. |
|issuerUri|Cadeia de caracteres|O emissorURI da federação de entrada. Somente leitura. |

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalDomainFederation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.externalDomainFederation",
  "issuerUri": "String",
  "domainName": "String",
  "displayName": "String"
}
```


