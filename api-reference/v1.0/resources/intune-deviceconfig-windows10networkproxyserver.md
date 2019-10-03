---
title: Tipo de recurso windows10NetworkProxyServer
description: Política de Servidor Proxy de Rede.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b126358a8ab8574d4dcbf7c1f22e412eda41d61f
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37367053"
---
# <a name="windows10networkproxyserver-resource-type"></a>Tipo de recurso windows10NetworkProxyServer

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

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




