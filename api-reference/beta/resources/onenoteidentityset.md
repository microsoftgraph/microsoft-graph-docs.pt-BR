---
title: tipo de recurso de oneNoteIdentitySet
description: '**Suporte em breve**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 9043b08a8586bcc9a0043a2fde13f0d5d9eea4a9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947166"
---
# <a name="onenoteidentityset-resource-type"></a>tipo de recurso de oneNoteIdentitySet

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

**Suporte em breve**

O tipo de OneNoteIdentitySet é uma coleção com chave de objetos [OneNoteIdentity](onenoteidentity.md) .
Ele é usado para representar um conjunto de identidades associado a vários eventos para um _Bloco de anotações_, _seção_ ou da _página_, como _criado por_ ou _modificado pela última vez_. 
 
Atualmente, ele contém um único _**usuário**_ de chave.  No futuro, chaves, como o dispositivo ou aplicativo para alterar o item podem ser adicionadas.

No futuro, esse tipo de será mesclado com [IdentitySet](identityset.md)

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteidentityset"
}-->

```json
{
  "user": {"@odata.type": "microsoft.graph.oneNoteIdentity"}
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|user|[oneNoteIdentity](onenoteidentity.md)|Um recurso de OneNoteIdentity que representa um usuário.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oneNoteIdentitySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
