---
title: Tipo de recurso sharingDetail
description: 'Tipo complexo que contém propriedades de itens compartilhados. '
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: c34d0bf2d35f51ecae7268ef754a228dc226664a
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473889"
---
# <a name="sharingdetail-resource-type"></a><span data-ttu-id="a8709-103">Tipo de recurso sharingDetail</span><span class="sxs-lookup"><span data-stu-id="a8709-103">sharingDetail resource type</span></span>

<span data-ttu-id="a8709-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8709-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8709-105">Tipo complexo que contém propriedades de [itens sharedInsight.](insights-shared.md)</span><span class="sxs-lookup"><span data-stu-id="a8709-105">Complex type containing properties of [sharedInsight](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="a8709-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a8709-106">JSON representation</span></span>
<span data-ttu-id="a8709-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="a8709-107">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sharingDetail"
}-->
```json
{
  "sharedDateTime": "dateTimeOffset",
  "sharingSubject": "string",
  "sharingType": "string",
  "sharedBy": "insightIdentity",
  "sharingReference": "resourceReference"
}
```

## <a name="properties"></a><span data-ttu-id="a8709-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a8709-108">Properties</span></span>

| <span data-ttu-id="a8709-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8709-109">Property</span></span>              | <span data-ttu-id="a8709-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8709-110">Type</span></span>          | <span data-ttu-id="a8709-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8709-111">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="a8709-112">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8709-112">sharedDateTime</span></span>        | <span data-ttu-id="a8709-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8709-113">DateTimeOffset</span></span>| <span data-ttu-id="a8709-114">A data e a hora em que o arquivo foi compartilhado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="a8709-114">The date and time the file was last shared.</span></span> <span data-ttu-id="a8709-115">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="a8709-115">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a8709-116">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="a8709-116">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="a8709-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a8709-117">Read-only.</span></span>  |
| <span data-ttu-id="a8709-118">sharingSubject</span><span class="sxs-lookup"><span data-stu-id="a8709-118">sharingSubject</span></span>        | <span data-ttu-id="a8709-119">String</span><span class="sxs-lookup"><span data-stu-id="a8709-119">String</span></span>          | <span data-ttu-id="a8709-120">O assunto com o qual o documento foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="a8709-120">The subject with which the document was shared.</span></span> |
| <span data-ttu-id="a8709-121">sharingType</span><span class="sxs-lookup"><span data-stu-id="a8709-121">sharingType</span></span>             | <span data-ttu-id="a8709-122">String</span><span class="sxs-lookup"><span data-stu-id="a8709-122">String</span></span>        | <span data-ttu-id="a8709-123">Determina como o documento foi compartilhado, pode ser por um "Link", "Attachment", "Group", "Site".</span><span class="sxs-lookup"><span data-stu-id="a8709-123">Determines the way the document was shared, can be by a "Link", "Attachment", "Group", "Site".</span></span>     |
| <span data-ttu-id="a8709-124">sharedBy</span><span class="sxs-lookup"><span data-stu-id="a8709-124">sharedBy</span></span>                | [<span data-ttu-id="a8709-125">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="a8709-125">insightIdentity</span></span>](insights-insightidentity.md)      | <span data-ttu-id="a8709-126">O usuário que compartilhou o documento.</span><span class="sxs-lookup"><span data-stu-id="a8709-126">The user who shared the document.</span></span>  |
| <span data-ttu-id="a8709-127">sharingReference</span><span class="sxs-lookup"><span data-stu-id="a8709-127">sharingReference</span></span>        | [<span data-ttu-id="a8709-128">resourceReference</span><span class="sxs-lookup"><span data-stu-id="a8709-128">resourceReference</span></span>](insights-resourcereference.md)      |  |


