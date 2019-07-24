---
title: tipo de recurso onPremisesPublishingProfile
description: tipo de recurso onPremisesPublishingProfile.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1eb442b6f3317ac7c0e2f130442e4a62c7f9c152
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841322"
---
# <a name="onpremisespublishingprofile-resource-type"></a>tipo de recurso onPremisesPublishingProfile

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Vários serviços do Azure (por exemplo, Azue Active Directory Connect PassThrough Authentication, workday to Azure AD Users Provisioning) permitem um acesso condicional a vários recursos locais de fora da rede corporativa. [Os agentes locais](onpremisesagent.md) instalados por um administrador de locatários podem ser configurados para acessar/lidar com solicitações de um [recurso publicado](publishedresource.md)específico.
Os [grupos de agentes](onpremisesagentgroup.md) permitem que um administrador de locatários atribua agentes específicos para atender recursos locais publicados específicos. Os administradores de locatários podem agrupar vários agentes e, em seguida, atribuir cada recurso publicado a um grupo. Todo o conjunto de entidades do mesmo tipo de publicação local é representado pelo **onPremisesPublishingProfile**.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter onPremisesPublishingProfile](../api/onpremisespublishingprofile-get.md) | [onPremisesPublishingProfile](onpremisespublishingprofile.md) | Leia as propriedades e os relacionamentos de um objeto **onPremisesPublishingProfile** . |
| [Atualizar onPremisesPublishingProfile](../api/onpremisespublishingprofile-update.md) | Nenhum | Atualize um objeto [onPremisesPublishingProfile](onpremisespublishingprofile.md) .

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|hybridAgentUpdaterConfiguration|[hybridAgentUpdaterConfiguration](hybridagentupdaterconfiguration.md)| Representa um objeto **hybridAgentUpdaterConfiguration** .|
|id|String| Representa um tipo de publicação. Os valores possíveis são: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`. Somente leitura.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|agentGroups|coleção [onPremisesAgentGroup](onpremisesagentgroup.md)| Lista de objetos **onPremisesAgentGroup** existentes. Somente leitura. Anulável.|
|SNMP|coleção [onPremisesAgent](onpremisesagent.md)| Lista de objetos **onPremisesAgent** existentes. Somente leitura. Anulável.|
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
