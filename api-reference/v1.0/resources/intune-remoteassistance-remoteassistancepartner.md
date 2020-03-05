---
title: Tipo de recurso remoteAssistancePartner
description: Recursos de remoteAssistPartner representam metadados e status de um determinado serviço de Parceiro de assistência remota.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 82b4696b29c76ac5c9d2a579135a1c38e2e8f44a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447903"
---
# <a name="remoteassistancepartner-resource-type"></a>Tipo de recurso remoteAssistancePartner

Namespace: Microsoft. Graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Recursos de remoteAssistPartner representam metadados e status de um determinado serviço de Parceiro de assistência remota.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar remoteAssistancePartners](../api/intune-remoteassistance-remoteassistancepartner-list.md)|Conjunto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Listar propriedades e relações de objetos de [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Obter remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Ler propriedades e relações de objetos de [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Criar remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Criar um novo objeto de [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Excluir remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|Nenhum|Excluir [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Atualizar remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Atualizar as propriedades de um objeto de [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Ação beginOnboarding](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|Nenhuma|Ainda não documentado|
|[ação de desconectar](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|Nenhuma|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do parceiro.|
|displayName|Cadeia de caracteres|Nome de exibição do parceiro.|
|onboardingUrl|Cadeia de caracteres|URL do portal de integração do parceiro, no qual um administrador pode configurar o serviço de assistência remota.|
|onboardingStatus|[remoteAssistanceOnboardingStatus](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|TBD. Os valores possíveis são: `notOnboarded`, `onboarding`, `onboarded`.|
|lastConnectionDateTime|DateTimeOffset|Carimbo de data/hora da última solicitação enviada ao Intune pelo parceiro TEM.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteAssistancePartner"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "String (identifier)",
  "displayName": "String",
  "onboardingUrl": "String",
  "onboardingStatus": "String",
  "lastConnectionDateTime": "String (timestamp)"
}
```




