---
title: tipo de recurso de meetingCapability
description: Contém os recursos de uma reunião
ms.openlocfilehash: 438193d08ab5542f07d4cbf61704520d81433e50
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036414"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="15ac3-103">tipo de recurso de meetingCapability</span><span class="sxs-lookup"><span data-stu-id="15ac3-103">meetingCapability resource type</span></span>

> <span data-ttu-id="15ac3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="15ac3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15ac3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="15ac3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="15ac3-106">Contém os recursos de uma reunião</span><span class="sxs-lookup"><span data-stu-id="15ac3-106">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="15ac3-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="15ac3-107">Properties</span></span>

| <span data-ttu-id="15ac3-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="15ac3-108">Property</span></span>       | <span data-ttu-id="15ac3-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="15ac3-109">Type</span></span>    | <span data-ttu-id="15ac3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="15ac3-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="15ac3-111">allowAnonymousUsersToDialOut</span><span class="sxs-lookup"><span data-stu-id="15ac3-111">allowAnonymousUsersToDialOut</span></span> | <span data-ttu-id="15ac3-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="15ac3-112">Boolean</span></span> | <span data-ttu-id="15ac3-113">Indica se os usuários anônimos discagem é permitida em uma reunião.</span><span class="sxs-lookup"><span data-stu-id="15ac3-113">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="15ac3-114">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="15ac3-114">autoAdmittedUsers</span></span> | <span data-ttu-id="15ac3-115">String</span><span class="sxs-lookup"><span data-stu-id="15ac3-115">String</span></span> | <span data-ttu-id="15ac3-116">Os valores possíveis são: `everyoneInCompany` e `everyone`.</span><span class="sxs-lookup"><span data-stu-id="15ac3-116">Possible values are: `everyoneInCompany`, `everyone`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="15ac3-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="15ac3-117">JSON representation</span></span>

<span data-ttu-id="15ac3-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="15ac3-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingCapability"
}-->
```json
{
  "allowAnonymousUsersToDialOut": true,
  "autoAdmittedUsers": "everyoneInCompany | everyone"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingCapability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
