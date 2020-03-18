---
title: tipo de recurso airPrintDestination
description: Representa um destino de impressão.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b0f77b9f0ee3ff3abe46a41b0c6760a15d7aa2c1
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797203"
---
# <a name="airprintdestination-resource-type"></a>tipo de recurso airPrintDestination

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um destino de impressão.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ipAddress|Cadeia de caracteres|O endereço IP do destino de impressão.|
|resourcePath|String|O caminho do recurso associado à impressora. Isso corresponde ao parâmetro RP do registro _ipps. TCP Bonjour. Por exemplo: impressoras/Canon_MG5300_series, impressoras/Xerox_Phaser_7600, IPP/imprimir Epson_IPP_Printer.|
|propor|Int32|A porta de escuta do destino de impressão. Se essa chave não for especificada, a impressão de impressa usará a porta padrão. Disponível no iOS 11,0 e posterior.|
|forceTls|Boolean|Se as conexões de impressão de verdade forem protegidas por TLS (Transport Layer Security). O padrão é false. Disponível no iOS 11,0 e posterior.|

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



