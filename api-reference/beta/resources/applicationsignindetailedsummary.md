---
title: tipo de recurso applicationSignInDetailedSummary-API do Microsoft Graph
description: Representa um resumo detalhado de uma entrada de aplicativo.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 527d60ff025e9a6d081226a51ec8cbefc53c20de
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013326"
---
# <a name="applicationsignindetailedsummary-resource-type"></a><span data-ttu-id="b28fd-103">tipo de recurso applicationSignInDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="b28fd-103">applicationSignInDetailedSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b28fd-104">Representa um resumo detalhado de uma entrada de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b28fd-104">Represents a detailed summary of an application sign-in.</span></span>

## <a name="methods"></a><span data-ttu-id="b28fd-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="b28fd-105">Methods</span></span>

| <span data-ttu-id="b28fd-106">Método</span><span class="sxs-lookup"><span data-stu-id="b28fd-106">Method</span></span>       | <span data-ttu-id="b28fd-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b28fd-107">Return Type</span></span> | <span data-ttu-id="b28fd-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b28fd-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b28fd-109">Obter applicationSignInDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="b28fd-109">Get applicationSignInDetailedSummary</span></span>](../api/applicationsignindetailedsummary-get.md) | [<span data-ttu-id="b28fd-110">applicationSignInDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="b28fd-110">applicationSignInDetailedSummary</span></span>](applicationsignindetailedsummary.md) | <span data-ttu-id="b28fd-111">Leia as propriedades e os relacionamentos de um objeto **applicationSignInDetailedSummary** .</span><span class="sxs-lookup"><span data-stu-id="b28fd-111">Read the properties and relationships of an **applicationSignInDetailedSummary** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b28fd-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b28fd-112">Properties</span></span>
| <span data-ttu-id="b28fd-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b28fd-113">Property</span></span>     | <span data-ttu-id="b28fd-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="b28fd-114">Type</span></span>        | <span data-ttu-id="b28fd-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="b28fd-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b28fd-116">aggregatedEventDateTime</span><span class="sxs-lookup"><span data-stu-id="b28fd-116">aggregatedEventDateTime</span></span>|<span data-ttu-id="b28fd-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b28fd-117">DateTimeOffset</span></span>|<span data-ttu-id="b28fd-118">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b28fd-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b28fd-119">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b28fd-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="b28fd-120">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="b28fd-120">appDisplayName</span></span>|<span data-ttu-id="b28fd-121">String</span><span class="sxs-lookup"><span data-stu-id="b28fd-121">String</span></span>|<span data-ttu-id="b28fd-122">Nome do aplicativo no qual o usuário entrou.</span><span class="sxs-lookup"><span data-stu-id="b28fd-122">Name of the application that the user signed in to.</span></span>|
|<span data-ttu-id="b28fd-123">appId</span><span class="sxs-lookup"><span data-stu-id="b28fd-123">appId</span></span>|<span data-ttu-id="b28fd-124">String</span><span class="sxs-lookup"><span data-stu-id="b28fd-124">String</span></span>|<span data-ttu-id="b28fd-125">ID do aplicativo no qual o usuário entrou.</span><span class="sxs-lookup"><span data-stu-id="b28fd-125">ID of the application that the user signed in to.</span></span>|
|<span data-ttu-id="b28fd-126">id</span><span class="sxs-lookup"><span data-stu-id="b28fd-126">id</span></span>|<span data-ttu-id="b28fd-127">String</span><span class="sxs-lookup"><span data-stu-id="b28fd-127">String</span></span>| <span data-ttu-id="b28fd-128">Uma ID exclusiva que representa a atividade de entrada.</span><span class="sxs-lookup"><span data-stu-id="b28fd-128">A unique ID representing the sign-in activity.</span></span>|
|<span data-ttu-id="b28fd-129">signInCount</span><span class="sxs-lookup"><span data-stu-id="b28fd-129">signInCount</span></span>|<span data-ttu-id="b28fd-130">Int64</span><span class="sxs-lookup"><span data-stu-id="b28fd-130">Int64</span></span>|<span data-ttu-id="b28fd-131">Contagem de entradas feitas pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b28fd-131">Count of sign-ins made by the application.</span></span>|
|<span data-ttu-id="b28fd-132">status</span><span class="sxs-lookup"><span data-stu-id="b28fd-132">status</span></span>|[<span data-ttu-id="b28fd-133">signInStatus</span><span class="sxs-lookup"><span data-stu-id="b28fd-133">signInStatus</span></span>](signinstatus.md)|<span data-ttu-id="b28fd-134">Detalhes do status de entrada.</span><span class="sxs-lookup"><span data-stu-id="b28fd-134">Details of the sign-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b28fd-135">Relações</span><span class="sxs-lookup"><span data-stu-id="b28fd-135">Relationships</span></span>
<span data-ttu-id="b28fd-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b28fd-136">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b28fd-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b28fd-137">JSON representation</span></span>

<span data-ttu-id="b28fd-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b28fd-138">The following is a JSON representation of the resource.</span></span>

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
