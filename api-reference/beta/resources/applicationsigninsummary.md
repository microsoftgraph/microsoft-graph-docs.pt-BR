---
title: tipo de recurso applicationSignInDetailedSummary
description: Representa um resumo de entrada do aplicativo.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0329aec304602151a23ff389bc041247f9fb65b7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339033"
---
# <a name="applicationsigninsummary-resource-type"></a><span data-ttu-id="87aa1-103">tipo de recurso applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="87aa1-103">applicationSignInSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87aa1-104">Representa um resumo de entrada do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="87aa1-104">Represents an application sign-in summary.</span></span>

## <a name="methods"></a><span data-ttu-id="87aa1-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="87aa1-105">Methods</span></span>

| <span data-ttu-id="87aa1-106">Método</span><span class="sxs-lookup"><span data-stu-id="87aa1-106">Method</span></span>       | <span data-ttu-id="87aa1-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="87aa1-107">Return Type</span></span> | <span data-ttu-id="87aa1-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="87aa1-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="87aa1-109">Obter applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="87aa1-109">Get applicationSignInSummary</span></span>](../api/applicationsigninsummary-get.md) | [<span data-ttu-id="87aa1-110">applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="87aa1-110">applicationSignInSummary</span></span>](applicationsigninsummary.md) | <span data-ttu-id="87aa1-111">Leia as propriedades e os relacionamentos de um objeto **applicationSignInSummary** .</span><span class="sxs-lookup"><span data-stu-id="87aa1-111">Read the properties and relationships of an **applicationSignInSummary** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="87aa1-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="87aa1-112">Properties</span></span>
| <span data-ttu-id="87aa1-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87aa1-113">Property</span></span>     | <span data-ttu-id="87aa1-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="87aa1-114">Type</span></span>        | <span data-ttu-id="87aa1-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="87aa1-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="87aa1-116">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="87aa1-116">appDisplayName</span></span>|<span data-ttu-id="87aa1-117">String</span><span class="sxs-lookup"><span data-stu-id="87aa1-117">String</span></span>|<span data-ttu-id="87aa1-118">Nome do aplicativo no qual o usuário entrou.</span><span class="sxs-lookup"><span data-stu-id="87aa1-118">Name of the application that the user signed in to.</span></span>|
|<span data-ttu-id="87aa1-119">appId</span><span class="sxs-lookup"><span data-stu-id="87aa1-119">appId</span></span>|<span data-ttu-id="87aa1-120">String</span><span class="sxs-lookup"><span data-stu-id="87aa1-120">String</span></span>|  <span data-ttu-id="87aa1-121">ID do aplicativo que o usuário assinou me .\n\nPara.</span><span class="sxs-lookup"><span data-stu-id="87aa1-121">ID of the application that the user signed i nto.</span></span>|
|<span data-ttu-id="87aa1-122">failedSignInCount</span><span class="sxs-lookup"><span data-stu-id="87aa1-122">failedSignInCount</span></span>|<span data-ttu-id="87aa1-123">Int64</span><span class="sxs-lookup"><span data-stu-id="87aa1-123">Int64</span></span>|<span data-ttu-id="87aa1-124">Contagem de entradas com falha feitas pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="87aa1-124">Count of failed sign-ins made by the application.</span></span>|
|<span data-ttu-id="87aa1-125">successPercentage</span><span class="sxs-lookup"><span data-stu-id="87aa1-125">successPercentage</span></span>|<span data-ttu-id="87aa1-126">Int32</span><span class="sxs-lookup"><span data-stu-id="87aa1-126">Int32</span></span>|<span data-ttu-id="87aa1-127">Porcentagem de entradas bem-sucedidas feitas pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="87aa1-127">Percentage of successful sign-ins made by the application.</span></span>|
|<span data-ttu-id="87aa1-128">successfulSignInCount</span><span class="sxs-lookup"><span data-stu-id="87aa1-128">successfulSignInCount</span></span>|<span data-ttu-id="87aa1-129">Int64</span><span class="sxs-lookup"><span data-stu-id="87aa1-129">Int64</span></span>|<span data-ttu-id="87aa1-130">Contagem de entradas bem-sucedidas feitas pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="87aa1-130">Count of successful sign-ins made by the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="87aa1-131">Relações</span><span class="sxs-lookup"><span data-stu-id="87aa1-131">Relationships</span></span>
<span data-ttu-id="87aa1-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="87aa1-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="87aa1-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="87aa1-133">JSON representation</span></span>

<span data-ttu-id="87aa1-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="87aa1-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationSignInSummary"
}-->

```json
{
  "appDisplayName": "String",
  "appId": "String (identifier)",
  "failedSignInCount": 1024,
  "successPercentage": 1024,
  "successfulSignInCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationSignInSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
