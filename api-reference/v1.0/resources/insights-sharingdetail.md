---
title: tipo de recurso sharingDetail
description: 'Tipo complexo contendo propriedades de itens compartilhados. '
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: c441dcdc3b743e5bf55786ad1b43bfe2010b01b8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531283"
---
# <a name="sharingdetail-resource-type"></a><span data-ttu-id="97586-103">tipo de recurso sharingDetail</span><span class="sxs-lookup"><span data-stu-id="97586-103">sharingDetail resource type</span></span>

<span data-ttu-id="97586-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97586-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="97586-105">Tipo complexo contendo propriedades de itens do [sharedInsight](insights-shared.md) .</span><span class="sxs-lookup"><span data-stu-id="97586-105">Complex type containing properties of [sharedInsight](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="97586-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="97586-106">JSON representation</span></span>
<span data-ttu-id="97586-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="97586-107">Here is a JSON representation of the resource</span></span>
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

## <a name="properties"></a><span data-ttu-id="97586-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="97586-108">Properties</span></span>

| <span data-ttu-id="97586-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97586-109">Property</span></span>              | <span data-ttu-id="97586-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="97586-110">Type</span></span>          | <span data-ttu-id="97586-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="97586-111">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="97586-112">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="97586-112">sharedDateTime</span></span>        | <span data-ttu-id="97586-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97586-113">DateTimeOffset</span></span>| <span data-ttu-id="97586-114">A data e a hora em que o arquivo foi compartilhado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="97586-114">The date and time the file was last shared.</span></span> <span data-ttu-id="97586-115">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="97586-115">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="97586-116">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="97586-116">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="97586-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="97586-117">Read-only.</span></span>  |
| <span data-ttu-id="97586-118">sharingSubject</span><span class="sxs-lookup"><span data-stu-id="97586-118">sharingSubject</span></span>        | <span data-ttu-id="97586-119">String</span><span class="sxs-lookup"><span data-stu-id="97586-119">String</span></span>          | <span data-ttu-id="97586-120">O assunto com o qual o documento foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="97586-120">The subject with which the document was shared.</span></span> |
| <span data-ttu-id="97586-121">sharingtype</span><span class="sxs-lookup"><span data-stu-id="97586-121">sharingType</span></span>             | <span data-ttu-id="97586-122">String</span><span class="sxs-lookup"><span data-stu-id="97586-122">String</span></span>        | <span data-ttu-id="97586-123">Determina o modo como o documento foi compartilhado, pode ser um "link", "anexo", "grupo", "site".</span><span class="sxs-lookup"><span data-stu-id="97586-123">Determines the way the document was shared, can be by a "Link", "Attachment", "Group", "Site".</span></span>     |
| <span data-ttu-id="97586-124">sharedBy</span><span class="sxs-lookup"><span data-stu-id="97586-124">sharedBy</span></span>                | [<span data-ttu-id="97586-125">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="97586-125">insightIdentity</span></span>](insights-insightidentity.md)      | <span data-ttu-id="97586-126">O usuário que compartilhou o documento.</span><span class="sxs-lookup"><span data-stu-id="97586-126">The user who shared the document.</span></span>  |
| <span data-ttu-id="97586-127">sharingReference</span><span class="sxs-lookup"><span data-stu-id="97586-127">sharingReference</span></span>        | [<span data-ttu-id="97586-128">resourceReference</span><span class="sxs-lookup"><span data-stu-id="97586-128">resourceReference</span></span>](insights-resourcereference.md)      |  |
