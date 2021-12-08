---
title: Tipo de recurso microsoftTunnelSite
description: Entidade que representa um Microsoft Tunnel site
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4f4ce76a16d63d4d97c7ab27fa74c53fdcdc3408
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61347316"
---
# <a name="microsofttunnelsite-resource-type"></a>Tipo de recurso microsoftTunnelSite

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa um Microsoft Tunnel site

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar microsoftTunnelSites](../api/intune-mstunnel-microsofttunnelsite-list.md)|[Coleção microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md)|Listar propriedades e relações dos [objetos microsoftTunnelSite.](../resources/intune-mstunnel-microsofttunnelsite.md)|
|[Obter microsoftTunnelSite](../api/intune-mstunnel-microsofttunnelsite-get.md)|[microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md)|Leia propriedades e relações do [objeto microsoftTunnelSite.](../resources/intune-mstunnel-microsofttunnelsite.md)|
|[Criar microsoftTunnelSite](../api/intune-mstunnel-microsofttunnelsite-create.md)|[microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md)|Crie um novo [objeto microsoftTunnelSite.](../resources/intune-mstunnel-microsofttunnelsite.md)|
|[Excluir microsoftTunnelSite](../api/intune-mstunnel-microsofttunnelsite-delete.md)|Nenhum|Exclui um [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md).|
|[Atualizar microsoftTunnelSite](../api/intune-mstunnel-microsofttunnelsite-update.md)|[microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md)|Atualize as propriedades de um [objeto microsoftTunnelSite.](../resources/intune-mstunnel-microsofttunnelsite.md)|
|[Ação requestUpgrade](../api/intune-mstunnel-microsofttunnelsite-requestupgrade.md)|Nenhuma|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Id do MicrosoftTunnelSite|
|displayName|String|O nome de exibição do MicrosoftTunnelSite|
|descrição|String|Descrição do MicrosoftTunnelSite|
|publicAddress|String|O nome de domínio público do MicrosoftTunnelSite ou o endereço IP|
|upgradeWindowUtcOffsetInMinutes|Int32|O timezone do site representado como um deslocamento de minuto do UTC|
|upgradeWindowStartTime|TimeOfDay|Hora de início da janela de atualização do site|
|upgradeWindowEndTime|TimeOfDay|Hora de término da janela de atualização do site|
|upgradeAutomatically|Booliano|A configuração de atualização automática do site. True para atualizações automáticas, false para controle manual|
|upgradeAvailable|Boolean|True se uma atualização estiver disponível|
|internalNetworkProbeUrl|String|A URL da Sonda de Acesso à Rede Interna do MicrosoftTunnelSite|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância entity.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|microsoftTunnelConfiguration|[microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md)|O MicrosoftTunnelConfiguration que foi aplicado a este MicrosoftTunnelSite|
|microsoftTunnelServers|[Coleção microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)|Uma lista de MicrosoftTunnelServers que estão registrados neste MicrosoftTunnelSite|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftTunnelSite"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftTunnelSite",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publicAddress": "String",
  "upgradeWindowUtcOffsetInMinutes": 1024,
  "upgradeWindowStartTime": "String (time of day)",
  "upgradeWindowEndTime": "String (time of day)",
  "upgradeAutomatically": true,
  "upgradeAvailable": true,
  "internalNetworkProbeUrl": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```




