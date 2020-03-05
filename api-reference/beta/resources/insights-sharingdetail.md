---
title: tipo de recurso sharingDetail
description: 'Tipo complexo contendo propriedades de itens compartilhados. '
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: e8216e08c4f7232c67c51fa8291ece63178472b3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42495596"
---
# <a name="sharingdetail-resource-type"></a><span data-ttu-id="887b4-103">tipo de recurso sharingDetail</span><span class="sxs-lookup"><span data-stu-id="887b4-103">sharingDetail resource type</span></span>

<span data-ttu-id="887b4-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="887b4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="887b4-105">Tipo complexo contendo propriedades de itens do [sharedInsight](insights-shared.md) .</span><span class="sxs-lookup"><span data-stu-id="887b4-105">Complex type containing properties of [sharedInsight](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="887b4-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="887b4-106">JSON representation</span></span>
<span data-ttu-id="887b4-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="887b4-107">Here is a JSON representation of the resource</span></span>
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
  "resourceReference": "resourceReference"
}
```

## <a name="properties"></a><span data-ttu-id="887b4-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="887b4-108">Properties</span></span>

| <span data-ttu-id="887b4-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="887b4-109">Property</span></span>              | <span data-ttu-id="887b4-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="887b4-110">Type</span></span>          | <span data-ttu-id="887b4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="887b4-111">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="887b4-112">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="887b4-112">sharedDateTime</span></span>        | <span data-ttu-id="887b4-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="887b4-113">DateTimeOffset</span></span>| <span data-ttu-id="887b4-114">A data e a hora em que o arquivo foi compartilhado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="887b4-114">The date and time the file was last shared.</span></span> <span data-ttu-id="887b4-115">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="887b4-115">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="887b4-116">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="887b4-116">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="887b4-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="887b4-117">Read-only.</span></span>  |
| <span data-ttu-id="887b4-118">sharingSubject</span><span class="sxs-lookup"><span data-stu-id="887b4-118">sharingSubject</span></span>        | <span data-ttu-id="887b4-119">String</span><span class="sxs-lookup"><span data-stu-id="887b4-119">String</span></span>          | <span data-ttu-id="887b4-120">O assunto com o qual o documento foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="887b4-120">The subject with which the document was shared.</span></span> |
| <span data-ttu-id="887b4-121">sharingtype</span><span class="sxs-lookup"><span data-stu-id="887b4-121">sharingType</span></span>             | <span data-ttu-id="887b4-122">String</span><span class="sxs-lookup"><span data-stu-id="887b4-122">String</span></span>        | <span data-ttu-id="887b4-123">Determina o modo como o documento foi compartilhado, pode ser um "link", "anexo", "grupo", "site".</span><span class="sxs-lookup"><span data-stu-id="887b4-123">Determines the way the document was shared, can be by a "Link", "Attachment", "Group", "Site".</span></span>     |
| <span data-ttu-id="887b4-124">sharedBy</span><span class="sxs-lookup"><span data-stu-id="887b4-124">sharedBy</span></span>                | [<span data-ttu-id="887b4-125">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="887b4-125">insightIdentity</span></span>](insights-insightidentity.md)      | <span data-ttu-id="887b4-126">O usuário que compartilhou o documento.</span><span class="sxs-lookup"><span data-stu-id="887b4-126">The user who shared the document.</span></span>  |
| <span data-ttu-id="887b4-127">sharingReference</span><span class="sxs-lookup"><span data-stu-id="887b4-127">sharingReference</span></span>        | [<span data-ttu-id="887b4-128">resourceReference</span><span class="sxs-lookup"><span data-stu-id="887b4-128">resourceReference</span></span>](insights-resourcereference.md)      |  |
