---
title: tipo de recurso airPrintDestination
description: Representa um destino de impressão.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3218a40ee1a735cef585866e1ca0c9f80ad95671
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31779969"
---
# <a name="airprintdestination-resource-type"></a>tipo de recurso airPrintDestination

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um destino de impressão.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ipAddress|Cadeia de caracteres|O endereço IP do destino de impressão.|
|resourcePath|Cadeia de caracteres|O caminho do recurso associado à impressora. Isso corresponde ao parâmetro RP do registro Bonjour _ipps. TCP. Por exemplo: impressoras/Canon_MG5300_series, impressoras/Xerox_Phaser_7600, IPP/imprimir, Epson_IPP_Printer.|
|propor|Int32|A porta de escuta do destino de impressão. Se essa chave não for especificada, a impressão de impressa usará a porta padrão. Disponível no iOS 11,0 e posterior.|
|forceTls|Booliano|Se as conexões de impressão de verdade forem protegidas por TLS (Transport Layer Security). O padrão é false. Disponível no iOS 11,0 e posterior.|

## <a name="relationships"></a>Relações
Nenhuma

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





