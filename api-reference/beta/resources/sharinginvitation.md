---
author: JeremyKelley
description: O recurso SharingInvitation transforma itens de dados relacionados a convite em uma única estrutura.
ms.date: 09/10/2017
title: SharingInvitation
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: db2214132dcbecdfb8b8689bdb3d5547a13be2ab
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723274"
---
# <a name="sharinginvitation-resource-type"></a>Tipo de recurso SharingInvitation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O **recurso SharingInvitation** transforma itens de dados relacionados a convite em uma única estrutura.

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

| Propriedade       | Tipo                          | Descrição                                                                                                                   |
| :------------- | :---------------------------- | :---------------------------------------------------------------------------------------------------------------------------- |
| email          | Cadeia de caracteres                        | O endereço de email fornecido para o destinatário do convite de compartilhamento. Somente leitura.                                            |
| invitedBy      | [identitySet](identityset.md) | Fornece informações sobre quem enviou o convite que criou essa permissão, se essas informações estiverem disponíveis. Somente leitura. |
| signInRequired | Booliano                       | Se `true`, o destinatário do convite precisa entrar para acessar o item compartilhado. Somente leitura.                     |

## <a name="remarks"></a>Comentários

Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
