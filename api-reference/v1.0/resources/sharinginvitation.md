---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingInvitation
localization_priority: Normal
description: O recurso SharingInvitation agrupa itens de dados relacionados a convites em uma única estrutura.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 011402b40b601642a048b91e3b3f66de0792aaf2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034241"
---
# <a name="sharinginvitation-resource-type"></a>Tipo de recurso SharingInvitation

O recurso **SharingInvitation** agrupa itens de dados relacionados a convites em uma única estrutura.

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

| Nome da Propriedade  | Tipo            | Descrição
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
  "tocPath": "Facets/SharingInvitation"
} -->
