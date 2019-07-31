---
author: JeremyKelley
description: O recurso DriveRecipient representa uma pessoa, um grupo ou outro destinatário com quem compartilhar usando a ação invite.
ms.date: 09/10/2017
title: DriveRecipient
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f86b79567b4148934f1c9624124026472fbb3395
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012706"
---
# <a name="driverecipient-resource"></a>Recurso DriveRecipient

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **DriveRecipient** representa uma pessoa, um grupo ou outro destinatário com quem compartilhar usando a ação [invite](../api/driveitem-invite.md).

## <a name="json-representation"></a>Representação JSON

<!-- { 
  "blockType": "resource", 
  "@odata.type": "microsoft.graph.driveRecipient", 
  "optionalProperties": ["alias", "objectId", "email"] } -->
```json
{
  "email": "string",
  "alias": "string",
  "objectId": "string",
}
```

## <a name="properties"></a>Propriedades
O recurso de destinatários possui essas propriedades.

| Nome da propriedade | Tipo   | Descrição                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| email         | Cadeia de caracteres | O endereço de email do destinatário, se este tiver um endereço de email associado.                  |
| alias         | String | O alias do objeto do domínio, para casos em que um endereço de email está indisponível (por exemplo, grupos de segurança). |
| objectId      | Cadeia de caracteres | O identificador exclusivo para o destinatário no diretório.                                               |

## <a name="remarks"></a>Comentários

Ao usar [invite](../api/driveitem-invite.md) para adicionar permissões, DriveRecipient pode especificar **email**, **alias** ou **objectId**. É necessário somente um desses valores.

<!--
{
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients",
  "suppressions": []
}
-->
