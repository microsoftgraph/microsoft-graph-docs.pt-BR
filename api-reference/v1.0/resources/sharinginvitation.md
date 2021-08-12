---
author: JeremyKelley
ms.date: 09/10/2017
title: SharingInvitation
localization_priority: Normal
description: O recurso SharingInvitation transforma itens de dados relacionados a convite em uma única estrutura.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: eaf917ccdd64a50dab9cdf6f2ed477716c18a0185be03812793d115247e17e93
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54134935"
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

