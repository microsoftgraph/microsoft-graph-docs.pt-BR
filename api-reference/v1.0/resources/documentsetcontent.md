---
author: swapnil1993
title: Tipo de recurso documentSetContent
description: O recurso documentSetContent contém metadados sobre um arquivo presente no local de conteúdo padrão de um conteúdo.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 741047ab90badd16e4f7dea61c92ca8d952ee978
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59072537"
---
# <a name="documentsetcontent-resource-type"></a>Tipo de recurso documentSetContent

Namespace: microsoft.graph

Representa o conteúdo padrão do conjunto de documentos SharePoint.
## <a name="properties"></a>Propriedades

| Nome da propriedade  | Tipo    | Descrição|
|:---------------|:--------|:--------------------------------------------------|
| contentType    | microsoft.graph.contentTypeInfo | Informações de tipo de conteúdo do arquivo. |
| fileName      | cadeia de caracteres  | Nome do arquivo na pasta de recursos que deve ser adicionado como um conteúdo padrão ou um modelo no conjunto de documentos.|
| folderName         | cadeia de caracteres  | Nome da pasta no qual o arquivo será colocado quando um novo conjunto de documentos for criado na biblioteca.|

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
