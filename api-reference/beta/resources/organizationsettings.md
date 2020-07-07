---
title: tipo de recurso organizationSettings
description: Contém configurações que se aplicam à organização ou aos objetos de usuário dentro dela.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 80b7272915cd6f9dbfc381aa93a32896e2eaf3f5
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050985"
---
# <a name="organizationsettings-resource-type"></a>tipo de recurso organizationSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém configurações que se aplicam à [organização](organization.md) ou que devem ser aplicadas a objetos de [usuário](user.md) em uma organização.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter configurações da organização](../api/organizationsettings-get.md) | [organizationSettings](organizationsettings.md) | Leia o objeto de configurações da organização. |
| [Criar profileCardProperty](../api/organizationsettings-post-profilecardproperties.md) | [profileCardProperty](profilecardproperty.md) | Crie um novo profileCardProperty postando na coleção profileCardProperties. |
| [Listar profileCardProperties](../api/organizationsettings-list-profilecardproperties.md) | coleção [profileCardProperty](profilecardproperty.md) | Obtenha uma coleção de objetos profileCardProperty. |

## <a name="properties"></a>Propriedades

Nenhum.

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id |String| ID do objeto de configurações da organização. |
|profileCardProperties|coleção [profileCardProperty](profilecardproperty.md)| Contém uma coleção das propriedades que um administrador definiu como visível no cartão de perfil do M365. |

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
