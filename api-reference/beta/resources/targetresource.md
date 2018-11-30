---
title: tipo de recurso de targetResource
description: Indica uma coleção de tipos de recursos de destino associado à atividade de auditoria. Cada tipo de recurso de destino herdará as propriedades descritas abaixo deste recurso.
ms.openlocfilehash: ba3bee7ce89f73ed97610d62676c22d14488ed9f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033559"
---
# <a name="targetresource-resource-type"></a>tipo de recurso de targetResource
Indica uma coleção de tipos de recursos de destino associado à atividade de auditoria. Cada tipo de recurso de destino herdará as propriedades descritas abaixo deste recurso.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|displayName|String|Indica o nome de exibição dos recursos descritos em tipos de recursos de destino abaixo.|
|id|String|Indica a Id exclusiva do recurso (por exemplo: UserId, AppId, RoleId.).|
|ModifiedProperties|coleção [modifiedProperty](modifiedproperty.md)|Indica o nome, o valor antigo e o novo valor de cada atributo a ser alterado. Isso é aplicável para qualquer atividades "Atualizar"|

### <a name="target-resource-types"></a>Tipos de recursos de destino

O tipo de recurso de destino varia de acordo com o recurso subjacente:

|Nome do recurso| Referência|
|-------------|----------|
Dispositivo|[targetResourceDevice](targetresourcedevice.md)
Diretório|[targetResourceDirectory] (targetresourcedirectory.md]
Group|[targetResourceGroup](targetresourcegroup.md)
Política|[targetResourcePolicy](targetresourcepolicy.md)
Role|[targetResourceRole](targetresourcerole.md)
Entidade de serviço|[targetResourceServicePrincipal](targetresourceserviceprincipal.md)
Usuário|[targetResourceUser](targetresourceuser.md)
Outro|[targetResourceOther](targetresourceother.md)

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResource"
}-->

```json
{
  "displayName": "String",
  "id": "String",
  "modifiedProperties": [{"@odata.type": "microsoft.graph.modifiedProperty"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->