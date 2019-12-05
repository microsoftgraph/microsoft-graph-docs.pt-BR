---
title: tipo de recurso sharingDetail
description: 'Tipo complexo contendo propriedades de itens compartilhados. '
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: fdfd17870841c260347a46984c16d96be11c1182
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844208"
---
# <a name="sharingdetail-resource-type"></a><span data-ttu-id="dc04d-103">tipo de recurso sharingDetail</span><span class="sxs-lookup"><span data-stu-id="dc04d-103">sharingDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc04d-104">Tipo complexo contendo propriedades de itens do [sharedInsight](insights-shared.md) .</span><span class="sxs-lookup"><span data-stu-id="dc04d-104">Complex type containing properties of [sharedInsight](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="dc04d-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dc04d-105">JSON representation</span></span>
<span data-ttu-id="dc04d-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="dc04d-106">Here is a JSON representation of the resource</span></span>
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

## <a name="properties"></a><span data-ttu-id="dc04d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dc04d-107">Properties</span></span>

| <span data-ttu-id="dc04d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dc04d-108">Property</span></span>              | <span data-ttu-id="dc04d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc04d-109">Type</span></span>          | <span data-ttu-id="dc04d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc04d-110">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="dc04d-111">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="dc04d-111">sharedDateTime</span></span>        | <span data-ttu-id="dc04d-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc04d-112">DateTimeOffset</span></span>| <span data-ttu-id="dc04d-113">A data e a hora em que o arquivo foi compartilhado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="dc04d-113">The date and time the file was last shared.</span></span> <span data-ttu-id="dc04d-114">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="dc04d-114">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="dc04d-115">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="dc04d-115">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="dc04d-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dc04d-116">Read-only.</span></span>  |
| <span data-ttu-id="dc04d-117">sharingSubject</span><span class="sxs-lookup"><span data-stu-id="dc04d-117">sharingSubject</span></span>        | <span data-ttu-id="dc04d-118">String</span><span class="sxs-lookup"><span data-stu-id="dc04d-118">String</span></span>          | <span data-ttu-id="dc04d-119">O assunto com o qual o documento foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="dc04d-119">The subject with which the document was shared.</span></span> |
| <span data-ttu-id="dc04d-120">sharingtype</span><span class="sxs-lookup"><span data-stu-id="dc04d-120">sharingType</span></span>             | <span data-ttu-id="dc04d-121">String</span><span class="sxs-lookup"><span data-stu-id="dc04d-121">String</span></span>        | <span data-ttu-id="dc04d-122">Determina o modo como o documento foi compartilhado, pode ser um "link", "anexo", "grupo", "site".</span><span class="sxs-lookup"><span data-stu-id="dc04d-122">Determines the way the document was shared, can be by a "Link", "Attachment", "Group", "Site".</span></span>     |
| <span data-ttu-id="dc04d-123">sharedBy</span><span class="sxs-lookup"><span data-stu-id="dc04d-123">sharedBy</span></span>                | [<span data-ttu-id="dc04d-124">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="dc04d-124">insightIdentity</span></span>](insights-insightidentity.md)      | <span data-ttu-id="dc04d-125">O usuário que compartilhou o documento.</span><span class="sxs-lookup"><span data-stu-id="dc04d-125">The user who shared the document.</span></span>  |
| <span data-ttu-id="dc04d-126">sharingReference</span><span class="sxs-lookup"><span data-stu-id="dc04d-126">sharingReference</span></span>        | [<span data-ttu-id="dc04d-127">resourceReference</span><span class="sxs-lookup"><span data-stu-id="dc04d-127">resourceReference</span></span>](insights-resourcereference.md)      |  |
