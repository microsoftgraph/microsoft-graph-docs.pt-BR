---
author: JeremyKelley
description: O recurso driveRecipient representa uma pessoa, grupo ou outro destinatário para compartilhar usando a ação de convite.
ms.date: 09/10/2017
title: DriveRecipient
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 1b7b666e520af98fd6fae193b770357a7813504e
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63722574"
---
# <a name="driverecipient-resource"></a>recurso driveRecipient

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma pessoa, grupo ou outro destinatário para compartilhar um item de unidade usando a [ação de](../api/driveitem-invite.md) convite.

Ao usar [o convite](../api/driveitem-invite.md) para adicionar permissões, o **objeto driveRecipient** pode especificar o **email**, **alias** ou **objectId** do destinatário.
Somente um desses valores é necessário; vários valores não são aceitos.

## <a name="properties"></a>Propriedades

O recurso de destinatários possui essas propriedades.

| Propriedade | Tipo   | Descrição                                                                                             |
| :------- | :----- | :------------------------------------------------------------------------------------------------------ |
| email    | Cadeia de caracteres | O endereço de email do destinatário, se este tiver um endereço de email associado.                  |
| alias    | Cadeia de caracteres | O alias do objeto do domínio, para casos em que um endereço de email está indisponível (por exemplo, grupos de segurança). |
| objectId | Cadeia de caracteres | O identificador exclusivo para o destinatário no diretório.                                               |

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
