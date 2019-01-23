---
title: tipo de recurso de airPrintDestination
description: Representa um destino AirPrint.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3f56578427427d45a69c4c64fe9fde3cf31f8fd9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422492"
---
# <a name="airprintdestination-resource-type"></a>tipo de recurso de airPrintDestination

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Representa um destino AirPrint.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ipAddress|Cadeia de caracteres|O endereço IP de destino AirPrint.|
|resourcePath|String|O caminho do recurso associado à impressora. Isso corresponde ao parâmetro rp do registro Bonjour _ipps.tcp. Por exemplo: impressoras/Canon_MG5300_series, impressoras/Xerox_Phaser_7600, ipp/impressão, Epson_IPP_Printer.|
|porta|Int32|A porta de escuta do destino AirPrint. Se essa chave não for especificado, AirPrint usará a porta padrão. Disponível no iOS 11.0 e versões posteriores.|
|forceTls|Boolean|Se true conexões de AirPrint são protegidas pela segurança de camada de transporte (TLS). O padrão é false. Disponível no iOS 11.0 e versões posteriores.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.airPrintDestination"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.airPrintDestination",
  "ipAddress": "String",
  "resourcePath": "String",
  "port": 1024,
  "forceTls": true
}
```




