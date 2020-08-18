---
title: tipo de recurso deviceLogCollectionResponse
description: Entidade de solicitação de conjunto de logs do Windows.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4c3a7725f0f02c0ba2b8588c57179fa80316c595
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792972"
---
# <a name="devicelogcollectionresponse-resource-type"></a>tipo de recurso deviceLogCollectionResponse

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade de solicitação de conjunto de logs do Windows.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceLogCollectionResponses](../api/intune-devices-devicelogcollectionresponse-list.md)|coleção [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)|Listar Propriedades e relações dos objetos [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) .|
|[Obter deviceLogCollectionResponse](../api/intune-devices-devicelogcollectionresponse-get.md)|[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)|Leia as propriedades e as relações do objeto [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) .|
|[Criar deviceLogCollectionResponse](../api/intune-devices-devicelogcollectionresponse-create.md)|[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)|Criar um novo objeto [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) .|
|[Excluir deviceLogCollectionResponse](../api/intune-devices-devicelogcollectionresponse-delete.md)|Nenhum|Exclui [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md).|
|[Atualizar deviceLogCollectionResponse](../api/intune-devices-devicelogcollectionresponse-update.md)|[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)|Atualiza as propriedades de um objeto [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) .|
|[ação createDownloadUrl](../api/intune-devices-devicelogcollectionresponse-createdownloadurl.md)|String|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo no formato de tenantId_deviceId_requestId|
|status|String|O status da solicitação de coleção de logs|
|managedDeviceId|Guid|A ID do dispositivo|
|errorCode|Int64|O código de erro, se houver. Valores válidos-9.22337203685478 E + 18 para 9.22337203685478 E + 18|
|requestedDateTimeUTC|DateTimeOffset|O DateTime da solicitação|
|receivedDateTimeUTC|DateTimeOffset|O DateTime que a solicitação foi recebida|
|initiatedByUserPrincipalName|String|O UPN para quem iniciou a solicitação|
|expirationDateTimeUTC|DateTimeOffset|O DateTime do vencimento dos logs|
|size|Duplo|O tamanho dos logs. Valores válidos-1.79769313486232 E + 308 a 1.79769313486232 E + 308|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceLogCollectionResponse"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceLogCollectionResponse",
  "id": "String (identifier)",
  "status": "String",
  "managedDeviceId": "Guid",
  "errorCode": 1024,
  "requestedDateTimeUTC": "String (timestamp)",
  "receivedDateTimeUTC": "String (timestamp)",
  "initiatedByUserPrincipalName": "String",
  "expirationDateTimeUTC": "String (timestamp)",
  "size": "4.2"
}
```



