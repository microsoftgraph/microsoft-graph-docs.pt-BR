---
title: Tipo de recurso onPremisesPublishingProfile
description: Tipo de recurso onPremisesPublishingProfile.
ms.localizationpriority: medium
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 2d984b304b47005db4de02d920cacc37ba21fb3c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62125078"
---
# <a name="onpremisespublishingprofile-resource-type"></a>Tipo de recurso onPremisesPublishingProfile

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Vários serviços do Azure (por exemplo, Azure Active Directory Conexão autenticação passo [a](/azure/active-directory/hybrid/how-to-connect-pta)passo, dia de trabalho para o provisionamento de usuários do [Azure AD](/azure/active-directory/saas-apps/workday-inbound-tutorial)e [Proxy](/azure/active-directory/app-proxy/what-is-application-proxy) de Aplicativo permitem acesso a vários recursos locais de fora da rede corporativa.

Agentes locais (ou conectores para Proxy de Aplicativo) [instalados](connector.md) por um administrador podem ser [configurados](onpremisesagent.md) para rotear solicitações para um determinado [recurso publicado.](publishedresource.md)
[Grupos de agentes](onpremisesagentgroup.md) (ou [grupos de](connectorgroup.md) conectores para Proxy de Aplicativo) permitem que um administrador atribua agentes específicos para atender a recursos locais publicados específicos. Os administradores também podem agrupar vários agentes e atribuir cada recurso publicado a um grupo de agentes. Todo o conjunto de entidades do mesmo tipo de publicação local é representado por **onPremisesPublishingProfile**.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter onPremisesPublishingProfile](../api/onpremisespublishingprofile-get.md) | [onPremisesPublishingProfile](onpremisespublishingprofile.md) | Leia as propriedades e as relações de um **objeto onPremisesPublishingProfile.** |
| [Atualizar onPremisesPublishingProfile](../api/onpremisespublishingprofile-update.md) | Nenhum | Atualize [um objeto onPremisesPublishingProfile.](onpremisespublishingprofile.md) |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|hybridAgentUpdaterConfiguration|[hybridAgentUpdaterConfiguration](hybridagentupdaterconfiguration.md)| Representa um **objeto hybridAgentUpdaterConfiguration.**|
|id|Cadeia de caracteres| Representa um tipo de publicação. Os valores possíveis são: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`. Somente leitura.|
|isEnabled|Booliano| Representa se o Proxy de Aplicativo [do Azure AD](/azure/active-directory/app-proxy/what-is-application-proxy) está habilitado para o locatário. |

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|agentGroups|[Coleção onPremisesAgentGroup](onpremisesagentgroup.md)| Lista de objetos **onPremisesAgentGroup** existentes. Somente leitura. Anulável.|
|agentes|[Coleção onPremisesAgent](onpremisesagent.md)| Lista de objetos **onPremisesAgent** existentes. Somente leitura. Anulável.|
|connectorGroups|[Coleção connectorGroup](connectorgroup.md)| Lista de objetos **connectorGroup** existentes para aplicativos publicados por meio do Proxy de Aplicativo. Somente leitura. Anulável.|
|conectores|[coleção connector](connector.md)| Lista de objetos **conectores existentes** para aplicativos publicados por meio do Proxy de Aplicativo. Somente leitura. Anulável.|
|publishedResources|[coleção publishedResource](publishedresource.md)| Lista de objetos **publishedResource** existentes. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile",
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