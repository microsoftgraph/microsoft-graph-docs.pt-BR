---
author: swapnil1993
title: Tipo de recurso documentSetContent
description: O recurso documentSetContent contém metadados sobre um arquivo presente no local de conteúdo padrão de um conteúdo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 5926e80c6c507591942009ae00ea199fdccfdca0
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696502"
---
# <a name="documentsetcontent-resource-type"></a>Tipo de recurso documentSetContent

Namespace: microsoft.graph

Representa o conteúdo padrão do conjunto de documentos SharePoint.
## <a name="properties"></a>Propriedades

| Nome da propriedade  | Tipo    | Descrição|
|:---------------|:--------|:--------------------------------------------------|
| contentType    | microsoft.graph.contentTypeInfo | Informações de tipo de conteúdo do arquivo. |
| fileName      | string  | Nome do arquivo na pasta de recursos que deve ser adicionado como um conteúdo padrão ou um modelo no conjunto de documentos.|
| folderName         | string  | Nome da pasta no qual o arquivo será colocado quando um novo conjunto de documentos for criado na biblioteca.|

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