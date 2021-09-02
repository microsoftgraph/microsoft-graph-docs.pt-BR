---
title: Tipo de recurso microsoftTunnelServer
description: Entidade que representa um único Microsoft Tunnel servidor
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2e20964b09e613c02c0e2483d10aece0439b765a
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58783194"
---
# <a name="microsofttunnelserver-resource-type"></a>Tipo de recurso microsoftTunnelServer

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa um único Microsoft Tunnel servidor

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar microsoftTunnelServers](../api/intune-mstunnel-microsofttunnelserver-list.md)|[Coleção microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)|Listar propriedades e relações dos [objetos microsoftTunnelServer.](../resources/intune-mstunnel-microsofttunnelserver.md)|
|[Obter microsoftTunnelServer](../api/intune-mstunnel-microsofttunnelserver-get.md)|[microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)|Leia propriedades e relações do [objeto microsoftTunnelServer.](../resources/intune-mstunnel-microsofttunnelserver.md)|
|[Criar microsoftTunnelServer](../api/intune-mstunnel-microsofttunnelserver-create.md)|[microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)|Crie um novo [objeto microsoftTunnelServer.](../resources/intune-mstunnel-microsofttunnelserver.md)|
|[Excluir microsoftTunnelServer](../api/intune-mstunnel-microsofttunnelserver-delete.md)|Nenhum(a)|Exclui um [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md).|
|[Atualizar o microsoftTunnelServer](../api/intune-mstunnel-microsofttunnelserver-update.md)|[microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)|Atualize as propriedades de um [objeto microsoftTunnelServer.](../resources/intune-mstunnel-microsofttunnelserver.md)|
|[Ação getHealthMetrics](../api/intune-mstunnel-microsofttunnelserver-gethealthmetrics.md)|[Coleção keyLongValuePair](../resources/intune-shared-keylongvaluepair.md)|Ainda não documentado|
|[Ação getHealthMetricTimeSeries](../api/intune-mstunnel-microsofttunnelserver-gethealthmetrictimeseries.md)|[Coleção metricTimeSeriesDataPoint](../resources/intune-mstunnel-metrictimeseriesdatapoint.md)|Ainda não documentado|
|[Ação createServerLogCollectionRequest](../api/intune-mstunnel-microsofttunnelserver-createserverlogcollectionrequest.md)|[microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Id do MicrosoftTunnelServer|
|displayName|Cadeia de caracteres|O nome de exibição do MicrosoftTunnelServer|
|tunnelServerHealthStatus|[microsoftTunnelServerHealthStatus](../resources/intune-mstunnel-microsofttunnelserverhealthstatus.md)|O status de saúde do MicrosoftTunnelServer. Os valores possíveis são: `unknown`, `healthy`, `unhealthy`, `warning`, `offline`, `upgradeInProgress`, `upgradeFailed`.|
|lastCheckinDateTime|DateTimeOffset|Quando o MicrosoftTunnelServer entrou pela última vez|
|agentImageDigest|Cadeia de caracteres|O resumo da imagem do agente atual em execução neste servidor |
|serverImageDigest|Cadeia de caracteres|O resumo da imagem atual do servidor em execução neste servidor |

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



