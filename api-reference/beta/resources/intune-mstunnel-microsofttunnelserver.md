---
title: Tipo de recurso microsoftTunnelServer
description: Entidade que representa um único Microsoft Tunnel servidor
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ad8186090c30267890e2e1240111edd1a8de5a6eb5c52e452fe9570d32dc319c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54227257"
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
|[Excluir microsoftTunnelServer](../api/intune-mstunnel-microsofttunnelserver-delete.md)|Nenhum|Exclui um [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md).|
|[Atualizar o microsoftTunnelServer](../api/intune-mstunnel-microsofttunnelserver-update.md)|[microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)|Atualize as propriedades de um [objeto microsoftTunnelServer.](../resources/intune-mstunnel-microsofttunnelserver.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Id do MicrosoftTunnelServer|
|displayName|Cadeia de caracteres|O nome de exibição do MicrosoftTunnelServer|
|tunnelServerHealthStatus|[microsoftTunnelServerHealthStatus](../resources/intune-mstunnel-microsofttunnelserverhealthstatus.md)|O status de saúde do MicrosoftTunnelServer. Os valores possíveis são: `unknown`, `healthy`, `unhealthy`, `warning`, `offline`, `upgradeInProgress`, `upgradeFailed`.|
|lastCheckinDateTime|DateTimeOffset|Quando o MicrosoftTunnelServer entrou pela última vez|

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




