---
title: Tipo de recurso searchHit
description: Descrição da entidade searchHit
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 9cb3a33d3638a982dd0dfd17f3042565aa77e666
ms.sourcegitcommit: 84db9d70672e7a36a1130ff4f4b9baf3554d287f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2022
ms.locfileid: "66810253"
---
# <a name="searchhit-resource-type"></a>Tipo de recurso searchHit

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

Representa um único resultado dentro da lista de resultados da pesquisa.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|hitId|String|O identificador interno do item. O formato do identificador varia de acordo com o tipo de entidade. Para obter detalhes, consulte [o formato hitId](#hitid-format).|
|classificação|Int32|A classificação ou a ordem do resultado.|
|Contentsource|String|O nome da fonte de conteúdo da qual **o externalItem** faz parte.|
|summary|String|Um resumo do resultado, se um resumo estiver disponível.|
|resultTemplateId|String|ID do modelo de resultado para renderizar o resultado da pesquisa. Essa ID deve ser mapeada para um layout de exibição no dicionário **resultTemplates** , incluído na [resposta](searchresponse.md) de pesquisa também.|
|recurso|[entity](entity.md)|A representação subjacente do Microsoft Graph do resultado da pesquisa.|
|_id (preterido)|Cadeia de caracteres| Renomeado como **hitId**. O identificador interno do item.|
|_score (preterido)|Int32|Renomeado como **classificação**. A pontuação ou a ordem do resultado.|
|_summary (preterido)|String|Renomeado como **resumo**. Um resumo do resultado (se o resumo estiver disponível).|
|_sortField (preterido)|String|Essa propriedade foi removida.|
|_source (preterido)|[entity](entity.md)|Renomeado como **recurso**. A representação do Graph subjacente do resultado da pesquisa.|

### <a name="hitid-format"></a>Formato hitId
| Tipo de entidade     | Formato de ID        | Exemplo |
|:-------------|:------------|:------------|
|message|RestId|`AAMkAGIwMDA5MmY0LWY5ZTgtNGY5YS04NzczLWNhNjc0ZGIyZDBjYgBGAAAAAADm35sgHbzESapJ8_BjBlhEBwDAYtphe7dsRbDrOT-HAHoKAACmqNsoAADAYtphe7dsRbDrOT-HAHoKAAFsBhyEAAA=`|
|event|EwsId|`AAMkAGIwMDA5MmY0LWY5ZTgtNGY5YS04NzczLWNhNjc0ZGIyZDBjYgFRAAgI232z8Q+AAEYAAAAA5t+bIB28xEmqSfPgYwZYRAcAwGLaYXu3bEWw6zk/xwB6CgAAAAABDQAAwGLaYXu3bEWw6zk/xwB6CgABGnD/jwAAEA==`|
|list|GUID|`6249f5a0-c9fd-4103-8da5-8362fe911151`|
|listItem|GUID|`89b4aeff-de77-4b0e-bec9-a20cd4f6c32d` |
|site|Host, GUID, GUID|`microsoft.sharepoint.com,a5eb6988-c9ad-44be-b3b4-d334d01066c0,4c5ce7de-dbe6-4807-9909-3018f0b83266`|
|Unidade|Cadeia de caracteres codificada|`b!kf7AlbfRu0SMqtfcmhLTwf7MGLd-Z0BEqfzvkoqsr21iQFpfPV09TIVf1sa8xOJ0` |
|driveItem|Cadeia de caracteres codificada|`01ALOVTAX7V22IS566BZF35SNCBTKPNQZN`|
|externalItem|Cadeia de caracteres codificada|`AAMkADRiYWU5MDRkLWE1NGEtNDg5OS1hZWM2LWIxOWZmNzQzMTdiYQBGAAAAAAAvZTGE+1bNQp4lDRL1ctayBwCQNOp97HTbQK/QVOV30iomAAAAEF6yAACQNOp97HTbQK/QVOV30iomAAAAG/DWAAA=` |
|person|GUID@GUID|`497b7a2a-9e1a-48d7-80e8-2965d2fc3a81@72f988bf-86f1-41af-91ab-2d7cd011db47`|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchHit",
  "baseType": null
}-->

```json
{
  "hitId": "String",
  "rank": 1,
  "summary": "String",
  "resultTemplateId": "String",
  "contentSource": "String",
  "resource": { "@odata.type": "microsoft.graph.entity" },
  "_id": "String",
  "_score": 1024,
  "_sortField": "String",
  "_summary": "String",
  "_source": { "@odata.type": "microsoft.graph.entity" }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchHit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

