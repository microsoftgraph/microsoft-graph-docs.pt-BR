---
title: Tipo de recurso publicClientApplication
description: Especifica configurações para não Web App ou Api da Web. (por exemplo, celular ou outro cliente público, como um aplicativo instalado em execução em um dispositivo de desktop)
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: a15f0ea159ab12403186465783200a9e374562bc
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137512"
---
# <a name="publicclientapplication-resource-type"></a>Tipo de recurso publicClientApplication

Namespace: microsoft.graph

Especifica configurações para aplicativo não Web ou API não Web (por exemplo, dispositivos móveis ou outros clientes públicos, como um aplicativo instalado em execução em um dispositivo de desktop).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|redirectUris|String collection| Especifica as URLs para onde os tokens de usuário são enviados para entrada ou os URIs de redirecionamento para os quais os códigos de autorização e tokens de acesso do OAuth 2.0 são enviados. |

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

