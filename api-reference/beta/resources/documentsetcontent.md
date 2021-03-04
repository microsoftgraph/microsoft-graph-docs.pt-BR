---
author: swapnil1993
title: Tipo de recurso documentSetContent
description: O recurso documentSetContent contém metadados sobre um arquivo presente no local de conteúdo padrão de um conteúdo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 8597dfb8a762d2166a9253fb4e806b9c2fcf5223
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445907"
---
# <a name="documentsetcontent-resource-type"></a>Tipo de recurso documentSetContent

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Contém metadados sobre um arquivo presente no local de conteúdo padrão de um tipo de conteúdo.

## <a name="properties"></a>Propriedades

| Nome da propriedade  | Tipo    | Descrição
|:---------------|:--------|:--------------------------------------------------
| contentType    | microsoft.graph.contentTypeInfo | Informações de tipo de conteúdo do arquivo. 
| fileName      | string  | Nome do arquivo na pasta de recursos que deve ser adicionado como um conteúdo padrão ou um modelo no conjunto de documentos  
| folderName         | string  | Nome da pasta no qual o arquivo será colocado quando um novo conjunto de documentos for criado na biblioteca.

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON de um **recurso documentSetContent.**
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.documentSetContent" } -->

```json
{
  "contentType": { "@type": "microsoft.graph.contentTypeInfo" },
  "fileName": "string",
  "folderName": "string"
}
```