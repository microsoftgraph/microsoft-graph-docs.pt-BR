---
title: tipo de recurso microsoftTunnelConfiguration
description: Entidade que representa uma coleção de configurações de encapsulamento da Microsoft
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4cd85d798085ed5d8caf12ae2becc58e2bf10a33
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301415"
---
# <a name="microsofttunnelconfiguration-resource-type"></a>tipo de recurso microsoftTunnelConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa uma coleção de configurações de encapsulamento da Microsoft

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar microsoftTunnelConfigurations](../api/intune-mstunnel-microsofttunnelconfiguration-list.md)|coleção [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md)|Listar Propriedades e relações dos objetos [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) .|
|[Obter microsoftTunnelConfiguration](../api/intune-mstunnel-microsofttunnelconfiguration-get.md)|[microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md)|Leia as propriedades e as relações do objeto [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) .|
|[Criar microsoftTunnelConfiguration](../api/intune-mstunnel-microsofttunnelconfiguration-create.md)|[microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md)|Criar um novo objeto [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) .|
|[Excluir microsoftTunnelConfiguration](../api/intune-mstunnel-microsofttunnelconfiguration-delete.md)|Nenhum|Exclui [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md).|
|[Atualizar microsoftTunnelConfiguration](../api/intune-mstunnel-microsofttunnelconfiguration-update.md)|[microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md)|Atualiza as propriedades de um objeto [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID do MicrosoftTunnelConfiguration|
|displayName|String|O nome de exibição do MicrosoftTunnelConfiguration|
|description|String|A descrição do MicrosoftTunnelConfiguration|
|rede|String|A sub-rede que será usada para alocar o endereço virtual para os clientes|
|dnsServers|Coleção de cadeias de caracteres|Os servidores DNS que serão usados pelos clientes|
|defaultDomainSuffix|String|O apêndice de domínio padrão que será usado pelos clientes|
|routesInclude|Coleção de cadeias de caracteres|O routs que será roteado pelo servidor|
|routesExclude|Coleção de cadeias de caracteres|Subconjuntos de rotas que não serão encaminhadas pelo servidor|
|splitDNS|Coleção de cadeias de caracteres|Os domínios que serão resolvidos usando os servidores DNS fornecidos|
|listenPort|Int32|A porta na qual o TCP e o UPD serão escutados no servidor|
|advancedSettings|Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Configurações adicionais que podem ser aplicadas ao servidor|
|lastUpdateDateTime|DateTimeOffset|Quando o MicrosoftTunnelConfiguration foi atualizado pela última vez|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância de entidade.|

## <a name="relationships"></a>Relações
Nenhum

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
  ]
}
```




