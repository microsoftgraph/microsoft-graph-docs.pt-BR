---
title: tipo de recurso organizationSettings
description: Contém configurações que se aplicam à organização ou aos objetos de usuário dentro dela.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: e95bae902b444735b87fa7b29e061bf9bf2629ba
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998471"
---
# <a name="organizationsettings-resource-type"></a>tipo de recurso organizationSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém configurações que se aplicam à [organização](organization.md) ou que devem ser aplicadas a objetos de [usuário](user.md) em uma organização.

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter configurações da organização](../api/organizationsettings-get.md) | [organizationSettings](organizationsettings.md) | Leia o objeto de configurações da organização. |
| [Criar profileCardProperty](../api/organizationsettings-post-profilecardproperties.md) | [profileCardProperty](profilecardproperty.md) | Crie um novo **profileCardProperty** postando na coleção de objetos **profileCardProperty** . |
| [Listar profileCardProperties](../api/organizationsettings-list-profilecardproperties.md) | coleção [profileCardProperty](profilecardproperty.md) | Obtenha uma coleção de objetos **profileCardProperty** . |
| [Obter itemInsightsSettings](../api/iteminsightssettings-get.md) | [itemInsightsSettings](iteminsightssettings.md) | Obter as propriedades de um objeto **itemInsightsSettings** . |
| [Atualizar itemInsightsSettings](../api/iteminsightssettings-update.md) | [itemInsightsSettings](iteminsightssettings.md) | Atualiza as propriedades do recurso **itemInsightsSettings** especificado. |

## <a name="properties"></a>Propriedades

Nenhum.

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id |String| ID do objeto de configurações da organização. |
|profileCardProperties|coleção [profileCardProperty](profilecardproperty.md)| Contém uma coleção de propriedades que um administrador definiu como visível no cartão de perfil do Microsoft 365. [Obter configurações da organização](../api/organizationsettings-get.md) retorna as propriedades configuradas para cartões de perfil para a organização.|
|itemInsights|[itemInsightsSettings](iteminsightssettings.md)| Contém as propriedades que são configuradas por um administrador para a visibilidade das ideias derivadas do Microsoft Graph, entre um usuário e outros itens no Microsoft 365, como documentos ou sites. [Obtenha itemInsightsSettings](../api/iteminsightssettings-get.md) por meio dessa propriedade de navegação.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.organizationSettings",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "profileCardProperties": [{"@odata.type": "microsoft.graph.profileCardProperty"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organizationSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


