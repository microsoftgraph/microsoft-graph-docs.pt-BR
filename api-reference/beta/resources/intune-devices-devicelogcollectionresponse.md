---
title: Tipo de recurso deviceLogCollectionResponse
description: Windows Entidade de solicitação do Conjunto de Log.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5727156187200a35d3d1d1ddfc8c30fb942f620e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091339"
---
# <a name="devicelogcollectionresponse-resource-type"></a>Tipo de recurso deviceLogCollectionResponse

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Windows Entidade de solicitação do Conjunto de Log.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceLogCollectionResponses](../api/intune-devices-devicelogcollectionresponse-list.md)|[Coleção deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)|Listar propriedades e relações dos [objetos deviceLogCollectionResponse.](../resources/intune-devices-devicelogcollectionresponse.md)|
|[Obter deviceLogCollectionResponse](../api/intune-devices-devicelogcollectionresponse-get.md)|[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)|Leia propriedades e relações do [objeto deviceLogCollectionResponse.](../resources/intune-devices-devicelogcollectionresponse.md)|
|[Criar deviceLogCollectionResponse](../api/intune-devices-devicelogcollectionresponse-create.md)|[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)|Crie um novo [objeto deviceLogCollectionResponse.](../resources/intune-devices-devicelogcollectionresponse.md)|
|[Excluir deviceLogCollectionResponse](../api/intune-devices-devicelogcollectionresponse-delete.md)|Nenhum|Exclui um [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md).|
|[Atualizar deviceLogCollectionResponse](../api/intune-devices-devicelogcollectionresponse-update.md)|[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)|Atualize as propriedades de um [objeto deviceLogCollectionResponse.](../resources/intune-devices-devicelogcollectionresponse.md)|
|[ação createDownloadUrl](../api/intune-devices-devicelogcollectionresponse-createdownloadurl.md)|String|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo na forma de tenantId_deviceId_requestId|
|status|Cadeia de caracteres|O status da solicitação do conjunto de log|
|managedDeviceId|Guid|A ID do dispositivo|
|errorCode|Int64|O código de erro, se for o caso. Valores válidos -9.22337203685478E+18 a 9.22337203685478E+18|
|requestedDateTimeUTC|DateTimeOffset|DateTime da solicitação|
|receivedDateTimeUTC|DateTimeOffset|DateTime a solicitação foi recebida|
|initiatedByUserPrincipalName|Cadeia de Caracteres|O UPN para quem iniciou a solicitação|
|expirationDateTimeUTC|DateTimeOffset|DateTime da expiração dos logs|
|size|Duplo|O tamanho dos logs. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|

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



