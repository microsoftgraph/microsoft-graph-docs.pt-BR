---
title: tipo de recurso de mobileAppTroubleshootingEvent
description: Descreve o recurso de mobileAppTroubleshootingEvent da Microsoft Graph API para Intune, que oferece suporte a vários fluxos de trabalho.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bb519309f68f732a28ed8f26235f01f37d9628b9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429219"
---
# <a name="mobileapptroubleshootingevent-resource-type"></a>tipo de recurso de mobileAppTroubleshootingEvent

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Evento que representa um aplicativo de usuários de dispositivos instale o status de fluxos de trabalho de evento de solução de problemas e gerenciamento de dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista mobileAppTroubleshootingEvents](../api/intune-shared-mobileapptroubleshootingevent-list.md)|coleção [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)|Lista as propriedades e os relacionamentos dos objetos [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) .|
|[Obter mobileAppTroubleshootingEvent](../api/intune-shared-mobileapptroubleshootingevent-get.md)|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)|Leia as propriedades e os relacionamentos do objeto [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) .|
|[Criar mobileAppTroubleshootingEvent](../api/intune-shared-mobileapptroubleshootingevent-create.md)|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)|Crie um novo objeto de [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) .|
|[Excluir mobileAppTroubleshootingEvent](../api/intune-shared-mobileapptroubleshootingevent-delete.md)|Nenhum|Exclui um [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).|
|[Atualizar mobileAppTroubleshootingEvent](../api/intune-shared-mobileapptroubleshootingevent-update.md)|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)|Atualize as propriedades de um objeto [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|UUID para o objeto.|
|**Solução de problemas**|
|informações adicionais|Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Um conjunto de chave de cadeia de caracteres e pares de valor de cadeia de caracteres que fornece informações adicionais sobre o evento de solução de problemas Inherited de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|
|ApplicationId|Cadeia de caracteres|Identificador de aplicativo Intune.|
|correlationId|Cadeia de caracteres|ID usado para a falha no serviço de rastreamento. |
|eventDateTime|DateTimeOffset|A hora em que o evento ocorreu. |
|eventName|String|Nome do evento correspondente ao evento de solução de problemas. Opcional|
|histórico|coleção [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)|Aplicativo móvel Intune Item do histórico de solução de problemas|
|managedDeviceIdentifier|Cadeia de caracteres|Identificador de dispositivo criado ou coletado pelo Intune.|
|troubleshootingErrorDetails|[deviceManagementTroubleshootingErrorDetails](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|Objeto que contém informações detalhadas sobre o erro e suas atualizações. Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|
|userId|Cadeia de caracteres|Identificador do usuário que tentou registrar o dispositivo.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|**Gerenciamento de dispositivos**|
|appLogCollectionRequests|coleção [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|A propriedade do conjunto de AppLogUploadRequest.|


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "String (identifier)",
  "eventDateTime": "String (timestamp)",
  "correlationId": "String",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "String",
    "failure": "String",
    "failureDetails": "String",
    "remediation": "String",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "String",
        "link": "String"
      }
    ]
  },
  "eventName": "String",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "managedDeviceIdentifier": "String",
  "userId": "String",
  "applicationId": "String",
  "history": [
    {
      "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem",
      "occurrenceDateTime": "String (timestamp)"
    }
  ]
}
```




