---
title: Tipo de recurso publicClientApplication
description: Especifica configurações para aplicativos não Web ou Api da Web. (por exemplo, celular ou outro cliente público, como um aplicativo instalado em execução em um dispositivo desktop)
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: a5769d2fcbc01114b9a79a6eb3bad21c65566663
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067049"
---
# <a name="publicclientapplication-resource-type"></a>Tipo de recurso publicClientApplication

Namespace: microsoft.graph

Especifica configurações para aplicativos não web ou API não web (por exemplo, clientes públicos móveis ou outros, como um aplicativo instalado em execução em um dispositivo de área de trabalho).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|redirectUris|Coleção String| Especifica as URLs para as quais os tokens de usuário são enviados para entrar ou as URIs de redirecionamento para as quais os códigos de autorização do OAuth 2.0 e tokens de acesso são enviados. |

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

