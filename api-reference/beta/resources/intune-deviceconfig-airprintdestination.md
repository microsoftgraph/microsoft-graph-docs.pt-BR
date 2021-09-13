---
title: Tipo de recurso airPrintDestination
description: Representa um destino AirPrint.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ad603ab29c7914ccb16845ceeddda89581a40568
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59095691"
---
# <a name="airprintdestination-resource-type"></a>Tipo de recurso airPrintDestination

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um destino AirPrint.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ipAddress|Cadeia de caracteres|O Endereço IP do destino AirPrint.|
|resourcePath|Cadeia de Caracteres|O Caminho do Recurso associado à impressora. Isso corresponde ao parâmetro rp do registro _ipps.tcp Bonjour. Por exemplo: impressoras/Canon_MG5300_series, impressoras/Xerox_Phaser_7600, ipp/impressão, Epson_IPP_Printer.|
|port|Int32|A porta de escuta do destino AirPrint. Se essa chave não for especificada, AirPrint usará a porta padrão. Disponível no iOS 11.0 e posterior.|
|forceTls|Boleano|Se as conexões AirPrint verdadeiras são protegidas pelo TLS (Transport Layer Security). O padrão é falso. Disponível no iOS 11.0 e posterior.|

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



