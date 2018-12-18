---
title: tipo de recurso de windows10VpnProxyServer
description: Servidor de Proxy VPN.
author: tfitzmac
ms.openlocfilehash: e21b964ab1bd648cd042a1364ecf5f0942ded085
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309454"
---
# <a name="windows10vpnproxyserver-resource-type"></a>tipo de recurso de windows10VpnProxyServer

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

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





