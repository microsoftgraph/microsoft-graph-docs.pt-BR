---
title: tipo de recurso onPremisesPublishingProfile
description: tipo de recurso onPremisesPublishingProfile.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4299ddec6a05e079d86a070b939c2220087281a0
ms.sourcegitcommit: 366178d3fc37439791061082da80a63fba2c27df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2020
ms.locfileid: "48921524"
---
# <a name="onpremisespublishingprofile-resource-type"></a>tipo de recurso onPremisesPublishingProfile

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Vários serviços do Azure (por exemplo, a autenticação de [passagem](/azure/active-directory/hybrid/how-to-connect-pta)do Azure Active Directory Connect, o [WORKDAY para o provisionamento de usuários do Azure ad](/azure/active-directory/saas-apps/workday-inbound-tutorial)e o [proxy de aplicativo](https://aka.ms/whyappproxy) permitem o acesso a vários recursos locais de fora da rede corporativa.

[Os agentes locais](onpremisesagent.md) (ou [conectores](connector.md) para o proxy de aplicativo) instalados por um administrador podem ser configurados para encaminhar solicitações a um determinado [recurso publicado](publishedresource.md).
[Grupos de agente](onpremisesagentgroup.md) (ou [grupos de conectores](connectorgroup.md) para o proxy de aplicativo) permitem que um administrador atribua agentes específicos para atender a recursos locais publicados específicos. Os administradores também podem agrupar vários agentes e, em seguida, atribuir cada recurso publicado a um grupo de agentes. Todo o conjunto de entidades do mesmo tipo de publicação local é representado pelo **onPremisesPublishingProfile**.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter onPremisesPublishingProfile](../api/onpremisespublishingprofile-get.md) | [onPremisesPublishingProfile](onpremisespublishingprofile.md) | Leia as propriedades e os relacionamentos de um objeto **onPremisesPublishingProfile** . |
| [Atualizar onPremisesPublishingProfile](../api/onpremisespublishingprofile-update.md) | Nenhum | Atualize um objeto [onPremisesPublishingProfile](onpremisespublishingprofile.md) . |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|hybridAgentUpdaterConfiguration|[hybridAgentUpdaterConfiguration](hybridagentupdaterconfiguration.md)| Representa um objeto **hybridAgentUpdaterConfiguration** .|
|id|String| Representa um tipo de publicação. Os valores possíveis são: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`. Somente leitura.|
|isEnabled|Booliano| Representa se o [proxy de aplicativo do Azure ad](https://aka.ms/whyappproxy) está habilitado para o locatário. |

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|agentGroups|coleção [onPremisesAgentGroup](onpremisesagentgroup.md)| Lista de objetos **onPremisesAgentGroup** existentes. Somente leitura. Anulável.|
|SNMP|coleção [onPremisesAgent](onpremisesagent.md)| Lista de objetos **onPremisesAgent** existentes. Somente leitura. Anulável.|
|connectorGroups|coleção de [conectores](connectorgroup.md)| Lista de objetos de **conector** existentes para aplicativos publicados por meio do proxy de aplicativo. Somente leitura. Anulável.|
|conectores|coleção [Connector](connector.md)| Lista de objetos **conectores** existentes para aplicativos publicados por meio do proxy de aplicativo. Somente leitura. Anulável.|
|publishedResources|coleção [publishedResource](publishedresource.md)| Lista de objetos **publishedResource** existentes. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "hybridAgentUpdaterConfiguration": {"@odata.type": "microsoft.graph.hybridAgentUpdaterConfiguration"},
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesPublishingProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


