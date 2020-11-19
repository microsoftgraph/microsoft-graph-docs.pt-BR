---
title: tipo de recurso microsoftTunnelServer
description: Entidade que representa um único servidor de encapsulamento da Microsoft
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ed9968e5f1d0f4c530d09d0ff8950ad6864b90c2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301414"
---
# <a name="microsofttunnelserver-resource-type"></a>tipo de recurso microsoftTunnelServer

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa um único servidor de encapsulamento da Microsoft

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar microsoftTunnelServers](../api/intune-mstunnel-microsofttunnelserver-list.md)|coleção [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)|Listar Propriedades e relações dos objetos [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) .|
|[Obter microsoftTunnelServer](../api/intune-mstunnel-microsofttunnelserver-get.md)|[microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)|Leia as propriedades e as relações do objeto [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) .|
|[Criar microsoftTunnelServer](../api/intune-mstunnel-microsofttunnelserver-create.md)|[microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)|Criar um novo objeto [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) .|
|[Excluir microsoftTunnelServer](../api/intune-mstunnel-microsofttunnelserver-delete.md)|Nenhum|Exclui [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md).|
|[Atualizar microsoftTunnelServer](../api/intune-mstunnel-microsofttunnelserver-update.md)|[microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)|Atualiza as propriedades de um objeto [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID do MicrosoftTunnelServer|
|displayName|String|O nome de exibição do MicrosoftTunnelServer|
|tunnelServerHealthStatus|[microsoftTunnelServerHealthStatus](../resources/intune-mstunnel-microsofttunnelserverhealthstatus.md)|O status de integridade do MicrosoftTunnelServer. Os valores possíveis são: `unknown`, `healthy`, `unhealthy`, `warning`, `offline`, `upgradeInProgress`, `upgradeFailed`.|
|lastCheckinDateTime|DateTimeOffset|Quando o MicrosoftTunnelServer último check-in|

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
  "lastCheckinDateTime": "String (timestamp)"
}
```




