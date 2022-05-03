---
title: Tipo de recurso printJobStatus
description: Representa o status atual de um trabalho de impressão.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 73038bbea54860ef37b8ebbf2602450dc556efd2
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176676"
---
# <a name="printjobstatus-resource-type"></a>Tipo de recurso printJobStatus

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o status atual de um trabalho de impressão.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|state|printJobProcessingState|O estado de processamento atual do trabalho de impressão. Os valores válidos são descritos na tabela a seguir. Somente leitura.|
|detalhes|Coleção printJobProcessingDetail|Detalhes adicionais para o estado do trabalho de impressão. Os valores válidos são descritos na tabela a seguir. Somente leitura.|
|description|Cadeia de caracteres|Uma descrição legível por humanos do estado de processamento atual do trabalho de impressão. Somente leitura.|
|isAcquiredByPrinter|Booliano|True se o trabalho foi confirmado por uma impressora; caso contrário, false. Somente leitura.|

### <a name="printjobprocessingstate-values"></a>Valores printJobProcessingState

|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|0|O estado de processamento relatado pela impressora não é reconhecido.|
|Pendente|1|O trabalho de impressão está aguardando processamento pela impressora.|
|Processamento|2|No momento, o trabalho de impressão está sendo processado pela impressora.|
|Pausado|3|O trabalho de impressão foi pausado.|
|Parou|4|O trabalho de impressão foi interrompido porque um problema com a impressora precisa ser resolvido antes que o trabalho possa continuar. Mais informações podem ser encontradas no recurso de estado da impressora.|
|Concluído|5|O trabalho de impressão foi concluído com êxito e nenhum processamento adicional ocorrerá.|
|Cancelado|6 |O trabalho de impressão foi cancelado por um usuário e nenhum processamento adicional ocorrerá.|
|Abortado|7 |O trabalho de impressão foi anulado por um usuário ou pela impressora e nenhum processamento adicional ocorrerá.|

### <a name="printjobprocessingdetail-values"></a>Valores printJobProcessingDetail

|Membro|Valor|Descrição|
|:---|:---|:---|
|uploadPending|0|O conteúdo do documento não foi carregado.|
|Transformar|1|A carga do documento está sendo transformada.|
|completedSuccessfully|2|O trabalho foi concluído com êxito.|
|completedWithWarnings|3|O trabalho foi concluído com avisos.|
|completedWithErrors|4|O trabalho foi concluído com erros.|
|releaseWait|5|O trabalho está pendente para ser liberado.|
|Interpretação|6 |O trabalho está no estado de "processamento", mas, mais especificamente, a carga do documento está sendo interpretada.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printJobStatus"
}-->

```json
{
    "state": "String",
    "description": "String",
    "isAcquiredByPrinter": true,    
    "details": ["String"]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printJobStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

