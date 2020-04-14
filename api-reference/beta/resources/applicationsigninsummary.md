---
title: tipo de recurso applicationSignInDetailedSummary
description: Representa um resumo de entrada do aplicativo.
localization_priority: Normal
author: kholtz
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 79dbe02f723c9c8912ce8a227a47d6f50260c330
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455273"
---
# <a name="applicationsigninsummary-resource-type"></a><span data-ttu-id="2fea9-103">tipo de recurso applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="2fea9-103">applicationSignInSummary resource type</span></span>

<span data-ttu-id="2fea9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fea9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fea9-105">Representa um resumo de entrada do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2fea9-105">Represents an application sign-in summary.</span></span>

## <a name="methods"></a><span data-ttu-id="2fea9-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="2fea9-106">Methods</span></span>

| <span data-ttu-id="2fea9-107">Método</span><span class="sxs-lookup"><span data-stu-id="2fea9-107">Method</span></span>       | <span data-ttu-id="2fea9-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2fea9-108">Return Type</span></span> | <span data-ttu-id="2fea9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fea9-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2fea9-110">Obter applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="2fea9-110">Get applicationSignInSummary</span></span>](../api/applicationsigninsummary-get.md) | [<span data-ttu-id="2fea9-111">applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="2fea9-111">applicationSignInSummary</span></span>](applicationsigninsummary.md) | <span data-ttu-id="2fea9-112">Leia as propriedades e os relacionamentos de um objeto **applicationSignInSummary** .</span><span class="sxs-lookup"><span data-stu-id="2fea9-112">Read the properties and relationships of an **applicationSignInSummary** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2fea9-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2fea9-113">Properties</span></span>
| <span data-ttu-id="2fea9-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2fea9-114">Property</span></span>     | <span data-ttu-id="2fea9-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="2fea9-115">Type</span></span>        | <span data-ttu-id="2fea9-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fea9-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2fea9-117">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="2fea9-117">appDisplayName</span></span>|<span data-ttu-id="2fea9-118">String</span><span class="sxs-lookup"><span data-stu-id="2fea9-118">String</span></span>|<span data-ttu-id="2fea9-119">Nome do aplicativo no qual o usuário entrou.</span><span class="sxs-lookup"><span data-stu-id="2fea9-119">Name of the application that the user signed in to.</span></span>|
|<span data-ttu-id="2fea9-120">appId</span><span class="sxs-lookup"><span data-stu-id="2fea9-120">appId</span></span>|<span data-ttu-id="2fea9-121">String</span><span class="sxs-lookup"><span data-stu-id="2fea9-121">String</span></span>|  <span data-ttu-id="2fea9-122">ID do aplicativo que o usuário assinou me .\n\nPara.</span><span class="sxs-lookup"><span data-stu-id="2fea9-122">ID of the application that the user signed i nto.</span></span>|
|<span data-ttu-id="2fea9-123">failedSignInCount</span><span class="sxs-lookup"><span data-stu-id="2fea9-123">failedSignInCount</span></span>|<span data-ttu-id="2fea9-124">Int64</span><span class="sxs-lookup"><span data-stu-id="2fea9-124">Int64</span></span>|<span data-ttu-id="2fea9-125">Contagem de entradas com falha feitas pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2fea9-125">Count of failed sign-ins made by the application.</span></span>|
|<span data-ttu-id="2fea9-126">successPercentage</span><span class="sxs-lookup"><span data-stu-id="2fea9-126">successPercentage</span></span>|<span data-ttu-id="2fea9-127">Int32</span><span class="sxs-lookup"><span data-stu-id="2fea9-127">Int32</span></span>|<span data-ttu-id="2fea9-128">Porcentagem de entradas bem-sucedidas feitas pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2fea9-128">Percentage of successful sign-ins made by the application.</span></span>|
|<span data-ttu-id="2fea9-129">successfulSignInCount</span><span class="sxs-lookup"><span data-stu-id="2fea9-129">successfulSignInCount</span></span>|<span data-ttu-id="2fea9-130">Int64</span><span class="sxs-lookup"><span data-stu-id="2fea9-130">Int64</span></span>|<span data-ttu-id="2fea9-131">Contagem de entradas bem-sucedidas feitas pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2fea9-131">Count of successful sign-ins made by the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2fea9-132">Relações</span><span class="sxs-lookup"><span data-stu-id="2fea9-132">Relationships</span></span>
<span data-ttu-id="2fea9-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2fea9-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="2fea9-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2fea9-134">JSON representation</span></span>

<span data-ttu-id="2fea9-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2fea9-135">The following is a JSON representation of the resource.</span></span>

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
