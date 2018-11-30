---
title: Tipo de recurso emailAddress
description: Representa o nome e o endereço SMTP de uma instância da entidade, por exemplo, uma mensagem destinatário ou calendário proprietário.
ms.openlocfilehash: f607fe4ce01b9a3c3f5e7af5aa1638fef3840177
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034176"
---
# <a name="emailaddress-resource-type"></a>Tipo de recurso emailAddress

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa o nome e o endereço SMTP de uma instância da entidade, por exemplo, uma mensagem destinatário ou calendário proprietário.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|address|Cadeia de caracteres|O endereço de email de uma instância da entidade.|
|name|String|O nome de exibição de uma instância da entidade.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailAddress"
}-->

```json
{
  "address": "string",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
