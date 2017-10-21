---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingInvitation
ms.openlocfilehash: 75fa8212f77873b86748f6d8f63c8e62c8d6a0ca
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="sharinginvitation-resource-type"></a>Tipo de recurso SharingInvitation

O recurso **SharingInvitation** agrupa itens de dados relacionados ao convite em uma única estrutura.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

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

| Nome da propriedade  | Tipo                          | Descrição                                                                                                                   |
|:---------------|:------------------------------|:------------------------------------------------------------------------------------------------------------------------------|
| email          | String                        | O endereço de email fornecido para o destinatário do convite de compartilhamento. Somente leitura.                                          |
| invitedBy      | [identitySet](identityset.md) | Fornece informações sobre quem enviou o convite que criou essa permissão, se essas informações estiverem disponíveis. Somente leitura. |
| signInRequired | Booliano                       | Se `true`, o destinatário do convite precisa entrar para acessar o item compartilhado. Somente leitura.                     |

## <a name="remarks"></a>Comentários 

Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).


<!-- {
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SharingInvitation"
} -->
