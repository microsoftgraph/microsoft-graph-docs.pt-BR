---
author: JeremyKelley
ms.date: 09/10/2017
title: SharingInvitation
ms.localizationpriority: medium
description: O recurso SharingInvitation transforma itens de dados relacionados a convite em uma única estrutura.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 064c687b761872f587f8fe992d320c204dc260f9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59032255"
---
# <a name="sharinginvitation-resource-type"></a>Tipo de recurso SharingInvitation

Namespace: microsoft.graph

O **recurso SharingInvitation** transforma itens de dados relacionados a convite em uma única estrutura.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sharingInvitation"
}-->

```json
{
  "email": "string",
  "invitedBy": {"@odata.type": "microsoft.graph.identitySet" },
  "signInRequired": true
}
```

## <a name="properties"></a>Propriedades

| Nome da propriedade  | Tipo            | Descrição
|:---------------|:----------------|:------------------------------------------
| email          | Cadeia de caracteres          | O endereço de email fornecido para o destinatário do convite de compartilhamento. Somente leitura.
| invitedBy      | [identitySet][] | Fornece informações sobre quem enviou o convite que criou essa permissão, se essas informações estiverem disponíveis. Somente leitura.
| signInRequired | Booliano         | Se `true`, o destinatário do convite precisa entrar para acessar o item compartilhado. Somente leitura.

## <a name="remarks"></a>Comentários

Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).

[DriveItem]: driveitem.md
[IdentitySet]: identityset.md

<!-- {
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath&quot;: &quot;Facets/SharingInvitation"
} -->

