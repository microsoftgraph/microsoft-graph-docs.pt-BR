---
title: tipo de recurso freeBusyError
description: Representa informações de erro da tentativa de obter a disponibilidade de um usuário, lista de distribuição ou recurso.
localization_priority: Normal
ms.openlocfilehash: e2c755b51e72adf3ff4efa4de5c9438e70d701e1
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869334"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="a7c94-103">tipo de recurso freeBusyError</span><span class="sxs-lookup"><span data-stu-id="a7c94-103">freeBusyError resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="a7c94-104">Representa informações de erro da tentativa de obter a disponibilidade de um usuário, lista de distribuição ou recurso.</span><span class="sxs-lookup"><span data-stu-id="a7c94-104">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="a7c94-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a7c94-105">Properties</span></span>
| <span data-ttu-id="a7c94-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a7c94-106">Property</span></span>     | <span data-ttu-id="a7c94-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7c94-107">Type</span></span>   |<span data-ttu-id="a7c94-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7c94-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a7c94-109">mensagem</span><span class="sxs-lookup"><span data-stu-id="a7c94-109">message</span></span> |<span data-ttu-id="a7c94-110">String</span><span class="sxs-lookup"><span data-stu-id="a7c94-110">String</span></span> |<span data-ttu-id="a7c94-111">Descreve o erro.</span><span class="sxs-lookup"><span data-stu-id="a7c94-111">Describes the error.</span></span> |
|<span data-ttu-id="a7c94-112">responseCode</span><span class="sxs-lookup"><span data-stu-id="a7c94-112">responseCode</span></span> |<span data-ttu-id="a7c94-113">String</span><span class="sxs-lookup"><span data-stu-id="a7c94-113">String</span></span> |<span data-ttu-id="a7c94-114">O código de resposta da consulta para a disponibilidade do usuário, lista de distribuição ou recurso.</span><span class="sxs-lookup"><span data-stu-id="a7c94-114">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="a7c94-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a7c94-115">JSON representation</span></span>

<span data-ttu-id="a7c94-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a7c94-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.freeBusyError"
}-->

```json
{
  "message": "String",
  "responseCode": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "freeBusyError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/freebusyerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
