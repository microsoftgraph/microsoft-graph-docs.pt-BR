---
title: Criar mobileThreatDefenseConnector
description: Cria um novo objeto mobileThreatDefenseConnector.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ba32a951f182ba7ba752410a3aac13b94da89850
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346015"
---
# <a name="create-mobilethreatdefenseconnector"></a>Criar mobileThreatDefenseConnector

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Cria um novo objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementServiceConfig.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto mobileThreatDefenseConnector.

A tabela a seguir mostra as propriedades obrigatórias ao criar mobileThreatDefenseConnector.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Ainda não documentado|
|lastHeartbeatDateTime|DateTimeOffset|Data e hora da última Pulsação recebida de um Parceiro de Sincronização de Dados|
|partnerState|[mobileThreatPartnerTenantState](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|Sincronização de Dados estado do parceiro para essa conta. Os valores possíveis são: `unavailable`, `available`, `enabled`, `unresponsive`.|
|androidMobileApplicationManagementEnabled|Booliano|Para Android, de definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações do Gerenciamento de Aplicativo Móvel (MAM). Somente um parceiro por plataforma pode estar habilitado para avaliação do Gerenciamento de Aplicativo Móvel (MAM).|
|iosMobileApplicationManagementEnabled|Booliano|Para IOS, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações do MAM (Gerenciamento de Aplicativo Móvel). Somente um parceiro por plataforma pode estar habilitado para avaliação do Gerenciamento de Aplicativo Móvel (MAM).|
|androidEnabled|Boolean|No Android, definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade|
|iosEnabled|Boolean|No iOS, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade|
|windowsEnabled|Boolean|Para Windows, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade|
|macEnabled|Boolean|Para Mac, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade|
|androidDeviceBlockedOnMissingPartnerData|Boolean|No Android, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível|
|iosDeviceBlockedOnMissingPartnerData|Boolean|No iOS, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível|
|windowsDeviceBlockedOnMissingPartnerData|Booliano|Para Windows, defina se o Intune deve receber dados do parceiro de sincronização de dados antes de marcar um dispositivo compatível|
|macDeviceBlockedOnMissingPartnerData|Booliano|Para Mac, obter ou definir se o Intune deve receber dados do parceiro de sincronização de dados antes de marcar um dispositivo compatível|
|partnerUnsupportedOsVersionBlocked|Boolean|Obter ou definir se dispositivos devem ser bloqueados nas plataformas habilitadas que não atendam aos requisitos mínimos de versão do Parceiro de Sincronização de Dados|
|partnerUnresponsivenessThresholdInDays|Int32|Obtém ou define dias de tolerância por locatário à falta de resposta para esta integração de parceiro|
|allowPartnerToCollectIOSApplicationMetadata|Boolean|Para dispositivos IOS, permite que o administrador configure se o parceiro de sincronização de dados também pode coletar metadados sobre aplicativos instalados do Intune|
|allowPartnerToCollectIOSPersonalApplicationMetadata|Boolean|Para dispositivos IOS, permite que o administrador configure se o parceiro de sincronização de dados também pode coletar metadados sobre aplicativos instalados pessoalmente do Intune|
|microsoftDefenderForEndpointAttachEnabled|Booliano|Quando VERDADEIRO, o gerenciamento de perfil de configuração por meio do Microsoft Defender para Ponto de Extremidade está habilitado. Quando FALSE, o gerenciamento de perfil de configuração por meio do Microsoft Defender for Endpoint é desabilitado.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors
Content-type: application/json
Content-length: 844

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
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
  "partnerUnresponsivenessThresholdInDays": 6,
  "allowPartnerToCollectIOSApplicationMetadata": true,
  "allowPartnerToCollectIOSPersonalApplicationMetadata": true,
  "microsoftDefenderForEndpointAttachEnabled": true
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 893

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "e4bede14-de14-e4be-14de-bee414debee4",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
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
  "partnerUnresponsivenessThresholdInDays": 6,
  "allowPartnerToCollectIOSApplicationMetadata": true,
  "allowPartnerToCollectIOSPersonalApplicationMetadata": true,
  "microsoftDefenderForEndpointAttachEnabled": true
}
```




