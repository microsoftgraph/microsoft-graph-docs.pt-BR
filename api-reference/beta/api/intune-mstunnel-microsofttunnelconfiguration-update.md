---
title: Atualizar microsoftTunnelConfiguration
description: Atualize as propriedades de um objeto microsoftTunnelConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 286147139eb81f9d2e9d8ec0b8e4f463d433586f
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61343410"
---
# <a name="update-microsofttunnelconfiguration"></a>Atualizar microsoftTunnelConfiguration

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de um [objeto microsoftTunnelConfiguration.](../resources/intune-mstunnel-microsofttunnelconfiguration.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/microsoftTunnelConfigurations/{microsoftTunnelConfigurationId}
PATCH /deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelConfiguration
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto microsoftTunnelConfiguration.](../resources/intune-mstunnel-microsofttunnelconfiguration.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [o microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Id do MicrosoftTunnelConfiguration|
|displayName|String|O nome de exibição do MicrosoftTunnelConfiguration|
|descrição|String|A descrição do MicrosoftTunnelConfiguration|
|network|String|A sub-rede que será usada para alocar endereço virtual para os clientes|
|dnsServers|Coleção String|Os servidores DNS que serão usados pelos clientes|
|defaultDomainSuffix|String|O apêndice Domínio Padrão que será usado pelos clientes|
|routesInclude|Coleção de cadeias de caracteres|Os routs que serão roteados pelo servidor|
|routesExclude|Coleção String|Subconjunto das rotas que não serão roteadas pelo servidor|
|splitDNS|Coleção de cadeias de caracteres|Os domínios que serão resolvidos usando os servidores dns fornecidos|
|listenPort|Int32|A porta que o TCP e o UPD escutarão no servidor|
|advancedSettings|Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Configurações adicionais que podem ser aplicadas ao servidor|
|lastUpdateDateTime|DateTimeOffset|Quando o MicrosoftTunnelConfiguration foi atualizado pela última vez|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância entity.|
|disableUDPConnections|Boolean|Quando DisableUDPConnections for definido, os clientes e o servidor VPN não usarão as connctions DTLS para fazer o tansfer de dados.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelConfigurations/{microsoftTunnelConfigurationId}
Content-type: application/json
Content-length: 782

{
  "@odata.type": "#microsoft.graph.microsoftTunnelConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "network": "Network value",
  "dnsServers": [
    "Dns Servers value"
  ],
  "defaultDomainSuffix": "Default Domain Suffix value",
  "routesInclude": [
    "Routes Include value"
  ],
  "routesExclude": [
    "Routes Exclude value"
  ],
  "splitDNS": [
    "Split DNS value"
  ],
  "listenPort": 10,
  "advancedSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "disableUDPConnections": true
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 831

{
  "@odata.type": "#microsoft.graph.microsoftTunnelConfiguration",
  "id": "b8bdb469-b469-b8bd-69b4-bdb869b4bdb8",
  "displayName": "Display Name value",
  "description": "Description value",
  "network": "Network value",
  "dnsServers": [
    "Dns Servers value"
  ],
  "defaultDomainSuffix": "Default Domain Suffix value",
  "routesInclude": [
    "Routes Include value"
  ],
  "routesExclude": [
    "Routes Exclude value"
  ],
  "splitDNS": [
    "Split DNS value"
  ],
  "listenPort": 10,
  "advancedSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "disableUDPConnections": true
}
```




