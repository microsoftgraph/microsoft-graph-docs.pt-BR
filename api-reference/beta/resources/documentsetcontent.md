---
author: swapnil1993
title: Tipo de recurso documentSetContent
description: O recurso documentSetContent contém metadados sobre um arquivo presente no local de conteúdo padrão de um conteúdo.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 0ec71779247f143c0f43f1695c75049af15d453f
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63722979"
---
# <a name="documentsetcontent-resource-type"></a>Tipo de recurso documentSetContent

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Contém metadados sobre um arquivo presente no local de conteúdo padrão de um tipo de conteúdo.

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo                            | Descrição                                                                                                     |
| :---------- | :------------------------------ | :-------------------------------------------------------------------------------------------------------------- |
| contentType | microsoft.graph.contentTypeInfo | Informações de tipo de conteúdo do arquivo.                                                                           |
| fileName    | string                          | Nome do arquivo na pasta de recursos que deve ser adicionado como um conteúdo padrão ou um modelo no conjunto de documentos |
| folderName  | string                          | Nome da pasta no qual o arquivo será colocado quando um novo conjunto de documentos for criado na biblioteca.                 |

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON de um **recurso documentSetContent** .

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.documentSetContent" } -->

```json
{
  "contentType": { "@type": "microsoft.graph.contentTypeInfo" },
  "fileName": "string",
  "folderName": "string"
}
```
