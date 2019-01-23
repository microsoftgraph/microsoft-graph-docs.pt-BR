---
title: Atualizar mobileThreatDefenseConnector
description: Atualiza as propriedades de um objeto mobileThreatDefenseConnector.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c8ed44a29f3e56f602689b58e3f58071998cde21
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411208"
---
# <a name="update-mobilethreatdefenseconnector"></a>Atualizar mobileThreatDefenseConnector

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Atualiza as propriedades de um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementServiceConfig.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).

A tabela a seguir mostra as propriedades obrigatórias ao criar [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Ainda não documentado|
|lastHeartbeatDateTime|DateTimeOffset|Data e hora da última Pulsação recebida de um Parceiro de Sincronização de Dados|
|partnerState|[mobileThreatPartnerTenantState](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|Estado de parceiro de sincronização de dados para essa conta. Os valores possíveis são: `unavailable`, `available`, `enabled`, `unresponsive`.|
|androidEnabled|Boolean|No Android, definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade|
|iosEnabled|Boolean|No iOS, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade|
|windowsEnabled|Boolean|Para Windows, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante as avaliações de conformidade|
|macEnabled|Boolean|Para Mac, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante as avaliações de conformidade|
|androidDeviceBlockedOnMissingPartnerData|Boolean|No Android, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível|
|iosDeviceBlockedOnMissingPartnerData|Boolean|No iOS, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível|
|windowsDeviceBlockedOnMissingPartnerData|Boolean|Para Windows, defina se Intune deve receber dados do parceiro de sincronização de dados antes da marcação de um dispositivo compatível com|
|macDeviceBlockedOnMissingPartnerData|Boolean|Para Mac, obter ou definir se Intune deve receber dados do parceiro de sincronização de dados antes da marcação de um dispositivo compatível com|
|partnerUnsupportedOsVersionBlocked|Boolean|Obter ou definir se dispositivos devem ser bloqueados nas plataformas habilitadas que não atendam aos requisitos mínimos de versão do Parceiro de Sincronização de Dados|
|partnerUnresponsivenessThresholdInDays|Int32|Obtém ou define dias de tolerância por locatário à falta de resposta para esta integração de parceiro|
|allowPartnerToCollectIOSApplicationMetadata|Boolean|Para dispositivos IOS, permite que o administrador configurar se o parceiro de sincronização de dados também pode coletar metadados sobre os aplicativos instalados de Intune|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
Content-type: application/json
Content-length: 622

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
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
  "allowPartnerToCollectIOSApplicationMetadata": true
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 671

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "e4bede14-de14-e4be-14de-bee414debee4",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
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
  "allowPartnerToCollectIOSApplicationMetadata": true
}
```




