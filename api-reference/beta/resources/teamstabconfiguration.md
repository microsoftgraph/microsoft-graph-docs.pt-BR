---
title: tipo de recurso teamsTabConfiguration (tipo aberto)
description: As configurações que determinam o conteúdo de uma guia.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ec8192d486194132e71f8f1fff493e081f8192e3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519838"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a>tipo de recurso teamsTabConfiguration (tipo aberto)

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

As configurações que determinam o conteúdo de uma [guia](teamstab.md). Quando uma guia é configurada de forma interativa, essa informação é definida pelo aplicativo de provedor de guias.
Além das propriedades abaixo, alguns aplicativos de provedor de guia especificam Propriedades personalizadas adicionais.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|-|-|-|
|  entityId   |   string |  Identificador da entidade hospedada pelo provedor de guias.     |
|  contentUrl |   string |  URL usada para renderizar o conteúdo da guia no Microsoft Teams. Obrigatório.    |
|  removeUrl  |   string |  URL chamada pelo cliente Teams quando uma guia é removida usando o cliente Teams.     |
|  websiteUrl |   string |  URL para mostrar o conteúdo de guia fora do teams.     |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTabConfiguration"
}-->

```json
{
   "entityId": "string",
   "contentUrl": "string (HTTPS Url)",
   "websiteUrl": "string (HTTPS Url)",
   "removeUrl": "string (HTTPS Url)"  
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsTabConfiguration complex type (Open Type)",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
