---
title: Tipo de recurso microsoftTunnelServerLogCollectionResponse
description: Entidade que armazena o status do conjunto de log do servidor.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8b61d6fbec3dedbc61de8908dafc70ea7fea3497
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61341926"
---
# <a name="microsofttunnelserverlogcollectionresponse-resource-type"></a>Tipo de recurso microsoftTunnelServerLogCollectionResponse

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que armazena o status do conjunto de log do servidor.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar microsoftTunnelServerLogCollectionResponses](../api/intune-mstunnel-microsofttunnelserverlogcollectionresponse-list.md)|[coleção microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)|Listar propriedades e relações dos [objetos microsoftTunnelServerLogCollectionResponse.](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)|
|[Obter microsoftTunnelServerLogCollectionResponse](../api/intune-mstunnel-microsofttunnelserverlogcollectionresponse-get.md)|[microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)|Leia propriedades e relações do [objeto microsoftTunnelServerLogCollectionResponse.](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)|
|[Criar microsoftTunnelServerLogCollectionResponse](../api/intune-mstunnel-microsofttunnelserverlogcollectionresponse-create.md)|[microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)|Crie um novo [objeto microsoftTunnelServerLogCollectionResponse.](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)|
|[Excluir microsoftTunnelServerLogCollectionResponse](../api/intune-mstunnel-microsofttunnelserverlogcollectionresponse-delete.md)|Nenhum|Exclui um [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md).|
|[Atualizar microsoftTunnelServerLogCollectionResponse](../api/intune-mstunnel-microsofttunnelserverlogcollectionresponse-update.md)|[microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)|Atualize as propriedades de um [objeto microsoftTunnelServerLogCollectionResponse.](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)|
|[ação createDownloadUrl](../api/intune-mstunnel-microsofttunnelserverlogcollectionresponse-createdownloadurl.md)|String|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID exclusiva da entidade|
|status|[microsoftTunnelLogCollectionStatus](../resources/intune-mstunnel-microsofttunnellogcollectionstatus.md)|O status do conjunto de log. Os valores possíveis são: `pending`, `completed`, `failed`.|
|startDateTime|DateTimeOffset|A hora de início dos logs coletados |
|endDateTime|DateTimeOffset|A hora de término dos logs coletados|
|sizeInBytes|Int64|O tamanho dos logs em bytes|
|serverId|String|ID do servidor em que o conjunto de log é solicitado|
|requestDateTime|DateTimeOffset|A hora em que o conjunto de log foi solicitado|
|expiryDateTime|DateTimeOffset|O tempo em que o conjunto de log expira|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftTunnelServerLogCollectionResponse"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftTunnelServerLogCollectionResponse",
  "id": "String (identifier)",
  "status": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "sizeInBytes": 1024,
  "serverId": "String",
  "requestDateTime": "String (timestamp)",
  "expiryDateTime": "String (timestamp)"
}
```




