---
author: swapnil1993
title: Tipo de recurso documentSet
description: Contém metadados sobre configurações de conjunto de documentos.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: d6a997dd721200eb732f83fb53bbb3155921f111
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758295"
---
# <a name="documentset-resource-type"></a>Tipo de recurso documentSet

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Contém metadados sobre configurações de conjunto de documentos.

## <a name="properties"></a>Propriedades

| Propriedade                    | Tipo                                           | Descrição                                                                                                                       |
| :-------------------------- | :--------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------- |
| allowedContentTypes         | Collection(microsoft.graph.contentTypeInfo)    | Tipos de conteúdo permitidos no conjunto de documentos.                                                                                            |
| defaultContents             | Collection(microsoft.graph.documentSetContent) | Conteúdo padrão do conjunto de documentos.                                                                                                 |
| propagateWelcomePageChanges | Booliano                                        | Indica se é preciso adicionar o nome do documento definido a cada nome de arquivo.                                                          |
| shouldPrefixNameToFile      | Boolean                                        | Adicione o nome do Conjunto de Documentos a cada nome de arquivo.                                                                               |
| welcomePageUrl              | cadeia de caracteres                                         | URL absoluta da página de boas-vindas.                                                                                                        |

## <a name="relationships"></a>Relações

| Relação   | Tipo                      | Descrição
|:----------------|:--------------------------|:-------------------------------
| sharedColumns       | Collection(microsoft.graph.columnDefinition) | Colunas editadas no conjunto de documentos que se sincronizam com todos os documentos no conjunto. Eles são somente leitura nos próprios documentos. 
| welcomePageColumns  | Collection(microsoft.graph.columnDefinition)  | Especifica colunas a mostrar na página de boas-vindas para o conjunto de documentos.

## <a name="json-representation"></a>Representação JSON

A seguir está uma representação JSON de um **recurso documentSet** .

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.documentSet" } -->

```json
{
  "shouldPrefixNameToFile": true,
  "allowedContentTypes": [{ "@type": "microsoft.graph.contentTypeInfo" }],
  "defaultContents": [{ "@type": "microsoft.graph.documentSetContent" }],
  "propagateWelcomePageChanges": false,
  "welcomePageUrl": "string"
}
```

[contentTypeInfo]: contentTypeInfo.md
[documentSetContent]: documentsetcontent.md
