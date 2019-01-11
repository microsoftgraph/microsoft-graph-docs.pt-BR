---
title: tipo de recurso de educationPowerPointResource
description: 'Uma subclasse de educationResource. Esse é um recurso do PowerPoint. O arquivo do PowerPoint que deve ser carregado no diretório **fileResource** associado a '
localization_priority: Normal
ms.openlocfilehash: 763a529e97b12c93d8f10aa6855c20818c02da67
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845455"
---
# <a name="educationpowerpointresource-resource-type"></a>tipo de recurso de educationPowerPointResource

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Uma subclasse de [educationResource](educationresource.md). Esse é um recurso do PowerPoint. O arquivo do PowerPoint deve ser carregado no diretório **fileResource** associado a atribuição ou o envio.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|fileUrl|Cadeia de caracteres|Local do arquivo no disco.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPowerPointResource"
}-->

```json
{
  "fileUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationPowerPointResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
