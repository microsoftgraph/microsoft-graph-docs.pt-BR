---
author: swapnil1993
title: Tipo de recurso documentSet
description: Contém metadados sobre configurações de conjunto de documentos.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: c39eeb8689f882939d506eb8e68e2d6c9409e350
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63721659"
---
# <a name="documentset-resource-type"></a>Tipo de recurso documentSet

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Contém metadados sobre configurações de conjunto de documentos.

## <a name="properties"></a>Propriedades

| Propriedade                    | Tipo                                           | Descrição                                                                                                                       |
| :-------------------------- | :--------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------- |
| shouldPrefixNameToFile      | Booliano                                        | Adicione o nome do Conjunto de Documentos a cada nome de arquivo.                                                                               |
| allowedContentTypes         | Collection(microsoft.graph.contentTypeInfo)    | Tipos de conteúdo permitidos no conjunto de documentos.                                                                                            |
| defaultContents             | Collection(microsoft.graph.documentSetContent) | Conteúdo padrão do conjunto de documentos.                                                                                                 |
| propagateWelcomePageChanges | Boolean                                        | Especifica se a página de boas-vindas deve ser pressionada para tipos de conteúdo herdados.                                                        |
| sharedColumns               | Collection(microsoft.graph.columnDefinition)   | Colunas editadas no conjunto de documentos que se sincronizam com todos os documentos no conjunto. Eles são somente leitura nos próprios documentos. |
| welcomePageColumns          | Collection(microsoft.graph.columnDefinition)   | Especifica colunas a mostrar na página de boas-vindas para o conjunto de documentos.                                                               |
| welcomePageUrl              | string                                         | URL absoluta da página de boas-vindas.                                                                                                        |

## <a name="json-representation"></a>Representação JSON

A seguir está uma representação JSON de um **recurso documentSet** .

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
