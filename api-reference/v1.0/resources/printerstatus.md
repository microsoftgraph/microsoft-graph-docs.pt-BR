---
title: Tipo de recurso printerStatus
description: Representa o status de processamento da impressora, incluindo quaisquer erros.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: da2c455f08830ee7bbfdf38def36f03250b21877
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60936968"
---
# <a name="printerstatus-resource-type"></a>Tipo de recurso printerStatus

Namespace: microsoft.graph

Representa o status de processamento da impressora, incluindo quaisquer erros.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|state|printerProcessingState|O estado de processamento atual. Os valores válidos são descritos na tabela a seguir. Somente leitura.|
|detalhes|Coleção printerProcessingStateDetail|A lista de detalhes que descrevem por que a impressora está no estado atual. Os valores válidos são descritos na tabela a seguir. Somente leitura.|
|description|Cadeia de caracteres|Uma descrição aceitável para humanos do estado de processamento atual da impressora. Somente leitura.|

### <a name="printerprocessingstate-values"></a>printerProcessingState values

|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|0|O estado de processamento relatado pela impressora é desconhecido.|
|idle|1|A impressora está ociosa e pronta para aceitar novos trabalhos de impressão.|
|processamento|2|No momento, a impressora está mediante o processamento de um trabalho de impressão e processará todos os trabalhos pendentes após a conclusão.|
|stopped|3|A impressora encontrou um problema (por exemplo, ficou sem papel na bandeja ativa) e não pode continuar o trabalho de impressão atual até que o problema seja resolvido. Confira os **valores** de detalhes ou o valor **de descrição** para obter mais informações.|
|unknownFutureValue|4|Valor de sentinela de enumeração evolvável. Não usar.|

### <a name="printerprocessingstatedetail-values"></a>printerProcessingStateDetail values

[tipo de número printerProcessingStateDetail](./printerprocessingstatedetail.md)

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printerStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerStatus",
  "state": "String",
  "details": [
    "String"
  ],
  "description": "String"
}
```
