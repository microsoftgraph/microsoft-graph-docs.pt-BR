---
title: Tipo de recurso mobileAppTroubleshootingEvent
description: Descreve o recurso mobileAppTroubleshootingEvent da API do Microsoft Graph para o Intune, que oferece suporte a vários fluxos de trabalho.
ms.localizationpriority: medium
author: rolyon
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c4c522e6b6adf2a6a41c5e1a6a9e5b63fd64b9b0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59020263"
---
# <a name="mobileapptroubleshootingevent-resource-type"></a>Tipo de recurso mobileAppTroubleshootingEvent

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Evento representando um status de instalação de aplicativo de dispositivo de usuários para gerenciamento de dispositivos e solução de problemas de fluxos de trabalho de eventos.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar mobileAppTroubleshootingEvents](../api/intune-shared-mobileapptroubleshootingevent-list.md)|[Coleção mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)|Listar propriedades e relações dos [objetos mobileAppTroubleshootingEvent.](../resources/intune-shared-mobileapptroubleshootingevent.md)|
|[Obter mobileAppTroubleshootingEvent](../api/intune-shared-mobileapptroubleshootingevent-get.md)|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)|Leia propriedades e relações do [objeto mobileAppTroubleshootingEvent.](../resources/intune-shared-mobileapptroubleshootingevent.md)|
|[Criar mobileAppTroubleshootingEvent](../api/intune-shared-mobileapptroubleshootingevent-create.md)|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)|Crie um novo [objeto mobileAppTroubleshootingEvent.](../resources/intune-shared-mobileapptroubleshootingevent.md)|
|[Excluir mobileAppTroubleshootingEvent](../api/intune-shared-mobileapptroubleshootingevent-delete.md)|Nenhum|Exclui um [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).|
|[Atualizar mobileAppTroubleshootingEvent](../api/intune-shared-mobileapptroubleshootingevent-update.md)|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)|Atualize as propriedades de [um objeto mobileAppTroubleshootingEvent.](../resources/intune-shared-mobileapptroubleshootingevent.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|UUID para o objeto.|
|**Solução de Problemas**|
|additionalInformation|Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Um conjunto de pares de valores de chave de cadeia de caracteres e cadeia de caracteres que fornece informações adicionais sobre o evento Troubleshooting Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|
|ApplicationId|Cadeia de caracteres|Identificador de aplicativo do Intune.|
|correlationId|Cadeia de caracteres|ID usada para rastrear a falha no serviço. |
|eventDateTime|DateTimeOffset|A hora em que o evento ocorreu. |
|eventName|Cadeia de Caracteres|Nome do Evento correspondente ao Evento de Solução de Problemas. Opcional|
|history|[coleção mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)|Item histórico de solução de problemas de aplicativo móvel do Intune|
|managedDeviceIdentifier|Cadeia de caracteres|Identificador de dispositivo criado ou coletado pelo Intune.|
|troubleshootingErrorDetails|[deviceManagementTroubleshootingErrorDetails](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|Objeto contendo informações detalhadas sobre o erro e sua correção. Herdado de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|
|userId|Cadeia de caracteres|Identificador do usuário que tentou registrar o dispositivo.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|**Gerenciamento de dispositivo**|
|appLogCollectionRequests|[Coleção appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|A propriedade collection de AppLogUploadRequest.|


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




