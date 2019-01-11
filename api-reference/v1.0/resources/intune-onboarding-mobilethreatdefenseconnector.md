---
title: Tipo de recurso mobileThreatDefenseConnector
description: Entidade que representa uma conexão com o parceiro de defesa contra ameaças móveis.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2469440ceff1dc6c301d6ed4cb6c9a4f341eed31
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834402"
---
# <a name="mobilethreatdefenseconnector-resource-type"></a>Tipo de recurso mobileThreatDefenseConnector

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Entidade que representa uma conexão com o parceiro de defesa contra ameaças móveis.
## <a name="methods"></a>Métodos
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
|id|Cadeia de caracteres|Ainda não documentado|
|lastHeartbeatDateTime|DateTimeOffset|Data e hora da última Pulsação recebida de um Parceiro de Sincronização de Dados|
|partnerState|[mobileThreatPartnerTenantState](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|Estado de parceiro de sincronização de dados para essa conta. Os valores possíveis são: `unavailable`, `available`, `enabled`, `unresponsive`.|
|androidEnabled|Boolean|No Android, definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade|
|iosEnabled|Boolean|No iOS, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade|
|androidDeviceBlockedOnMissingPartnerData|Boolean|No Android, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível|
|iosDeviceBlockedOnMissingPartnerData|Boolean|No iOS, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível|
|partnerUnsupportedOsVersionBlocked|Boolean|Obter ou definir se dispositivos devem ser bloqueados nas plataformas habilitadas que não atendam aos requisitos mínimos de versão do Parceiro de Sincronização de Dados|
|partnerUnresponsivenessThresholdInDays|Int32|Obtém ou define dias de tolerância por locatário à falta de resposta para esta integração de parceiro|

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
  "androidEnabled": true,
  "iosEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 1024
}
```



