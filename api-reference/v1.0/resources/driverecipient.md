---
author: JeremyKelley
ms.date: 09/10/2017
title: DriveRecipient
ms.localizationpriority: medium
ms.prod: sharepoint
description: O recurso driveRecipient representa uma pessoa, grupo ou outro destinatário para compartilhar usando a ação de convite.
doc_type: resourcePageType
ms.openlocfilehash: 4788b02e0ec52965475745a4e234beaaf6b2910e
ms.sourcegitcommit: 94dc71a6d4fbdc46f2681a1add13416bc9b4a6e9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/05/2021
ms.locfileid: "60115386"
---
# <a name="driverecipient-resource"></a>recurso driveRecipient

Namespace: microsoft.graph

Representa uma pessoa, grupo ou outro destinatário para compartilhar um item de unidade usando a [ação de](../api/driveitem-invite.md) convite.

Ao usar [o convite](../api/driveitem-invite.md) para adicionar permissões, o **objeto driveRecipient** especificaria o **email**, **alias** ou **objectId** do destinatário.
Somente um desses valores é necessário; vários valores não são aceitos.

## <a name="properties"></a>Propriedades
O recurso de destinatários possui essas propriedades.

| Nome da propriedade | Tipo   | Descrição                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| email         | Cadeia de caracteres | O endereço de email do destinatário, se este tiver um endereço de email associado.                  |
| alias         | Cadeia de caracteres | O alias do objeto do domínio, para casos em que um endereço de email está indisponível (por exemplo, grupos de segurança). |
| objectId      | Cadeia de caracteres | O identificador exclusivo para o destinatário no diretório.                                               |

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

<!-- {
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients"
} -->

