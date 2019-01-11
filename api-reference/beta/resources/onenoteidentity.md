---
title: tipo de recurso de oneNoteIdentity
description: '**Suporte em breve**'
localization_priority: Normal
ms.openlocfilehash: 80d0719bd2770b715902b5c600fe65012e0064d9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883885"
---
# <a name="onenoteidentity-resource-type"></a><span data-ttu-id="dbdd5-103">tipo de recurso de oneNoteIdentity</span><span class="sxs-lookup"><span data-stu-id="dbdd5-103">oneNoteIdentity resource type</span></span>

> <span data-ttu-id="dbdd5-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="dbdd5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dbdd5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dbdd5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dbdd5-106">**Suporte em breve**</span><span class="sxs-lookup"><span data-stu-id="dbdd5-106">**Support coming soon**</span></span>

<span data-ttu-id="dbdd5-107">O tipo de OneNoteIdentity representa uma identidade de um _usuário_.</span><span class="sxs-lookup"><span data-stu-id="dbdd5-107">The OneNoteIdentity type represents an identity of a _user_.</span></span>

<span data-ttu-id="dbdd5-108">No futuro, esse tipo de será mesclado com [identidade](identity.md)</span><span class="sxs-lookup"><span data-stu-id="dbdd5-108">In future, this type will be merged with [Identity](identity.md)</span></span>


## <a name="json-representation"></a><span data-ttu-id="dbdd5-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dbdd5-109">JSON representation</span></span>

<span data-ttu-id="dbdd5-110">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dbdd5-110">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteidentity"
}-->

```json
{
  "displayName": "string",
  "id": "string"
}

```
## <a name="properties"></a><span data-ttu-id="dbdd5-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dbdd5-111">Properties</span></span>
| <span data-ttu-id="dbdd5-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dbdd5-112">Property</span></span>     | <span data-ttu-id="dbdd5-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbdd5-113">Type</span></span>   |<span data-ttu-id="dbdd5-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbdd5-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dbdd5-115">displayName</span><span class="sxs-lookup"><span data-stu-id="dbdd5-115">displayName</span></span>|<span data-ttu-id="dbdd5-116">string</span><span class="sxs-lookup"><span data-stu-id="dbdd5-116">string</span></span>|<span data-ttu-id="dbdd5-117">Nome para exibição da identidade.</span><span class="sxs-lookup"><span data-stu-id="dbdd5-117">The identity's display name.</span></span>|
|<span data-ttu-id="dbdd5-118">id</span><span class="sxs-lookup"><span data-stu-id="dbdd5-118">id</span></span>|<span data-ttu-id="dbdd5-119">string</span><span class="sxs-lookup"><span data-stu-id="dbdd5-119">string</span></span>|<span data-ttu-id="dbdd5-120">Identificador exclusivo da identidade.</span><span class="sxs-lookup"><span data-stu-id="dbdd5-120">Unique identifier for the identity.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oneNoteIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
