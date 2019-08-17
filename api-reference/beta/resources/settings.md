---
title: tipo de recurso de configurações
description: As configurações atuais necessárias para um usuário usar a API de análise.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: a7d534aecf6e7ffa427ea175ae06e2b1820435b2
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450706"
---
# <a name="settings-resource-type"></a><span data-ttu-id="8bdf1-103">tipo de recurso de configurações</span><span class="sxs-lookup"><span data-stu-id="8bdf1-103">settings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bdf1-104">Representa as configurações atuais necessárias para que um usuário use a API de análise.</span><span class="sxs-lookup"><span data-stu-id="8bdf1-104">Represents the current required settings for a user to use the analytics API.</span></span>

<span data-ttu-id="8bdf1-105">Para a API de análise retornar resultados para os usuários, eles devem ter uma caixa de correio hospedada na nuvem habilitada para o Microsoft Graph, ter uma licença válida do myAnalytics e ser optou por usar myAnalytics.</span><span class="sxs-lookup"><span data-stu-id="8bdf1-105">For the analytics API to return results for users, they must have a cloud-hosted mailbox that’s enabled for Microsoft Graph, have a valid MyAnalytics license, and be opted in to using MyAnalytics.</span></span>

## <a name="methods"></a><span data-ttu-id="8bdf1-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="8bdf1-106">Methods</span></span>

| <span data-ttu-id="8bdf1-107">Método</span><span class="sxs-lookup"><span data-stu-id="8bdf1-107">Method</span></span>       | <span data-ttu-id="8bdf1-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8bdf1-108">Return Type</span></span> | <span data-ttu-id="8bdf1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8bdf1-109">Description</span></span> |
|:-------------|:------------|:------------|
[<span data-ttu-id="8bdf1-110">Obter configurações</span><span class="sxs-lookup"><span data-stu-id="8bdf1-110">Get settings</span></span>](../api/useranalytics-get-settings.md) | [<span data-ttu-id="8bdf1-111">configurações</span><span class="sxs-lookup"><span data-stu-id="8bdf1-111">settings</span></span>](settings.md) | <span data-ttu-id="8bdf1-112">Obter as configurações de propriedade a seguir para um usuário.</span><span class="sxs-lookup"><span data-stu-id="8bdf1-112">Get the following property settings for a user.</span></span>|

## <a name="properties"></a><span data-ttu-id="8bdf1-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8bdf1-113">Properties</span></span>

| <span data-ttu-id="8bdf1-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8bdf1-114">Property</span></span>     | <span data-ttu-id="8bdf1-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="8bdf1-115">Type</span></span>        | <span data-ttu-id="8bdf1-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="8bdf1-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8bdf1-117">hasGraphMailbox</span><span class="sxs-lookup"><span data-stu-id="8bdf1-117">hasGraphMailbox</span></span>|<span data-ttu-id="8bdf1-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="8bdf1-118">Boolean</span></span>|<span data-ttu-id="8bdf1-119">Especifica se a caixa de correio principal do usuário está hospedada na nuvem e está habilitada para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8bdf1-119">Specifies if the user's primary mailbox is hosted in the cloud and is enabled for Microsoft Graph.</span></span>|
|<span data-ttu-id="8bdf1-120">hasLicense</span><span class="sxs-lookup"><span data-stu-id="8bdf1-120">hasLicense</span></span>|<span data-ttu-id="8bdf1-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="8bdf1-121">Boolean</span></span>|<span data-ttu-id="8bdf1-122">Especifica se o usuário tem uma licença myAnalytics atribuída.</span><span class="sxs-lookup"><span data-stu-id="8bdf1-122">Specifies if the user has a MyAnalytics license assigned.</span></span>|
|<span data-ttu-id="8bdf1-123">hasOptedOut</span><span class="sxs-lookup"><span data-stu-id="8bdf1-123">hasOptedOut</span></span>|<span data-ttu-id="8bdf1-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="8bdf1-124">Boolean</span></span>|<span data-ttu-id="8bdf1-125">Especifica se o usuário optou por ter o myAnalytics.</span><span class="sxs-lookup"><span data-stu-id="8bdf1-125">Specifies if the user opted out of MyAnalytics.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8bdf1-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8bdf1-126">JSON representation</span></span>

<span data-ttu-id="8bdf1-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8bdf1-127">The following is a JSON representation of the resource.</span></span>

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