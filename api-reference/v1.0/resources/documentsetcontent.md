---
author: swapnil1993
title: Tipo de recurso documentSetContent
description: O recurso documentSetContent contém metadados sobre um arquivo presente no local de conteúdo padrão de um conteúdo.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 5894c31c990f2cd55d5646c44e569c310d599e39
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757637"
---
# <a name="documentsetcontent-resource-type"></a>Tipo de recurso documentSetContent

Namespace: microsoft.graph

Representa o conteúdo padrão do conjunto de documentos SharePoint.
## <a name="properties"></a>Propriedades

| Propriedade  | Tipo    | Descrição|
|:---------------|:--------|:--------------------------------------------------|
| contentType    | microsoft.graph.contentTypeInfo | Informações de tipo de conteúdo do arquivo. |
| fileName      | cadeia de caracteres  | Nome do arquivo na pasta de recursos que deve ser adicionado como um conteúdo padrão ou um modelo no conjunto de documentos.|
| folderName         | cadeia de caracteres  | Nome da pasta no qual o arquivo será colocado quando um novo conjunto de documentos for criado na biblioteca.|

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
