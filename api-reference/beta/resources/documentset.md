---
author: swapnil1993
title: Tipo de recurso documentSet
description: Contém metadados sobre configurações de conjunto de documentos.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 25a2b5e71c76a8a097ff9c490313ae6d319abeb8
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445906"
---
# <a name="documentset-resource-type"></a>Tipo de recurso documentSet

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Contém metadados sobre configurações de conjunto de documentos.

## <a name="properties"></a>Propriedades

| Nome da propriedade  | Tipo    | Descrição
|:---------------|:--------|:--------------------------------------------------
| shouldPrefixNameToFile | Booliano  | Adicione o nome do Conjunto de Documentos a cada nome de arquivo.
| allowedContentTypes | Collection(microsoft.graph.contentTypeInfo) | Tipos de conteúdo permitidos no conjunto de documentos.
| defaultContents     | Collection(microsoft.graph.documentSetContent) | Conteúdo padrão do conjunto de documentos.  
| propagateWelcomePageChanges | Booliano | Especifica se a página de boas-vindas deve ser pressionada para tipos de conteúdo herdados.  
| sharedColumns       | Collection(microsoft.graph.columnDefinition) | Colunas editadas no conjunto de documentos que se sincronizam com todos os documentos no conjunto. Eles são somente leitura nos próprios documentos. 
| welcomePageColumns  | Collection(microsoft.graph.columnDefinition)  | Especifica colunas a mostrar na página de boas-vindas para o conjunto de documentos.  
| welcomePageUrl      | string | URL absoluta da página de boas-vindas.  

## <a name="json-representation"></a>Representação JSON

A seguir está uma representação JSON de um **recurso documentSet.**
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.documentSet" } -->

```json
{
  "shouldPrefixNameToFile": true,
  "allowedContentTypes": [{ "@type": "microsoft.graph.contentTypeInfo" }],
  "defaultContents": [{ "@type": "microsoft.graph.documentSetContent" }],
  "propagateWelcomePageChanges": false,
  "sharedColumns": [{ "@type": "microsoft.graph.columnDefinition" }],
  "welcomePageColumns": [{ "@type": "microsoft.graph.columnDefinition" }],
  "welcomePageUrl": "string"
}
```

[contentTypeInfo]: contentTypeInfo.md
[documentSetContent]: documentsetcontent.md
