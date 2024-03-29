---
title: Tipo de recurso microsoftTunnelConfiguration
description: Entidade que representa uma coleção de Microsoft Tunnel configurações
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 90086f8b01f1991ff7135f5f5b10dc179570d6d0
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63367773"
---
# <a name="microsofttunnelconfiguration-resource-type"></a>Tipo de recurso microsoftTunnelConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa uma coleção de Microsoft Tunnel configurações

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar microsoftTunnelConfigurations](../api/intune-mstunnel-microsofttunnelconfiguration-list.md)|[coleção microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md)|Listar propriedades e relações dos [objetos microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) .|
|[Obter microsoftTunnelConfiguration](../api/intune-mstunnel-microsofttunnelconfiguration-get.md)|[microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md)|Leia propriedades e relações do [objeto microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) .|
|[Criar microsoftTunnelConfiguration](../api/intune-mstunnel-microsofttunnelconfiguration-create.md)|[microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md)|Crie um novo [objeto microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) .|
|[Excluir microsoftTunnelConfiguration](../api/intune-mstunnel-microsofttunnelconfiguration-delete.md)|Nenhuma|Exclui um [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md).|
|[Atualizar microsoftTunnelConfiguration](../api/intune-mstunnel-microsofttunnelconfiguration-update.md)|[microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md)|Atualize as propriedades de um [objeto microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Id do MicrosoftTunnelConfiguration|
|displayName|String|O nome de exibição do MicrosoftTunnelConfiguration|
|description|Cadeia de caracteres|A descrição do MicrosoftTunnelConfiguration|
|network|String|A sub-rede que será usada para alocar endereço virtual para os clientes|
|dnsServers|Coleção String|Os servidores DNS que serão usados pelos clientes|
|defaultDomainSuffix|Cadeia de caracteres|O apêndice Domínio Padrão que será usado pelos clientes|
|routesInclude|Coleção String|Os routs que serão roteados pelo servidor|
|routesExclude|Coleção String|Subconjunto das rotas que não serão roteadas pelo servidor|
|splitDNS|Coleção String|Os domínios que serão resolvidos usando os servidores dns fornecidos|
|listenPort|Int32|A porta que o TCP e o UPD escutarão no servidor|
|advancedSettings|Coleção [keyValuePair](../resources/intune-mstunnel-keyvaluepair.md)|Configurações adicionais que podem ser aplicadas ao servidor|
|lastUpdateDateTime|DateTimeOffset|Quando o MicrosoftTunnelConfiguration foi atualizado pela última vez|
|roleScopeTagIds|String collection|Lista de marcas de escopo para esta instância entity.|
|disableUdpConnections|Booliano|Quando DisableUdpConnections for definido, os clientes e o servidor VPN não usarão conexões DTLS para dados de tansfer.|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftTunnelConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftTunnelConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "network": "String",
  "dnsServers": [
    "String"
  ],
  "defaultDomainSuffix": "String",
  "routesInclude": [
    "String"
  ],
  "routesExclude": [
    "String"
  ],
  "splitDNS": [
    "String"
  ],
  "listenPort": 1024,
  "advancedSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "lastUpdateDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "disableUdpConnections": true
}
```




