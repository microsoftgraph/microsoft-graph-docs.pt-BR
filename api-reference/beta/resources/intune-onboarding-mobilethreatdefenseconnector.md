---
title: Tipo de recurso mobileThreatDefenseConnector
description: Entidade que representa uma conexão com o parceiro de defesa contra ameaças móveis.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 338366d99bf17cad44b63bfee7ad3fb13709ddf0
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61348184"
---
# <a name="mobilethreatdefenseconnector-resource-type"></a>Tipo de recurso mobileThreatDefenseConnector

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa uma conexão com o parceiro de defesa contra ameaças móveis.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar mobileThreatDefenseConnectors](../api/intune-onboarding-mobilethreatdefenseconnector-list.md)|Coleção [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)|Lista propriedades e relações dos objetos [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).|
|[Obter mobileThreatDefenseConnector](../api/intune-onboarding-mobilethreatdefenseconnector-get.md)|[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)|Propriedades de leitura e relações do objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).|
|[Criar mobileThreatDefenseConnector](../api/intune-onboarding-mobilethreatdefenseconnector-create.md)|[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)|Cria um novo objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).|
|[Excluir mobileThreatDefenseConnector](../api/intune-onboarding-mobilethreatdefenseconnector-delete.md)|Nenhuma|Exclui um [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).|
|[Atualizar mobileThreatDefenseConnector](../api/intune-onboarding-mobilethreatdefenseconnector-update.md)|[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)|Atualiza as propriedades de um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Ainda não documentado|
|lastHeartbeatDateTime|DateTimeOffset|Data e hora da última Pulsação recebida de um Parceiro de Sincronização de Dados|
|partnerState|[mobileThreatPartnerTenantState](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|Sincronização de Dados estado do parceiro para essa conta. Os valores possíveis são: `unavailable`, `available`, `enabled`, `unresponsive`.|
|androidMobileApplicationManagementEnabled|Booliano|Para Android, de definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações do Gerenciamento de Aplicativo Móvel (MAM). Somente um parceiro por plataforma pode estar habilitado para avaliação do Gerenciamento de Aplicativo Móvel (MAM).|
|iosMobileApplicationManagementEnabled|Boolean|Para IOS, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações do MAM (Gerenciamento de Aplicativo Móvel). Somente um parceiro por plataforma pode estar habilitado para avaliação do Gerenciamento de Aplicativo Móvel (MAM).|
|androidEnabled|Boolean|No Android, definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade|
|iosEnabled|Boolean|No iOS, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade|
|windowsEnabled|Booliano|Para Windows, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade|
|macEnabled|Booliano|Para Mac, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade|
|androidDeviceBlockedOnMissingPartnerData|Boolean|No Android, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível|
|iosDeviceBlockedOnMissingPartnerData|Boolean|No iOS, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível|
|windowsDeviceBlockedOnMissingPartnerData|Boolean|Para Windows, defina se o Intune deve receber dados do parceiro de sincronização de dados antes de marcar um dispositivo compatível|
|macDeviceBlockedOnMissingPartnerData|Booliano|Para Mac, obter ou definir se o Intune deve receber dados do parceiro de sincronização de dados antes de marcar um dispositivo compatível|
|partnerUnsupportedOsVersionBlocked|Boolean|Obter ou definir se dispositivos devem ser bloqueados nas plataformas habilitadas que não atendam aos requisitos mínimos de versão do Parceiro de Sincronização de Dados|
|partnerUnresponsivenessThresholdInDays|Int32|Obtém ou define dias de tolerância por locatário à falta de resposta para esta integração de parceiro|
|allowPartnerToCollectIOSApplicationMetadata|Boolean|Para dispositivos IOS, permite que o administrador configure se o parceiro de sincronização de dados também pode coletar metadados sobre aplicativos instalados do Intune|
|allowPartnerToCollectIOSPersonalApplicationMetadata|Boolean|Para dispositivos IOS, permite que o administrador configure se o parceiro de sincronização de dados também pode coletar metadados sobre aplicativos instalados pessoalmente do Intune|
|microsoftDefenderForEndpointAttachEnabled|Booliano|Quando VERDADEIRO, o gerenciamento de perfil de configuração por meio do Microsoft Defender para Ponto de Extremidade está habilitado. Quando FALSE, o gerenciamento de perfil de configuração por meio do Microsoft Defender for Endpoint é desabilitado.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileThreatDefenseConnector"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "String (identifier)",
  "lastHeartbeatDateTime": "String (timestamp)",
  "partnerState": "String",
  "androidMobileApplicationManagementEnabled": true,
  "iosMobileApplicationManagementEnabled": true,
  "androidEnabled": true,
  "iosEnabled": true,
  "windowsEnabled": true,
  "macEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "windowsDeviceBlockedOnMissingPartnerData": true,
  "macDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 1024,
  "allowPartnerToCollectIOSApplicationMetadata": true,
  "allowPartnerToCollectIOSPersonalApplicationMetadata": true,
  "microsoftDefenderForEndpointAttachEnabled": true
}
```




