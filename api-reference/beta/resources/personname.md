---
title: tipo de recurso PersonName
description: tipo de recurso PersonName
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: e4927ba05443d4b54eaac3f54b7e0d3a8cd62159
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227683"
---
# <a name="personname-resource-type"></a>tipo de recurso PersonName

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as informações de nome estendidas fornecidas pelo usuário ou que elas associaram à conta.

Herda de [Myfacet](itemfacet.md).

## <a name="methods"></a>Métodos

| Método                                     | Tipo de retorno                 | Descrição                                             |
|:-------------------------------------------|:----------------------------|:--------------------------------------------------------|
| [Obter PersonName](../api/personname-get.md) | [personName](personname.md) | Leia as propriedades e as relações do objeto PersonName. |
| [Update](../api/personname-update.md)      | [personName](personname.md) | Objeto Update PersonName.                               |
| [Delete](../api/personname-delete.md)      | None                        | Exclua o objeto PersonName.                               |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo                              | Descrição                                                                                                  |
|:-------------|:----------------------------------|:-------------------------------------------------------------------------------------------------------------|
|displayName   |Cadeia de caracteres                             | Fornece uma renderização ordenada de firstName e lastName, dependendo da localidade do usuário ou de seu dispositivo. |
|primeiro         |String                             | Nome do usuário.                                                                                      |
|initials      |String                             | Iniciais do usuário.                                                                                        |
|languageTag   |String                             | Contém o nome do idioma (en-US, no-NB, en-AU) após o formato BCP47 da IETF.                        |
|durar          |String                             | Sobrenome do usuário.                                                                                       |
|Virgem        |String                             | Nome de solteira do usuário.                                                                                     |
|middleware        |String                             | Middlie nome do usuário.                                                                                    |
|apelido      |String                             | Apelido do usuário.                                                                                        |
|pronúncia |[yomiPersonName](yomipersonname.md)| Orientações sobre como pronunciar o nome dos usuários.                                                                 |
|sufixo        |String                             | Designadores usados após o nome dos usuários (por exemplo: PhD).                                                             |
|title         |String                             | Honorifics usado para prefixar um nome de usuário (por exemplo: Dr, Sir, Madam, Sra.)                                            |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personName",
  "baseType": ""
}-->

```json
{
  "displayName": "String",
  "first": "String",
  "initials": "String",
  "languageTag": "String",
  "last": "String",
  "maiden": "String",
  "middle": "String",
  "nickname": "String",
  "pronunciation": {"@odata.type": "microsoft.graph.yomiPersonName"},
  "suffix": "String",
  "title": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personName resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->