---
title: Tipo de recurso printJobConfiguration
description: Um grupo de configurações que uma impressora deve usar para imprimir um trabalho.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 1e12541bd4426dca1e0d7b48b0e3bcbd9e2bb7ea
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517038"
---
# <a name="printjobconfiguration-resource-type"></a>Tipo de recurso printJobConfiguration

Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Um grupo de configurações que uma impressora deve usar para imprimir um trabalho.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|pageRanges|[Coleção integerRange](integerrange.md)|A página varia para imprimir. Somente leitura.|
|quality|[printQuality](enums.md#printquality-values)|A qualidade de impressão a ser usada ao imprimir o trabalho. Os valores válidos são descritos na tabela abaixo. Somente leitura.|
|dpi|Int32|A resolução a ser usada ao imprimir o trabalho, expressa em pontos por polegada (DPI). Somente leitura.|
|feedOrientation|printerFeedOrientation|A orientação a ser usada ao alimentar mídia na impressora. Os valores válidos são descritos na tabela a seguir. Somente leitura.|
|orientation|[printOrientation](enums.md#printorientation-values)|A configuração de orientação que a impressora deve usar ao imprimir o trabalho. Os valores válidos são descritos na tabela a seguir.|
|duplexMode|[printDuplexMode](enums.md#printduplexmode-values)|O modo duplex que a impressora deve usar ao imprimir o trabalho. Os valores válidos são descritos na tabela abaixo. Somente leitura.|
|copies|Int32|O número de cópias que devem ser impressas. Somente leitura.|
|colorMode|[printColorMode](enums.md#printcolormode-values)|O modo de cor que a impressora deve usar para imprimir o trabalho. Os valores válidos são descritos na tabela abaixo. Somente leitura.|
|inputBin|Cadeia de caracteres|A bandeja de entrada (bandeja) a ser usada durante a impressão. Consulte os recursos da [impressora para](printercapabilities.md) uma lista de caixas de entrada com suporte.|
|outputBin|Cadeia de caracteres|A lixeira de saída para colocar as impressões concluídas. Consulte os recursos da [impressora para](printercapabilities.md) uma lista de caixas de saída com suporte.|
|mediaSize|Cadeia de caracteres|O tamanho da mídia a ser usado ao imprimir. Oferece suporte a nomes de tamanho padrão para tamanhos de mídia ISO e ANSI, juntamente com todos os tamanhos personalizados suportados pela impressora associada.|
|margin|[printMargin](printmargin.md)|As configurações de margem a ser usadas ao imprimir.|
|mediaType|Cadeia de caracteres|O tipo de mídia padrão (como papel) para imprimir o documento. Os valores válidos são descritos na tabela a seguir.|
|finishings|[Coleção printFinishing](enums.md#printfinishing-values)|Processos de término a ser usado ao imprimir.|
|pagesPerSheet|Int32|O número de páginas de documento a ser impressa em cada planilha.
|multipageLayout|[printMultipageLayout](enums.md#printmultipagelayout-values)|A direção para colocar as páginas quando várias páginas estão sendo impressas por planilha. Os valores válidos são descritos na tabela a seguir.|
|collate|Booliano|Se a impressora deve colá-los para imprimir várias cópias de um documento de várias páginas.|
|scaling|[printScaling](enums.md#printscaling-values)|Especifica como a impressora deve dimensionar os dados do documento para se ajustar à mídia solicitada. Os valores válidos são descritos na tabela a seguir.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printJobConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printJobConfiguration",
  "pageRanges": [
    {
      "@odata.type": "microsoft.graph.integerRange"
    }
  ],
  "quality": "String",
  "dpi": "Integer",
  "feedOrientation": "String",
  "orientation": "String",
  "duplexMode": "String",
  "copies": "Integer",
  "colorMode": "String",
  "inputBin": "String",
  "outputBin": "String",
  "mediaSize": "String",
  "margin": {
    "@odata.type": "microsoft.graph.printMargin"
  },
  "mediaType": "String",
  "finishings": [
    "String"
  ],
  "pagesPerSheet": "Integer",
  "multipageLayout": "String",
  "collate": "Boolean",
  "scaling": "String",
  "fitPdfToPage": "Boolean"
}
```

