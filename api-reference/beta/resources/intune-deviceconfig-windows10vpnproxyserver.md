---
title: Tipo de recurso windows10VpnProxyServer
description: Servidor Proxy VPN.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a9ab8f6ab7a662487d7cf8e144cd25bb8bd53a0f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59147903"
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
|automaticConfigurationScriptUrl|Cadeia de Caracteres|Url de script de configuração automática do proxy. Herdado [de vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
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



