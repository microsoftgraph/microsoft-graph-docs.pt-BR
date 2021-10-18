---
title: Tipo de recurso subjectRightsRequestDetail
description: Representa os detalhes de uma solicitação de direitos de assunto, incluindo o número de itens encontrados, o número de itens revisados e assim por diante.
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: aab09a9ba567e3725f1d8ff72c027f950e4f969e
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60451321"
---
# <a name="subjectrightsrequestdetail-resource-type"></a>Tipo de recurso subjectRightsRequestDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de uma solicitação de direitos de assunto, incluindo o número de itens encontrados, o número de itens revisados e assim por diante.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|excludedItemCount|Int64|Contagem de itens excluídos da solicitação.|
|insightCounts|Coleção [keyValuePair](../resources/keyvaluepair.md)|Contagem de itens por insight.|
|itemCount|Int64|Contagem de itens encontrados.|
|itemNeedReview|Int64|Contagem do item que precisa de revisão.|
|productItemCounts|Coleção [keyValuePair](../resources/keyvaluepair.md)|Contagem de itens por produto, como Exchange, SharePoint, OneDrive e Teams.|
|signedOffItemCount|Int64|Contagem de itens assinados pelo administrador.|
|totalItemSize|Int64|Tamanho total do item em bytes.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.subjectRightsRequestDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.subjectRightsRequestDetail",
      "itemCount": "Int64",
      "totalItemSize": "Int64",
      "itemNeedReview": "Int64",
      "signedOffItemCount": "Int64",
      "excludedItemCount": "Int64",
      "productItemCounts": [],
      "insightCounts": []
}
```

