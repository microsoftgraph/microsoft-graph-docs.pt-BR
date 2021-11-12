---
title: Tipo de recurso printerDefaults
description: Representa as configurações padrão da impressora. Verifique os recursos da impressora para ver todos os valores compatíveis.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 4a76d1590cc6b180786d48e889796769b0de2c2b
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60936975"
---
# <a name="printerdefaults-resource-type"></a>Tipo de recurso printerDefaults

Namespace: microsoft.graph

Representa as configurações padrão da impressora. Verifique os recursos da [impressora para](printercapabilities.md) ver todos os valores compatíveis.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|copiesPerJob|Int32|O número padrão de cópias impressas por trabalho.|
|contentType|String|O tipo de conteúdo padrão (MIME) a ser usado ao processar documentos.|
|finishings|[Coleção printFinishing](enums.md#printfinishing-values)|O conjunto padrão de acabamentos a ser aplicado a trabalhos de impressão. Os valores válidos são descritos na tabela a seguir.|
|mediaColor|Cadeia de caracteres|A cor padrão da mídia (como papel) para imprimir o documento.|
|mediaType|Cadeia de caracteres|O tipo de mídia padrão (como papel) para imprimir o documento.|
|mediaSize|Cadeia de caracteres|O tamanho de mídia padrão a ser usado. Oferece suporte a nomes de tamanho padrão para tamanhos de mídia ISO e ANSI. Os valores válidos são listados no tópico [printerCapabilities.](printercapabilities.md#mediasizes-values)|
|pagesPerSheet|Int32|O número padrão de páginas de documento a ser impressa em cada planilha.
|orientation|[printOrientation](enums.md#printorientation-values)|A orientação padrão a ser usada ao imprimir o documento. Os valores válidos são descritos na tabela a seguir.|
|outputBin|Cadeia de caracteres|A lixeira de saída padrão para colocar as impressões concluídas. Consulte os recursos da [impressora para](printercapabilities.md) uma lista de caixas de saída com suporte.|
|fitPdfToPage|Boolean|A configuração padrão fitPdfToPage. True para ajustar cada página de um documento PDF a uma folha física de mídia; false para permitir que a impressora decida como definir impressões.|
|multipageLayout|[printMultipageLayout](enums.md#printmultipagelayout-values)|A direção padrão para colocar as páginas quando várias páginas estão sendo impressas por planilha. Os valores válidos são descritos na tabela a seguir.|
|colorMode|[printColorMode](enums.md#printcolormode-values)|O modo de cor padrão a ser usado ao imprimir o documento. Os valores válidos são descritos na tabela a seguir.|
|quality|[printQuality](enums.md#printquality-values)|A qualidade padrão a ser usada ao imprimir o documento. Os valores válidos são descritos na tabela a seguir.|
|duplexMode|[printDuplexMode](enums.md#printduplexmode-values)|A configuração duplex padrão (com duas laterais) a ser usada ao imprimir um documento. Os valores válidos são descritos na tabela a seguir.|
|dpi|Int32|A resolução padrão no DPI a ser usada ao imprimir o trabalho.|
|escala|[printScaling](enums.md#printscaling-values)|Especifica como a impressora dimensiona os dados do documento para se ajustar à mídia solicitada. Os valores válidos são descritos na tabela a seguir.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printerDefaults"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerDefaults",
  "copiesPerJob": "Integer",
  "contentType": "String",
  "finishings": [
    "String"
  ],
  "mediaColor": "String",
  "mediaType": "String",
  "mediaSize": "String",
  "pagesPerSheet": "Integer",
  "orientation": "String",
  "outputBin": "String",
  "inputBin": "String",
  "fitPdfToPage": "Boolean",
  "multipageLayout": "String",
  "colorMode": "String",
  "quality": "String",
  "duplexMode": "String",
  "dpi": "Integer",
  "scaling": "String"
}
```

