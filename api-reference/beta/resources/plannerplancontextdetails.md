---
title: Tipo de recurso plannerPlanContextDetails
description: O **recurso plannerPlanContextDetails** contém informações adicionais sobre um plannerPlanContext.
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: bdb65fab6aecf9c61e066c7e80e9226220c3491c
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63367920"
---
# <a name="plannerplancontextdetails-resource-type"></a>Tipo de recurso plannerPlanContextDetails

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O **recurso plannerPlanContextDetails** contém informações adicionais sobre um [plannerPlanContext](plannerplancontext.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|customLinkText|String|Anulável. Especifica o texto a ser usado em uma experiência do usuário para exibir um link do [plannerPlanContext associado](plannerplancontext.md). Se nulo, os aplicativos devem exibir o link com um texto personalizado com base na **propriedade displayLinkType** .|
|displayLinkType|plannerPlanContextType|Especifica como um aplicativo deve exibir o link para o **plannerPlanContext associado**. Os aplicativos podem optar por fornecer texto, descrição, ícones ou outras experiências personalizadas com base no tipo do link. Os valores possíveis são: `teamsTab`, `sharePointPage`, `meetingNotes`, `other`, `unknownFutureValue`.|
|url|Cadeia de caracteres|URL da experiência do usuário representada pelo **plannerPlanContext associado**. |
|estado|plannerContextState| Indica o estado do **plannerPlanContext associado**. |

### <a name="plannercontextstate-values"></a>valores plannerContextState

|Valor              |Descrição|
|:------------------|:----------------------------------------------------------------------|
|active             | O contexto não tem problemas.                                          |
|delinked           | Um **plannerPlanContext** anteriormente vinculado não está mais vinculado ao plano. |
|unknownFutureValue | Valor de sentinela de enumeração evolvável. Não usar.                     |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.plannerPlanContextDetails"
}-->

```json
{
  "url": "string",
  "customLinkText": "string",
  "displayLinkType": "string",
  "state": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


