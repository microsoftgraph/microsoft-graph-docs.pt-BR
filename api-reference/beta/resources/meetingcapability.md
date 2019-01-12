---
title: tipo de recurso de meetingCapability
description: Contém os recursos de uma reunião
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 342d264c1f4c670d159c15558c78cc896d4a9487
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931360"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="1bbd8-103">tipo de recurso de meetingCapability</span><span class="sxs-lookup"><span data-stu-id="1bbd8-103">meetingCapability resource type</span></span>

> <span data-ttu-id="1bbd8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1bbd8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1bbd8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1bbd8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1bbd8-106">Contém os recursos de uma reunião</span><span class="sxs-lookup"><span data-stu-id="1bbd8-106">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="1bbd8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1bbd8-107">Properties</span></span>

| <span data-ttu-id="1bbd8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1bbd8-108">Property</span></span>                          | <span data-ttu-id="1bbd8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1bbd8-109">Type</span></span>    | <span data-ttu-id="1bbd8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bbd8-110">Description</span></span>                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| <span data-ttu-id="1bbd8-111">allowAnonymousUsersToDialOut</span><span class="sxs-lookup"><span data-stu-id="1bbd8-111">allowAnonymousUsersToDialOut</span></span>      | <span data-ttu-id="1bbd8-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="1bbd8-112">Boolean</span></span> | <span data-ttu-id="1bbd8-113">Indica se os usuários anônimos discagem é permitida em uma reunião.</span><span class="sxs-lookup"><span data-stu-id="1bbd8-113">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="1bbd8-114">allowAnonymousUsersToStartMeeting</span><span class="sxs-lookup"><span data-stu-id="1bbd8-114">allowAnonymousUsersToStartMeeting</span></span> | <span data-ttu-id="1bbd8-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="1bbd8-115">Boolean</span></span> | <span data-ttu-id="1bbd8-116">Indica se os usuários anônimos poderão iniciar uma reunião.</span><span class="sxs-lookup"><span data-stu-id="1bbd8-116">Indicates whether anonymous users are allowed to start a meeting.</span></span>  |
| <span data-ttu-id="1bbd8-117">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="1bbd8-117">autoAdmittedUsers</span></span>                 | <span data-ttu-id="1bbd8-118">String</span><span class="sxs-lookup"><span data-stu-id="1bbd8-118">String</span></span>  | <span data-ttu-id="1bbd8-119">Os valores possíveis são: `everyoneInCompany` e `everyone`.</span><span class="sxs-lookup"><span data-stu-id="1bbd8-119">Possible values are: `everyoneInCompany`, `everyone`.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="1bbd8-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1bbd8-120">JSON representation</span></span>

<span data-ttu-id="1bbd8-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1bbd8-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingCapability"
}-->
```json
{
  "allowAnonymousUsersToDialOut": true,
  "allowAnonymousUsersToStartMeeting": true,
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
