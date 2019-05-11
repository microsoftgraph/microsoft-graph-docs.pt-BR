---
title: tipo de recurso vpnProxyServer
description: Servidor proxy VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 73b004eaae0b49c9f3e4341c32923d7f2d48ae45
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944576"
---
# <a name="vpnproxyserver-resource-type"></a>tipo de recurso vpnProxyServer

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Servidor proxy VPN.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|automaticConfigurationScriptUrl|Cadeia de caracteres|URL do script de configuração automática do proxy.|
|address|Cadeia de caracteres|Enfrentar.|
|propor|Int32|Propor. Valores válidos de 0 a 65535|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024
}
```




