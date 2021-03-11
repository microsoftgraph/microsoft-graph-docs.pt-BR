---
title: Tipo de recurso applicationSignInDetailedSummary - API do Microsoft Graph
description: Representa um resumo detalhado de uma assinatura de aplicativo.
localization_priority: Normal
author: sureshja
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 8f53d1ebce8a7a578c067354ba7f89c6c27ea947
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720827"
---
# <a name="applicationsignindetailedsummary-resource-type"></a><span data-ttu-id="dd4da-103">Tipo de recurso applicationSignInDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="dd4da-103">applicationSignInDetailedSummary resource type</span></span>

<span data-ttu-id="dd4da-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd4da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd4da-105">Representa um resumo detalhado de uma assinatura de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dd4da-105">Represents a detailed summary of an application sign-in.</span></span>

## <a name="methods"></a><span data-ttu-id="dd4da-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="dd4da-106">Methods</span></span>

| <span data-ttu-id="dd4da-107">Método</span><span class="sxs-lookup"><span data-stu-id="dd4da-107">Method</span></span>       | <span data-ttu-id="dd4da-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="dd4da-108">Return Type</span></span> | <span data-ttu-id="dd4da-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd4da-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="dd4da-110">Obter applicationSignInDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="dd4da-110">Get applicationSignInDetailedSummary</span></span>](../api/applicationsignindetailedsummary-get.md) | [<span data-ttu-id="dd4da-111">applicationSignInDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="dd4da-111">applicationSignInDetailedSummary</span></span>](applicationsignindetailedsummary.md) | <span data-ttu-id="dd4da-112">Leia as propriedades e as relações de um **objeto applicationSignInDetailedSummary.**</span><span class="sxs-lookup"><span data-stu-id="dd4da-112">Read the properties and relationships of an **applicationSignInDetailedSummary** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="dd4da-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dd4da-113">Properties</span></span>
| <span data-ttu-id="dd4da-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd4da-114">Property</span></span>     | <span data-ttu-id="dd4da-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd4da-115">Type</span></span>        | <span data-ttu-id="dd4da-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd4da-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dd4da-117">aggregatedEventDateTime</span><span class="sxs-lookup"><span data-stu-id="dd4da-117">aggregatedEventDateTime</span></span>|<span data-ttu-id="dd4da-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd4da-118">DateTimeOffset</span></span>|<span data-ttu-id="dd4da-119">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="dd4da-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="dd4da-120">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="dd4da-120">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="dd4da-121">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="dd4da-121">appDisplayName</span></span>|<span data-ttu-id="dd4da-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd4da-122">String</span></span>|<span data-ttu-id="dd4da-123">Nome do aplicativo ao que o usuário se inscreveu.</span><span class="sxs-lookup"><span data-stu-id="dd4da-123">Name of the application that the user signed in to.</span></span>|
|<span data-ttu-id="dd4da-124">appId</span><span class="sxs-lookup"><span data-stu-id="dd4da-124">appId</span></span>|<span data-ttu-id="dd4da-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd4da-125">String</span></span>|<span data-ttu-id="dd4da-126">ID do aplicativo ao que o usuário se inscreveu.</span><span class="sxs-lookup"><span data-stu-id="dd4da-126">ID of the application that the user signed in to.</span></span>|
|<span data-ttu-id="dd4da-127">id</span><span class="sxs-lookup"><span data-stu-id="dd4da-127">id</span></span>|<span data-ttu-id="dd4da-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd4da-128">String</span></span>| <span data-ttu-id="dd4da-129">Uma ID exclusiva que representa a atividade de login.</span><span class="sxs-lookup"><span data-stu-id="dd4da-129">A unique ID representing the sign-in activity.</span></span>|
|<span data-ttu-id="dd4da-130">signInCount</span><span class="sxs-lookup"><span data-stu-id="dd4da-130">signInCount</span></span>|<span data-ttu-id="dd4da-131">Int64</span><span class="sxs-lookup"><span data-stu-id="dd4da-131">Int64</span></span>|<span data-ttu-id="dd4da-132">Contagem de assinaturas feitas pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dd4da-132">Count of sign-ins made by the application.</span></span>|
|<span data-ttu-id="dd4da-133">status</span><span class="sxs-lookup"><span data-stu-id="dd4da-133">status</span></span>|[<span data-ttu-id="dd4da-134">signInStatus</span><span class="sxs-lookup"><span data-stu-id="dd4da-134">signInStatus</span></span>](signinstatus.md)|<span data-ttu-id="dd4da-135">Detalhes do status de login.</span><span class="sxs-lookup"><span data-stu-id="dd4da-135">Details of the sign-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd4da-136">Relações</span><span class="sxs-lookup"><span data-stu-id="dd4da-136">Relationships</span></span>
<span data-ttu-id="dd4da-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dd4da-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="dd4da-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dd4da-138">JSON representation</span></span>

<span data-ttu-id="dd4da-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dd4da-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationSignInDetailedSummary"
}-->

```json
{
  "aggregatedEventDateTime": "String (timestamp)",
  "appDisplayName": "String",
  "appId": "String",
  "id": "String (identifier)",
  "signInCount": 1024,
  "status": {"@odata.type": "microsoft.graph.signInStatus"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationSignInDetailedSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


