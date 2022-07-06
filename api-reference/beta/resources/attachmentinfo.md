---
title: Tipo de recurso attachmentInfo
description: Representa os atributos de um anexo.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: af43c3e53dd41a28f9e123912bf6153679500f00
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645587"
---
# <a name="attachmentinfo-resource-type"></a>Tipo de recurso attachmentInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os atributos de um anexo.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Attachmenttype|Attachmenttype|O tipo de anexo. Os valores possíveis são: `file`, `item`, `reference`. Obrigatório.|
|contentType|String|A natureza dos dados no anexo. Opcional.|
|nome|Cadeia de caracteres|O nome de exibição do anexo. Isso pode ser uma cadeia de caracteres descritiva e não precisa ser o nome de arquivo real. Obrigatório.|
|size|Int64|O comprimento do anexo em bytes. Obrigatório.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.attachmentInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attachmentInfo",
  "attachmentType": "String",
  "contentType": "String",
  "name": "String",
  "size": "Int64"
}
```

