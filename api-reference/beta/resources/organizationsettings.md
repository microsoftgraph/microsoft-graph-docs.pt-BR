---
title: Tipo de recurso organizationSettings
description: Contém configurações aplicáveis à organização ou aos objetos do usuário dentro dela.
ms.localizationpriority: medium
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: dfaddb2a4297a1cf63dca360e099c64e99ec71d7
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64588425"
---
# <a name="organizationsettings-resource-type"></a>Tipo de recurso organizationSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém configurações aplicáveis à organização [ou](organization.md) que devem ser aplicadas a objetos [de](user.md) usuário em uma organização.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter configurações da organização](../api/organizationsettings-get.md) | [organizationSettings](organizationsettings.md) | Leia o objeto de configurações da organização. |
| [Criar profileCardProperty](../api/organizationsettings-post-profilecardproperties.md) | [profileCardProperty](profilecardproperty.md) | Crie um novo **profileCardProperty** postando na coleção **de objetos profileCardProperty** . |
| [Item de listaInsights](../api/organizationsettings-list-iteminsights.md) | [insightsSettings](insightssettings.md) | Obter as propriedades de um [objeto insightsSettings](insightssettings.md) para exibir ou retornar insights de item em uma organização. |
| [Listar microsoftApplicationDataAccessSettings](../api/organizationsettings-list-microsoftapplicationdataaccess.md) | [microsoftApplicationDataAccessSettings](microsoftapplicationdataaccesssettings.md) | Obter as propriedades de um [objeto microsoftApplicationDataAccessSettings](microsoftapplicationdataaccesssettings.md) que especificam o acesso de aplicativos Microsoft para Microsoft 365 dados do usuário em uma organização. |
| [Listar peopleInsights](../api/organizationsettings-list-peopleinsights.md) | [insightsSettings](insightssettings.md) | Obter as propriedades de um [objeto insightsSettings](insightssettings.md) para exibir ou retornar informações de pessoas em uma organização. |
| [Listar profileCardProperties](../api/organizationsettings-list-profilecardproperties.md) | [Coleção profileCardProperty](profilecardproperty.md) | Obter uma **coleção de objetos profileCardProperty** . |

## <a name="properties"></a>Propriedades

Nenhum.

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id |Cadeia de caracteres| ID do objeto settings da organização. |
|profileCardProperties|[Coleção profileCardProperty](profilecardproperty.md)| Contém uma coleção das propriedades que um administrador definiu como visíveis no Microsoft 365 de perfil. [Obter configurações da organização](../api/organizationsettings-get.md) retorna as propriedades configuradas para cartões de perfil para a organização.|
|itemInsights|[insightsSettings](insightssettings.md)| Contém as propriedades que são configuradas por um administrador para a visibilidade das informações derivadas do Microsoft Graph, entre um usuário e outros itens no Microsoft 365, como documentos ou sites. [Item de listaInsights](../api/organizationsettings-list-iteminsights.md) retorna _as configurações_ para exibir ou retornar informações de item em uma organização.|
|microsoftApplicationDataAccessSettings|[microsoftApplicationDataAccessSettings](../resources/microsoftapplicationdataaccesssettings.md)| Contém as propriedades configuradas por um administrador para especificar o acesso de aplicativos Microsoft Microsoft 365 dados pertencentes aos usuários em uma organização. [Listar microsoftApplicationDataAccessSettings](../api/organizationsettings-list-microsoftapplicationdataaccess.md) retorna as _configurações_ que especificam o acesso. |
|peopleInsights|[insightsSettings](insightssettings.md)| Contém as propriedades configuradas por um administrador para a visibilidade de uma lista de pessoas relevantes [](/graph/people-example#including-a-person-as-relevant-or-working-with) e trabalhando com um usuário no Microsoft 365. [Listar pessoasInsights](../api/organizationsettings-list-peopleinsights.md) retorna _as configurações_ para exibir ou retornar informações de pessoas em uma organização.|

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


