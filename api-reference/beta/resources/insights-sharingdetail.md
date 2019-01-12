---
title: tipo de recurso de sharingDetail
description: 'Tipo complexo que contém as propriedades de itens compartilhados. '
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: add63a89a451b742778dda1d6d313d58f675a642
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918760"
---
# <a name="sharingdetail-resource-type"></a><span data-ttu-id="b2e4d-103">tipo de recurso de sharingDetail</span><span class="sxs-lookup"><span data-stu-id="b2e4d-103">sharingDetail resource type</span></span>

> <span data-ttu-id="b2e4d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b2e4d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2e4d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b2e4d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b2e4d-106">Tipo complexo que contém as propriedades de itens [compartilhados](insights-shared.md) .</span><span class="sxs-lookup"><span data-stu-id="b2e4d-106">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="b2e4d-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b2e4d-107">JSON representation</span></span>
<span data-ttu-id="b2e4d-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b2e4d-108">Here is a JSON representation of the resource</span></span>

```json
{
  "sharedDateTime": "dateTimeOffset",
  "sharingSubject": "string",
  "sharingType": "string",
  "sharedBy": "insightIdentity",
  "resourceReference": "resourceReference"
}
```

## <a name="properties"></a><span data-ttu-id="b2e4d-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b2e4d-109">Properties</span></span>

| <span data-ttu-id="b2e4d-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2e4d-110">Property</span></span>              | <span data-ttu-id="b2e4d-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2e4d-111">Type</span></span>          | <span data-ttu-id="b2e4d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2e4d-112">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="b2e4d-113">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="b2e4d-113">sharedDateTime</span></span>        | <span data-ttu-id="b2e4d-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2e4d-114">DateTimeOffset</span></span>| <span data-ttu-id="b2e4d-115">A data e hora que o arquivo foi última compartilhado.</span><span class="sxs-lookup"><span data-stu-id="b2e4d-115">The date and time the file was last shared.</span></span> <span data-ttu-id="b2e4d-116">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b2e4d-116">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b2e4d-117">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="b2e4d-117">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="b2e4d-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2e4d-118">Read-only.</span></span>  |
| <span data-ttu-id="b2e4d-119">sharingSubject</span><span class="sxs-lookup"><span data-stu-id="b2e4d-119">sharingSubject</span></span>        | <span data-ttu-id="b2e4d-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2e4d-120">String</span></span>          | <span data-ttu-id="b2e4d-121">O assunto com a qual o documento foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="b2e4d-121">The subject with which the document was shared.</span></span> |
| <span data-ttu-id="b2e4d-122">sharingType</span><span class="sxs-lookup"><span data-stu-id="b2e4d-122">sharingType</span></span>             | <span data-ttu-id="b2e4d-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2e4d-123">String</span></span>        | <span data-ttu-id="b2e4d-124">Determina a maneira como o documento foi compartilhada, pode ser um "Link", por "Anexo", "Grupo", "Site".</span><span class="sxs-lookup"><span data-stu-id="b2e4d-124">Determines the way the document was shared, can be by a "Link", "Attachment", "Group", "Site".</span></span>     |
| <span data-ttu-id="b2e4d-125">sharedBy</span><span class="sxs-lookup"><span data-stu-id="b2e4d-125">sharedBy</span></span>                | [<span data-ttu-id="b2e4d-126">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="b2e4d-126">insightIdentity</span></span>](insights-insightidentity.md)      | <span data-ttu-id="b2e4d-127">O usuário que compartilhado do documento.</span><span class="sxs-lookup"><span data-stu-id="b2e4d-127">The user who shared the document.</span></span>  |
| <span data-ttu-id="b2e4d-128">sharingReference</span><span class="sxs-lookup"><span data-stu-id="b2e4d-128">sharingReference</span></span>        | [<span data-ttu-id="b2e4d-129">resourceReference</span><span class="sxs-lookup"><span data-stu-id="b2e4d-129">resourceReference</span></span>](insights-resourcereference.md)      |  |
