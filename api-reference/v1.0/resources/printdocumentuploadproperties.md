---
author: nilakhan
description: Representa informações para upload de documento de impressão
title: Tipo de recurso printDocumentUploadProperties
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: cloud-printing
ms.openlocfilehash: 855f9fc66d7dc35c7fddc0904e76788e280fcdba
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60944995"
---
# <a name="printdocumentuploadproperties-resource-type"></a>Tipo de recurso printDocumentUploadProperties

Namespace: microsoft.graph

Descreve o documento que está sendo carregado

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|contentType|String|Tipo de conteúdo do documento (MIME).|
|documentName|Cadeia de caracteres|O nome do documento.|
|size|Int64|O tamanho do documento em bytes.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printDocumentUploadProperties"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printDocumentUploadProperties",
  "contentType": "String",
  "documentName": "String",
  "size": "Integer"
}
```

