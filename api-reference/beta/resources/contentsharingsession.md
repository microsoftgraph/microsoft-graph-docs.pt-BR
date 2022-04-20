---
title: Tipo de recurso contentSharingSession
description: Representa uma sessão de compartilhamento de conteúdo em uma chamada.
author: satyakonmsft
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5d642350b3fe5e6b1edf5e35dbc3cb5a1f677aea
ms.sourcegitcommit: 9bbcce5784a89768ece55a66e3651080d56e1e92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/19/2022
ms.locfileid: "64917824"
---
# <a name="contentsharingsession-resource-type"></a>Tipo de recurso contentSharingSession

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma sessão de compartilhamento de conteúdo em uma chamada.

## <a name="methods"></a>Métodos

| Método                                                             | Tipo de retorno                                                 | Descrição                                                                     |
|:-------------------------------------------------------------------|:------------------------------------------------------------|:--------------------------------------------------------------------------------|
| [Obter contentSharingSession](../api/contentsharingsession-get.md )                                     | [contentSharingSession](contentsharingsession.md)                                             | Recupere as propriedades de um **objeto contentSharingSession** .                                         |
| [Listar contentSharingSessions](../api/call-list-contentsharingsessions.md )              | [coleção contentSharingSession](contentsharingsession.md)                    | Recupere uma lista de **objetos contentSharingSession** em uma chamada.                                            |

## <a name="properties"></a>Propriedades

|Propriedade                 |Tipo                      |Descrição                                                                        |
|:---                     |:---                      |:---                                                                               |
| id                      | Cadeia de caracteres                   | Identificador exclusivo para a sessão de compartilhamento de conteúdo. Somente leitura. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.contentSharingSession"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.contentSharingSession",
  "id": "String(identifier)"
}
```
