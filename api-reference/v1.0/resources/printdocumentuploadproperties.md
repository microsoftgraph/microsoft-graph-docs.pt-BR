---
author: nilakhan
description: Representa informações para upload de documento de impressão
title: Tipo de recurso printDocumentUploadProperties
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-printing
ms.openlocfilehash: e877901b842670e09cb283b40613a1185aabaafe
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516912"
---
# <a name="printdocumentuploadproperties-resource-type"></a>Tipo de recurso printDocumentUploadProperties

Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

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

