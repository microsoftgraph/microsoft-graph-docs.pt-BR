---
title: tipo de recurso de privilegedRoleSummary
description: As estatísticas de resumida de uma determinada função.
ms.openlocfilehash: f6c66433651eff188ce6fdaa07c2422d3bb6e0ce
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039650"
---
# <a name="privilegedrolesummary-resource-type"></a><span data-ttu-id="3c67b-103">tipo de recurso de privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="3c67b-103">privilegedRoleSummary resource type</span></span>

> <span data-ttu-id="3c67b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3c67b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c67b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3c67b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3c67b-106">As estatísticas de resumida de uma determinada função.</span><span class="sxs-lookup"><span data-stu-id="3c67b-106">The statistics summary for a particular role.</span></span>


## <a name="methods"></a><span data-ttu-id="3c67b-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="3c67b-107">Methods</span></span>

| <span data-ttu-id="3c67b-108">Método</span><span class="sxs-lookup"><span data-stu-id="3c67b-108">Method</span></span>           | <span data-ttu-id="3c67b-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3c67b-109">Return Type</span></span>    |<span data-ttu-id="3c67b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c67b-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3c67b-111">Obter privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="3c67b-111">Get privilegedRoleSummary</span></span>](../api/privilegedrolesummary-get.md) | [<span data-ttu-id="3c67b-112">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="3c67b-112">privilegedRoleSummary</span></span>](privilegedrolesummary.md) |<span data-ttu-id="3c67b-113">Leia as propriedades e os relacionamentos do objeto privilegedRoleSummary.</span><span class="sxs-lookup"><span data-stu-id="3c67b-113">Read properties and relationships of privilegedRoleSummary object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3c67b-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3c67b-114">Properties</span></span>
| <span data-ttu-id="3c67b-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c67b-115">Property</span></span>     | <span data-ttu-id="3c67b-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c67b-116">Type</span></span>   |<span data-ttu-id="3c67b-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c67b-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c67b-118">elevatedCount</span><span class="sxs-lookup"><span data-stu-id="3c67b-118">elevatedCount</span></span>|<span data-ttu-id="3c67b-119">int32</span><span class="sxs-lookup"><span data-stu-id="3c67b-119">int32</span></span>|<span data-ttu-id="3c67b-120">O número de usuários que possuem a função atribuída e a função está ativado.</span><span class="sxs-lookup"><span data-stu-id="3c67b-120">The number of users that have the role assigned and the role is activated.</span></span>|
|<span data-ttu-id="3c67b-121">id</span><span class="sxs-lookup"><span data-stu-id="3c67b-121">id</span></span>|<span data-ttu-id="3c67b-122">string</span><span class="sxs-lookup"><span data-stu-id="3c67b-122">string</span></span>| <span data-ttu-id="3c67b-123">O identificador exclusivo para a função.</span><span class="sxs-lookup"><span data-stu-id="3c67b-123">The unique identifier for the role.</span></span> <span data-ttu-id="3c67b-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3c67b-124">Read-only.</span></span>|
|<span data-ttu-id="3c67b-125">managedCount</span><span class="sxs-lookup"><span data-stu-id="3c67b-125">managedCount</span></span>|<span data-ttu-id="3c67b-126">int32</span><span class="sxs-lookup"><span data-stu-id="3c67b-126">int32</span></span>|<span data-ttu-id="3c67b-127">O número de usuários que possuem a função atribuída, mas a função é desativado.</span><span class="sxs-lookup"><span data-stu-id="3c67b-127">The number of users that have the role assigned but the role is deactivated.</span></span>|
|<span data-ttu-id="3c67b-128">mfaEnabled</span><span class="sxs-lookup"><span data-stu-id="3c67b-128">mfaEnabled</span></span>|<span data-ttu-id="3c67b-129">booliano</span><span class="sxs-lookup"><span data-stu-id="3c67b-129">boolean</span></span>|<span data-ttu-id="3c67b-130">**true** se a ativação de função requer MFA.</span><span class="sxs-lookup"><span data-stu-id="3c67b-130">**true** if the role activation requires MFA.</span></span> <span data-ttu-id="3c67b-131">**false** se a ativação de função não exige MFA.</span><span class="sxs-lookup"><span data-stu-id="3c67b-131">**false** if the role activation doesn't require MFA.</span></span>|
|<span data-ttu-id="3c67b-132">status</span><span class="sxs-lookup"><span data-stu-id="3c67b-132">status</span></span>|<span data-ttu-id="3c67b-133">string</span><span class="sxs-lookup"><span data-stu-id="3c67b-133">string</span></span>| <span data-ttu-id="3c67b-134">Os valores possíveis são: `ok` e `bad`.</span><span class="sxs-lookup"><span data-stu-id="3c67b-134">Possible values are: `ok`, `bad`.</span></span> <span data-ttu-id="3c67b-135">O valor depende a proporção entre (managedCount / usersCount).</span><span class="sxs-lookup"><span data-stu-id="3c67b-135">The value depends on the ratio of (managedCount / usersCount).</span></span> <span data-ttu-id="3c67b-136">Se a taxa for menor que um limite predefinido, `ok` é retornado.</span><span class="sxs-lookup"><span data-stu-id="3c67b-136">If the ratio is less than a predefined threshold, `ok` is returned.</span></span> <span data-ttu-id="3c67b-137">Caso contrário, `bad` é retornado.</span><span class="sxs-lookup"><span data-stu-id="3c67b-137">Otherwise, `bad` is returned.</span></span>|
|<span data-ttu-id="3c67b-138">usersCount</span><span class="sxs-lookup"><span data-stu-id="3c67b-138">usersCount</span></span>|<span data-ttu-id="3c67b-139">int32</span><span class="sxs-lookup"><span data-stu-id="3c67b-139">int32</span></span>|<span data-ttu-id="3c67b-140">O número de usuários que são atribuídos com a função.</span><span class="sxs-lookup"><span data-stu-id="3c67b-140">The number of users that are assigned with the role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c67b-141">Relações</span><span class="sxs-lookup"><span data-stu-id="3c67b-141">Relationships</span></span>
<span data-ttu-id="3c67b-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3c67b-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3c67b-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3c67b-143">JSON representation</span></span>

<span data-ttu-id="3c67b-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3c67b-144">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleSummary"
}-->

```json
{
  "elevatedCount": 1024,
  "id": "string (identifier)",
  "managedCount": 1024,
  "mfaEnabled": true,
  "status": "string",
  "usersCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->