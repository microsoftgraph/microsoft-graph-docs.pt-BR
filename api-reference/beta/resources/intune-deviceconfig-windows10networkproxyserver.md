---
title: Tipo de recurso windows10NetworkProxyServer
description: Política de Servidor Proxy de Rede.
author: tfitzmac
ms.openlocfilehash: f0f56da348203c2b30a6d49e40e5148f4e7d818b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316818"
---
# <a name="windows10networkproxyserver-resource-type"></a>Tipo de recurso windows10NetworkProxyServer

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Política de Servidor Proxy de Rede.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|address|Cadeia de caracteres|Endereço para o servidor proxy. Especifique um endereço no formato <server>\[“:”<port>\]|
|exceptions|Coleção de cadeias de caracteres|Endereços que não devem usar o servidor proxy. O sistema não usará o servidor proxy para endereços que começam com o conteúdo especificado nesse nó.|
|useForLocalAddresses|Booliano|Especifica se o servidor proxy deve ser usado para endereços locais (intranet).|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10NetworkProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10NetworkProxyServer",
  "address": "String",
  "exceptions": [
    "String"
  ],
  "useForLocalAddresses": true
}
```





