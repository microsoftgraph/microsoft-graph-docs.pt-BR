---
title: Tipo de recurso windows10VpnProxyServer
description: Servidor Proxy VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b60102b1139bc1c869082016afb1436bcf061b94
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58785735"
---
# <a name="windows10vpnproxyserver-resource-type"></a>Tipo de recurso windows10VpnProxyServer

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Servidor Proxy VPN.


Herda de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|automaticConfigurationScriptUrl|Cadeia de caracteres|Url de script de configuração automática do proxy. Herdado [de vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|address|Cadeia de caracteres|Endereço. Herdado [de vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|port|Int32|Porta. Valores válidos de 0 a 65535 Herdados de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|bypassProxyServerForLocalAddress|Boleano|Ignorar o servidor proxy para endereço local.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10VpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10VpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024,
  "bypassProxyServerForLocalAddress": true
}
```



