---
title: Tipo de recurso applicationSignInDetailedSummary
description: Representa um resumo de login do aplicativo.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 454c4e2e9e57b61194e6f3e6970e5db1ea414369
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137407"
---
# <a name="applicationsigninsummary-resource-type"></a><span data-ttu-id="3ef1e-103">Tipo de recurso applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="3ef1e-103">applicationSignInSummary resource type</span></span>

<span data-ttu-id="3ef1e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ef1e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ef1e-105">Representa um resumo de login do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3ef1e-105">Represents an application sign-in summary.</span></span>

## <a name="methods"></a><span data-ttu-id="3ef1e-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="3ef1e-106">Methods</span></span>

| <span data-ttu-id="3ef1e-107">Método</span><span class="sxs-lookup"><span data-stu-id="3ef1e-107">Method</span></span>       | <span data-ttu-id="3ef1e-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3ef1e-108">Return Type</span></span> | <span data-ttu-id="3ef1e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ef1e-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3ef1e-110">Obter applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="3ef1e-110">Get applicationSignInSummary</span></span>](../api/applicationsigninsummary-get.md) | [<span data-ttu-id="3ef1e-111">applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="3ef1e-111">applicationSignInSummary</span></span>](applicationsigninsummary.md) | <span data-ttu-id="3ef1e-112">Leia as propriedades e os relacionamentos de **um objeto applicationSignInSummary.**</span><span class="sxs-lookup"><span data-stu-id="3ef1e-112">Read the properties and relationships of an **applicationSignInSummary** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3ef1e-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3ef1e-113">Properties</span></span>
| <span data-ttu-id="3ef1e-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3ef1e-114">Property</span></span>     | <span data-ttu-id="3ef1e-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ef1e-115">Type</span></span>        | <span data-ttu-id="3ef1e-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ef1e-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3ef1e-117">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="3ef1e-117">appDisplayName</span></span>|<span data-ttu-id="3ef1e-118">String</span><span class="sxs-lookup"><span data-stu-id="3ef1e-118">String</span></span>|<span data-ttu-id="3ef1e-119">Nome do aplicativo em que o usuário se inscreveu.</span><span class="sxs-lookup"><span data-stu-id="3ef1e-119">Name of the application that the user signed in to.</span></span>|
|<span data-ttu-id="3ef1e-120">appId</span><span class="sxs-lookup"><span data-stu-id="3ef1e-120">appId</span></span>|<span data-ttu-id="3ef1e-121">String</span><span class="sxs-lookup"><span data-stu-id="3ef1e-121">String</span></span>|  <span data-ttu-id="3ef1e-122">ID do aplicativo que o usuário assinou i nto.</span><span class="sxs-lookup"><span data-stu-id="3ef1e-122">ID of the application that the user signed i nto.</span></span>|
|<span data-ttu-id="3ef1e-123">failedSignInCount</span><span class="sxs-lookup"><span data-stu-id="3ef1e-123">failedSignInCount</span></span>|<span data-ttu-id="3ef1e-124">Int64</span><span class="sxs-lookup"><span data-stu-id="3ef1e-124">Int64</span></span>|<span data-ttu-id="3ef1e-125">Contagem de falhas de logins feitas pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3ef1e-125">Count of failed sign-ins made by the application.</span></span>|
|<span data-ttu-id="3ef1e-126">successPercentage</span><span class="sxs-lookup"><span data-stu-id="3ef1e-126">successPercentage</span></span>|<span data-ttu-id="3ef1e-127">Int32</span><span class="sxs-lookup"><span data-stu-id="3ef1e-127">Int32</span></span>|<span data-ttu-id="3ef1e-128">Porcentagem de logins bem-sucedidos feitos pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3ef1e-128">Percentage of successful sign-ins made by the application.</span></span>|
|<span data-ttu-id="3ef1e-129">successfulSignInCount</span><span class="sxs-lookup"><span data-stu-id="3ef1e-129">successfulSignInCount</span></span>|<span data-ttu-id="3ef1e-130">Int64</span><span class="sxs-lookup"><span data-stu-id="3ef1e-130">Int64</span></span>|<span data-ttu-id="3ef1e-131">Contagem de logins bem-sucedidos feitos pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3ef1e-131">Count of successful sign-ins made by the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ef1e-132">Relações</span><span class="sxs-lookup"><span data-stu-id="3ef1e-132">Relationships</span></span>
<span data-ttu-id="3ef1e-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3ef1e-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3ef1e-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3ef1e-134">JSON representation</span></span>

<span data-ttu-id="3ef1e-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3ef1e-135">The following is a JSON representation of the resource.</span></span>

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


