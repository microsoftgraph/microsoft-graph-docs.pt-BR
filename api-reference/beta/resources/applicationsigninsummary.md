---
title: tipo de recurso applicationSignInDetailedSummary
description: Representa um resumo de entrada do aplicativo.
localization_priority: Normal
author: khotz
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0e654df6af359069bbc476c5419a20ca0429f9a5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050238"
---
# <a name="applicationsigninsummary-resource-type"></a><span data-ttu-id="64887-103">tipo de recurso applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="64887-103">applicationSignInSummary resource type</span></span>

<span data-ttu-id="64887-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64887-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64887-105">Representa um resumo de entrada do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="64887-105">Represents an application sign-in summary.</span></span>

## <a name="methods"></a><span data-ttu-id="64887-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="64887-106">Methods</span></span>

| <span data-ttu-id="64887-107">Método</span><span class="sxs-lookup"><span data-stu-id="64887-107">Method</span></span>       | <span data-ttu-id="64887-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="64887-108">Return Type</span></span> | <span data-ttu-id="64887-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="64887-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="64887-110">Obter applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="64887-110">Get applicationSignInSummary</span></span>](../api/applicationsigninsummary-get.md) | [<span data-ttu-id="64887-111">applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="64887-111">applicationSignInSummary</span></span>](applicationsigninsummary.md) | <span data-ttu-id="64887-112">Leia as propriedades e os relacionamentos de um objeto **applicationSignInSummary** .</span><span class="sxs-lookup"><span data-stu-id="64887-112">Read the properties and relationships of an **applicationSignInSummary** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="64887-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="64887-113">Properties</span></span>
| <span data-ttu-id="64887-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64887-114">Property</span></span>     | <span data-ttu-id="64887-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="64887-115">Type</span></span>        | <span data-ttu-id="64887-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="64887-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="64887-117">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="64887-117">appDisplayName</span></span>|<span data-ttu-id="64887-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="64887-118">String</span></span>|<span data-ttu-id="64887-119">Nome do aplicativo no qual o usuário entrou.</span><span class="sxs-lookup"><span data-stu-id="64887-119">Name of the application that the user signed in to.</span></span>|
|<span data-ttu-id="64887-120">appId</span><span class="sxs-lookup"><span data-stu-id="64887-120">appId</span></span>|<span data-ttu-id="64887-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="64887-121">String</span></span>|  <span data-ttu-id="64887-122">ID do aplicativo que o usuário assinou me .\n\nPara.</span><span class="sxs-lookup"><span data-stu-id="64887-122">ID of the application that the user signed i nto.</span></span>|
|<span data-ttu-id="64887-123">failedSignInCount</span><span class="sxs-lookup"><span data-stu-id="64887-123">failedSignInCount</span></span>|<span data-ttu-id="64887-124">Int64</span><span class="sxs-lookup"><span data-stu-id="64887-124">Int64</span></span>|<span data-ttu-id="64887-125">Contagem de entradas com falha feitas pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="64887-125">Count of failed sign-ins made by the application.</span></span>|
|<span data-ttu-id="64887-126">successPercentage</span><span class="sxs-lookup"><span data-stu-id="64887-126">successPercentage</span></span>|<span data-ttu-id="64887-127">Int32</span><span class="sxs-lookup"><span data-stu-id="64887-127">Int32</span></span>|<span data-ttu-id="64887-128">Porcentagem de entradas bem-sucedidas feitas pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="64887-128">Percentage of successful sign-ins made by the application.</span></span>|
|<span data-ttu-id="64887-129">successfulSignInCount</span><span class="sxs-lookup"><span data-stu-id="64887-129">successfulSignInCount</span></span>|<span data-ttu-id="64887-130">Int64</span><span class="sxs-lookup"><span data-stu-id="64887-130">Int64</span></span>|<span data-ttu-id="64887-131">Contagem de entradas bem-sucedidas feitas pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="64887-131">Count of successful sign-ins made by the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64887-132">Relações</span><span class="sxs-lookup"><span data-stu-id="64887-132">Relationships</span></span>
<span data-ttu-id="64887-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="64887-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="64887-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="64887-134">JSON representation</span></span>

<span data-ttu-id="64887-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="64887-135">The following is a JSON representation of the resource.</span></span>

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


