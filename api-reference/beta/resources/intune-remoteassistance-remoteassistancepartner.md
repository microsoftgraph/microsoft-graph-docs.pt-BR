---
title: Tipo de recurso remoteAssistancePartner
description: Recursos de remoteAssistPartner representam metadados e status de um determinado serviço de Parceiro de assistência remota.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b0bdbffc33358770b43ac67dcb67d9acea7655f0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407932"
---
# <a name="remoteassistancepartner-resource-type"></a>Tipo de recurso remoteAssistancePartner

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Recursos de remoteAssistPartner representam metadados e status de um determinado serviço de Parceiro de assistência remota.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar remoteAssistancePartners](../api/intune-remoteassistance-remoteassistancepartner-list.md)|Conjunto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Listar propriedades e relações de objetos de [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Obter remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Ler propriedades e relações de objetos de [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Criar remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Criar um novo objeto de [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Excluir remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|Nenhum|Excluir [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Atualizar remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Atualizar as propriedades de um objeto de [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Ação beginOnboarding](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|Nenhum|Ainda não documentado|
|[ação de desconectar](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|Nenhum|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do parceiro.|
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




