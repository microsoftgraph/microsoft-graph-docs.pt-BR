---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveRecipient
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 85def7dd812d2046e02f814cf63e9f82b28d2781
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919684"
---
# <a name="driverecipient-resource"></a>Recurso DriveRecipient

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

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
| alias         | Cadeia de caracteres | O alias do objeto do domínio, para casos em que um endereço de email está indisponível (por exemplo, grupos de segurança). |
| objectId      | Cadeia de caracteres | O identificador exclusivo para o destinatário no diretório.                                               |

## <a name="remarks"></a>Comentários

Ao usar [invite](../api/driveitem-invite.md) para adicionar permissões, DriveRecipient pode especificar **email**, **alias** ou **objectId**. É necessário somente um desses valores.

<!-- {
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients"
} -->
