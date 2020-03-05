---
title: tipo de recurso de configurações
description: As configurações atuais necessárias para um usuário usar a API de análise.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: abd68f3623f78d57b2db5812038223dc6137027f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520763"
---
# <a name="settings-resource-type"></a><span data-ttu-id="04273-103">tipo de recurso de configurações</span><span class="sxs-lookup"><span data-stu-id="04273-103">settings resource type</span></span>

<span data-ttu-id="04273-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="04273-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04273-105">Representa as configurações atuais necessárias para que um usuário use a API de análise.</span><span class="sxs-lookup"><span data-stu-id="04273-105">Represents the current required settings for a user to use the analytics API.</span></span>

<span data-ttu-id="04273-106">Para a API de análise retornar resultados para os usuários, eles devem ter uma caixa de correio hospedada na nuvem habilitada para o Microsoft Graph, ter uma licença válida do myAnalytics e ser optou por usar myAnalytics.</span><span class="sxs-lookup"><span data-stu-id="04273-106">For the analytics API to return results for users, they must have a cloud-hosted mailbox that’s enabled for Microsoft Graph, have a valid MyAnalytics license, and be opted in to using MyAnalytics.</span></span>

## <a name="methods"></a><span data-ttu-id="04273-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="04273-107">Methods</span></span>

| <span data-ttu-id="04273-108">Método</span><span class="sxs-lookup"><span data-stu-id="04273-108">Method</span></span>       | <span data-ttu-id="04273-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="04273-109">Return Type</span></span> | <span data-ttu-id="04273-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="04273-110">Description</span></span> |
|:-------------|:------------|:------------|
[<span data-ttu-id="04273-111">Obter configurações</span><span class="sxs-lookup"><span data-stu-id="04273-111">Get settings</span></span>](../api/useranalytics-get-settings.md) | [<span data-ttu-id="04273-112">configurações</span><span class="sxs-lookup"><span data-stu-id="04273-112">settings</span></span>](settings.md) | <span data-ttu-id="04273-113">Obter as configurações de propriedade a seguir para um usuário.</span><span class="sxs-lookup"><span data-stu-id="04273-113">Get the following property settings for a user.</span></span>|

## <a name="properties"></a><span data-ttu-id="04273-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="04273-114">Properties</span></span>

| <span data-ttu-id="04273-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04273-115">Property</span></span>     | <span data-ttu-id="04273-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="04273-116">Type</span></span>        | <span data-ttu-id="04273-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="04273-117">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="04273-118">hasGraphMailbox</span><span class="sxs-lookup"><span data-stu-id="04273-118">hasGraphMailbox</span></span>|<span data-ttu-id="04273-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="04273-119">Boolean</span></span>|<span data-ttu-id="04273-120">Especifica se a caixa de correio principal do usuário está hospedada na nuvem e está habilitada para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="04273-120">Specifies if the user's primary mailbox is hosted in the cloud and is enabled for Microsoft Graph.</span></span>|
|<span data-ttu-id="04273-121">hasLicense</span><span class="sxs-lookup"><span data-stu-id="04273-121">hasLicense</span></span>|<span data-ttu-id="04273-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="04273-122">Boolean</span></span>|<span data-ttu-id="04273-123">Especifica se o usuário tem uma licença myAnalytics atribuída.</span><span class="sxs-lookup"><span data-stu-id="04273-123">Specifies if the user has a MyAnalytics license assigned.</span></span>|
|<span data-ttu-id="04273-124">hasOptedOut</span><span class="sxs-lookup"><span data-stu-id="04273-124">hasOptedOut</span></span>|<span data-ttu-id="04273-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="04273-125">Boolean</span></span>|<span data-ttu-id="04273-126">Especifica se o usuário optou por ter o myAnalytics.</span><span class="sxs-lookup"><span data-stu-id="04273-126">Specifies if the user opted out of MyAnalytics.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="04273-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="04273-127">JSON representation</span></span>

<span data-ttu-id="04273-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="04273-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settings",
  "baseType": null
}-->

```json
{
  "hasGraphMailbox": true,
  "hasLicense": true,
  "hasOptedOut": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->