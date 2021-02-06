---
title: Tipo de recurso onPremisesPublishingProfile
description: Tipo de recurso onPremisesPublishingProfile.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 8e74374baa397c292d323dc0520833a7318cbe79
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134894"
---
# <a name="onpremisespublishingprofile-resource-type"></a>Tipo de recurso onPremisesPublishingProfile

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Vários serviços do Azure (por exemplo, a Autenticação de Passagem do Azure Active Directory [Connect,](/azure/active-directory/hybrid/how-to-connect-pta)o dia de trabalho para o provisionamento de usuários do [Azure AD](/azure/active-directory/saas-apps/workday-inbound-tutorial)e o [Proxy](https://aka.ms/whyappproxy) de aplicativo permitem acesso a vários recursos locais de fora da rede corporativa.

[Agentes locais (ou](onpremisesagent.md) conectores para Proxy de Aplicativo) instalados por um administrador podem ser [configurados](connector.md) para encaminhar solicitações para um recurso [publicado específico.](publishedresource.md)
[Grupos de agentes](onpremisesagentgroup.md) (ou [grupos de conectores](connectorgroup.md) para Proxy de Aplicativo) permitem que um administrador atribua agentes específicos para atender a recursos locais publicados específicos. Os administradores também podem agrupar vários agentes e atribuir cada recurso publicado a um grupo de agentes. Todo o conjunto de entidades do mesmo tipo de publicação local é representado por **onPremisesPublishingProfile**.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter onPremisesPublishingProfile](../api/onpremisespublishingprofile-get.md) | [onPremisesPublishingProfile](onpremisespublishingprofile.md) | Leia as propriedades e os relacionamentos de um **objeto onPremisesPublishingProfile.** |
| [Atualizar onPremisesPublishingProfile](../api/onpremisespublishingprofile-update.md) | Nenhuma | Atualize [um objeto onPremisesPublishingProfile.](onpremisespublishingprofile.md) |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|hybridAgentUpdaterConfiguration|[hybridAgentUpdaterConfiguration](hybridagentupdaterconfiguration.md)| Representa um **objeto hybridAgentUpdaterConfiguration.**|
|id|String| Representa um tipo de publicação. Os valores possíveis são: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`. Somente leitura.|
|isEnabled|Booliano| Representa se o [Proxy de Aplicativo do Azure AD](https://aka.ms/whyappproxy) está habilitado para o locatário. |

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|agentGroups|[Coleção onPremisesAgentGroup](onpremisesagentgroup.md)| Lista de objetos **onPremisesAgentGroup** existentes. Somente leitura. Anulável.|
|agentes|[Coleção onPremisesAgent](onpremisesagent.md)| Lista de objetos **onPremisesAgent** existentes. Somente leitura. Anulável.|
|connectorGroups|[Coleção connectorGroup](connectorgroup.md)| Lista de objetos **connectorGroup existentes** para aplicativos publicados por meio do Proxy de Aplicativo. Somente leitura. Anulável.|
|conectores|[conjunto de conectores](connector.md)| Lista de objetos de **conector existentes** para aplicativos publicados por meio do Proxy de Aplicativo. Somente leitura. Anulável.|
|publishedResources|[Coleção publishedResource](publishedresource.md)| Lista de objetos **publishedResource** existentes. Somente leitura. Anulável.|

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



