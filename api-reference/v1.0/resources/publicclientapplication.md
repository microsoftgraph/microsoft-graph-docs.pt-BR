---
title: Tipo de recurso publicClientApplication
description: Especifica configurações para aplicativos não Web ou Api da Web. (por exemplo, celular ou outro cliente público, como um aplicativo instalado em execução em um dispositivo desktop)
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: b8172eb64c1f54e33f8b5775a9234a7a30a42b641b68dd328c2fef5355fb9688
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54228988"
---
# <a name="publicclientapplication-resource-type"></a>Tipo de recurso publicClientApplication

Namespace: microsoft.graph

Especifica configurações para aplicativos não web ou API não web (por exemplo, clientes públicos móveis ou outros, como um aplicativo instalado em execução em um dispositivo de área de trabalho).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|redirectUris|String collection| Especifica as URLs para as quais os tokens de usuário são enviados para entrar ou as URIs de redirecionamento para as quais os códigos de autorização do OAuth 2.0 e tokens de acesso são enviados. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.publicClientApplication"
}-->

```json
{
  "redirectUris": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "installedClient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

