---
title: Tipo de recurso attachmentSession
description: Representa um recurso que carrega anexos grandes em um todoTask.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 71be9f9afb61735341f98e77b7790b724fcd036a
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645585"
---
# <a name="attachmentsession-resource-type"></a>Tipo de recurso attachmentSession

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um recurso que carrega anexos grandes em um [todoTask](../resources/todotask.md).

Herda de [entidade](../resources/entity.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|conteúdo|Fluxo|Os fluxos de conteúdo carregados.|
|expirationDateTime|DateTimeOffset| A data e a hora em UTC em que a sessão de upload expirará. O arquivo completo deve ser carregado antes que esta hora de expiração seja atingida.|
|id|Cadeia de caracteres|Identificador exclusivo para a sessão de anexo. Somente leitura. Herdado da [entidade](../resources/entity.md).|
|nextExpectedRanges|Coleção de cadeias de caracteres|Indica um único valor que `{start}` representa o local no arquivo em que o próximo carregamento deve começar.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attachmentSession",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attachmentSession",
  "content": "Stream",
  "expirationDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "nextExpectedRanges": [
    "String"
  ]
}
```

