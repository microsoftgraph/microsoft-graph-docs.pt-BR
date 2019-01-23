---
title: tipo de recurso de windows10VpnProxyServer
description: Servidor de Proxy VPN.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d4f8975a08e60105c37e0959ac72e24a1dd639cd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407120"
---
# <a name="windows10vpnproxyserver-resource-type"></a>tipo de recurso de windows10VpnProxyServer

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Servidor de Proxy VPN.


Herda de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|automaticConfigurationScriptUrl|String|Url de script de configuração automática do proxy. Herdado de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|address|Cadeia de caracteres|Endereço. Herdado de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|porta|Int32|Porta. 0 a 65.535 Inherited de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md) de valores válido|
|bypassProxyServerForLocalAddress|Boolean|Ignorar servidor proxy para endereços locais.|

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




