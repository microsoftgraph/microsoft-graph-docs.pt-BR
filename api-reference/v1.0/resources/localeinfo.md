---
title: Tipo de recurso localeInfo
description: Informações sobre a localidade, incluindo o idioma preferencial e o país/região do usuário conectado.
ms.localizationpriority: medium
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 6156caa38ce645705c4fe73bf82ca3bffc92bb45
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134728"
---
# <a name="localeinfo-resource-type"></a>Tipo de recurso localeInfo

Namespace: microsoft.graph

Informações sobre a localidade, incluindo o idioma preferencial e o país/região do usuário conectado.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|localidade|cadeia de caracteres|Uma representação da localidade do usuário, que inclui o idioma preferencial do usuário e o país/região. Por exemplo, "pt-br". O componente do idioma segue um padrão de código de duas letras, conforme definido na [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm), e o componente do país segue um padrão de código de duas letras, conforme definido na [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm).|
|displayName|cadeia de caracteres|Um nome que representa a localidade do usuário em seu idioma natural, por exemplo, "Português (Brasil)".|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.localeInfo"
}-->

```json
{
  "locale": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "localeInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

