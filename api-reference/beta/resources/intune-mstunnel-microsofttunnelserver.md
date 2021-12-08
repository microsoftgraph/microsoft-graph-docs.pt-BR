---
title: Tipo de recurso microsoftTunnelServer
description: Entidade que representa um único Microsoft Tunnel servidor
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 507c3d7af22614b96235853e0f5e0351adaf1198
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61336129"
---
# <a name="microsofttunnelserver-resource-type"></a>Tipo de recurso microsoftTunnelServer

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa um único Microsoft Tunnel servidor

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar microsoftTunnelServers](../api/intune-mstunnel-microsofttunnelserver-list.md)|[Coleção microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)|Listar propriedades e relações dos [objetos microsoftTunnelServer.](../resources/intune-mstunnel-microsofttunnelserver.md)|
|[Obter microsoftTunnelServer](../api/intune-mstunnel-microsofttunnelserver-get.md)|[microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)|Leia propriedades e relações do [objeto microsoftTunnelServer.](../resources/intune-mstunnel-microsofttunnelserver.md)|
|[Criar microsoftTunnelServer](../api/intune-mstunnel-microsofttunnelserver-create.md)|[microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)|Crie um novo [objeto microsoftTunnelServer.](../resources/intune-mstunnel-microsofttunnelserver.md)|
|[Excluir microsoftTunnelServer](../api/intune-mstunnel-microsofttunnelserver-delete.md)|Nenhum|Exclui um [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md).|
|[Atualizar o microsoftTunnelServer](../api/intune-mstunnel-microsofttunnelserver-update.md)|[microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)|Atualize as propriedades de um [objeto microsoftTunnelServer.](../resources/intune-mstunnel-microsofttunnelserver.md)|
|[Ação getHealthMetrics](../api/intune-mstunnel-microsofttunnelserver-gethealthmetrics.md)|[Coleção keyLongValuePair](../resources/intune-shared-keylongvaluepair.md)|Ainda não documentado|
|[Ação getHealthMetricTimeSeries](../api/intune-mstunnel-microsofttunnelserver-gethealthmetrictimeseries.md)|[Coleção metricTimeSeriesDataPoint](../resources/intune-mstunnel-metrictimeseriesdatapoint.md)|Ainda não documentado|
|[Ação createServerLogCollectionRequest](../api/intune-mstunnel-microsofttunnelserver-createserverlogcollectionrequest.md)|[microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Id do MicrosoftTunnelServer|
|displayName|String|O nome de exibição do MicrosoftTunnelServer|
|tunnelServerHealthStatus|[microsoftTunnelServerHealthStatus](../resources/intune-mstunnel-microsofttunnelserverhealthstatus.md)|O status de saúde do MicrosoftTunnelServer. Os valores possíveis são: `unknown`, `healthy`, `unhealthy`, `warning`, `offline`, `upgradeInProgress`, `upgradeFailed`.|
|lastCheckinDateTime|DateTimeOffset|Quando o MicrosoftTunnelServer entrou pela última vez|
|agentImageDigest|String|O resumo da imagem do agente atual em execução neste servidor |
|serverImageDigest|String|O resumo da imagem atual do servidor em execução neste servidor |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftTunnelServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftTunnelServer",
  "id": "String (identifier)",
  "displayName": "String",
  "tunnelServerHealthStatus": "String",
  "lastCheckinDateTime": "String (timestamp)",
  "agentImageDigest": "String",
  "serverImageDigest": "String"
}
```




