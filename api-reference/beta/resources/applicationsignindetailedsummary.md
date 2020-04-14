---
title: tipo de recurso applicationSignInDetailedSummary-API do Microsoft Graph
description: Representa um resumo detalhado de uma entrada de aplicativo.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 754a7f69b4f38fa101fe2fe5c349e089ae25c457
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455280"
---
# <a name="applicationsignindetailedsummary-resource-type"></a><span data-ttu-id="78347-103">tipo de recurso applicationSignInDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="78347-103">applicationSignInDetailedSummary resource type</span></span>

<span data-ttu-id="78347-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78347-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78347-105">Representa um resumo detalhado de uma entrada de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="78347-105">Represents a detailed summary of an application sign-in.</span></span>

## <a name="methods"></a><span data-ttu-id="78347-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="78347-106">Methods</span></span>

| <span data-ttu-id="78347-107">Método</span><span class="sxs-lookup"><span data-stu-id="78347-107">Method</span></span>       | <span data-ttu-id="78347-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="78347-108">Return Type</span></span> | <span data-ttu-id="78347-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="78347-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="78347-110">Obter applicationSignInDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="78347-110">Get applicationSignInDetailedSummary</span></span>](../api/applicationsignindetailedsummary-get.md) | [<span data-ttu-id="78347-111">applicationSignInDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="78347-111">applicationSignInDetailedSummary</span></span>](applicationsignindetailedsummary.md) | <span data-ttu-id="78347-112">Leia as propriedades e os relacionamentos de um objeto **applicationSignInDetailedSummary** .</span><span class="sxs-lookup"><span data-stu-id="78347-112">Read the properties and relationships of an **applicationSignInDetailedSummary** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="78347-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="78347-113">Properties</span></span>
| <span data-ttu-id="78347-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="78347-114">Property</span></span>     | <span data-ttu-id="78347-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="78347-115">Type</span></span>        | <span data-ttu-id="78347-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="78347-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="78347-117">aggregatedEventDateTime</span><span class="sxs-lookup"><span data-stu-id="78347-117">aggregatedEventDateTime</span></span>|<span data-ttu-id="78347-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78347-118">DateTimeOffset</span></span>|<span data-ttu-id="78347-119">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="78347-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="78347-120">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="78347-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="78347-121">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="78347-121">appDisplayName</span></span>|<span data-ttu-id="78347-122">String</span><span class="sxs-lookup"><span data-stu-id="78347-122">String</span></span>|<span data-ttu-id="78347-123">Nome do aplicativo no qual o usuário entrou.</span><span class="sxs-lookup"><span data-stu-id="78347-123">Name of the application that the user signed in to.</span></span>|
|<span data-ttu-id="78347-124">appId</span><span class="sxs-lookup"><span data-stu-id="78347-124">appId</span></span>|<span data-ttu-id="78347-125">String</span><span class="sxs-lookup"><span data-stu-id="78347-125">String</span></span>|<span data-ttu-id="78347-126">ID do aplicativo no qual o usuário entrou.</span><span class="sxs-lookup"><span data-stu-id="78347-126">ID of the application that the user signed in to.</span></span>|
|<span data-ttu-id="78347-127">id</span><span class="sxs-lookup"><span data-stu-id="78347-127">id</span></span>|<span data-ttu-id="78347-128">String</span><span class="sxs-lookup"><span data-stu-id="78347-128">String</span></span>| <span data-ttu-id="78347-129">Uma ID exclusiva que representa a atividade de entrada.</span><span class="sxs-lookup"><span data-stu-id="78347-129">A unique ID representing the sign-in activity.</span></span>|
|<span data-ttu-id="78347-130">signInCount</span><span class="sxs-lookup"><span data-stu-id="78347-130">signInCount</span></span>|<span data-ttu-id="78347-131">Int64</span><span class="sxs-lookup"><span data-stu-id="78347-131">Int64</span></span>|<span data-ttu-id="78347-132">Contagem de entradas feitas pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="78347-132">Count of sign-ins made by the application.</span></span>|
|<span data-ttu-id="78347-133">status</span><span class="sxs-lookup"><span data-stu-id="78347-133">status</span></span>|[<span data-ttu-id="78347-134">signInStatus</span><span class="sxs-lookup"><span data-stu-id="78347-134">signInStatus</span></span>](signinstatus.md)|<span data-ttu-id="78347-135">Detalhes do status de entrada.</span><span class="sxs-lookup"><span data-stu-id="78347-135">Details of the sign-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78347-136">Relações</span><span class="sxs-lookup"><span data-stu-id="78347-136">Relationships</span></span>
<span data-ttu-id="78347-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="78347-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="78347-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="78347-138">JSON representation</span></span>

<span data-ttu-id="78347-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="78347-139">The following is a JSON representation of the resource.</span></span>

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
