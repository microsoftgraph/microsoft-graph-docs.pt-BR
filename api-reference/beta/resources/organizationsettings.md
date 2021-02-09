---
title: Tipo de recurso organizationSettings
description: Contém configurações que são aplicáveis à organização ou aos objetos do usuário dentro dela.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 105a57c7cb5827e9017df7494d32802ef7ac6fa5
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158321"
---
# <a name="organizationsettings-resource-type"></a>Tipo de recurso organizationSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém configurações que são aplicáveis à organização [ou](organization.md) que devem ser aplicadas a objetos [de](user.md) usuário dentro de uma organização.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter configurações da organização](../api/organizationsettings-get.md) | [organizationSettings](organizationsettings.md) | Leia o objeto de configurações da organização. |
| [Criar profileCardProperty](../api/organizationsettings-post-profilecardproperties.md) | [profileCardProperty](profilecardproperty.md) | Crie um novo **profileCardProperty** postando na coleção de objetos **profileCardProperty.** |
| [Listar profileCardProperties](../api/organizationsettings-list-profilecardproperties.md) | [Coleção profileCardProperty](profilecardproperty.md) | Obter uma **coleção de objetos profileCardProperty.** |
| [Obter itemInsightsSettings](../api/iteminsightssettings-get.md) | [itemInsightsSettings](iteminsightssettings.md) | Obter as propriedades de um **objeto itemInsightsSettings** . |
| [Atualizar itemInsightsSettings](../api/iteminsightssettings-update.md) | [itemInsightsSettings](iteminsightssettings.md) | Atualizar as propriedades do recurso **itemInsightsSettings** especificado. |

## <a name="properties"></a>Propriedades

Nenhum.

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id |String| ID do objeto de configurações da organização. |
|profileCardProperties|[Coleção profileCardProperty](profilecardproperty.md)| Contém uma coleção das propriedades que um administrador definiu como visíveis no cartão de perfil do Microsoft 365. [Obter as configurações da organização](../api/organizationsettings-get.md) retorna as propriedades configuradas para cartões de perfil da organização.|
|itemInsights|[itemInsightsSettings](iteminsightssettings.md)| Contém as propriedades configuradas por um administrador para a visibilidade das informações derivadas do Microsoft Graph, entre um usuário e outros itens no Microsoft 365, como documentos ou sites. [Obter itemInsightsSettings](../api/iteminsightssettings-get.md) por meio desta propriedade de navegação.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.organizationSettings",
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


