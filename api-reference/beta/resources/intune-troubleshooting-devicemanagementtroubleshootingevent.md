---
title: Tipo de recurso deviceManagementTroubleshootingEvent
description: Evento que representa uma falha geral.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ad5513f6872297f792ea19b913ae32089004e251
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59057296"
---
# <a name="devicemanagementtroubleshootingevent-resource-type"></a>Tipo de recurso deviceManagementTroubleshootingEvent

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Evento que representa uma falha geral.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementTroubleshootingEvents](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-list.md)|Conjunto [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|Listar propriedades e relações de objetos de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).|
|[Obter deviceManagementTroubleshootingEvent](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-get.md)|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|Ler propriedades e relações de objetos de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).|
|[Criar deviceManagementTroubleshootingEvent](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-create.md)|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|Criar um novo objeto de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).|
|[Excluir deviceManagementTroubleshootingEvent](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-delete.md)|Nenhum|Excluir [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).|
|[Atualizar deviceManagementTroubleshootingEvent](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-update.md)|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|Atualizar as propriedades de um objeto de [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O UUID do objeto.|
|eventDateTime|DateTimeOffset|A hora em que o evento ocorreu.|
|correlationId|Cadeia de caracteres|ID usada para rastrear a falha no serviço.|
|troubleshootingErrorDetails|[deviceManagementTroubleshootingErrorDetails](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|Objeto contendo informações detalhadas sobre o erro e sua correção.|
|eventName|Cadeia de Caracteres|Nome do Evento correspondente ao Evento de Solução de Problemas. É um campo Opcional|
|additionalInformation|Coleção [keyValuePair](../resources/intune-troubleshooting-keyvaluepair.md)|Um conjunto de pares de valores de chave de cadeia de caracteres e cadeia de caracteres que fornece informações adicionais sobre o evento Solução de problemas|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
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
  ]
}
```




