---
title: tipo de recurso diário
description: Um diário no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 041de72a3372fd80063b96ba73d10272247c4fdb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503744"
---
# <a name="journal-resource-type"></a><span data-ttu-id="81f58-103">tipo de recurso diário</span><span class="sxs-lookup"><span data-stu-id="81f58-103">journal resource type</span></span>

<span data-ttu-id="81f58-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="81f58-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81f58-105">Representa um diário no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="81f58-105">Represents a journal in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="81f58-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="81f58-106">Methods</span></span>

| <span data-ttu-id="81f58-107">Método</span><span class="sxs-lookup"><span data-stu-id="81f58-107">Method</span></span>                                            |<span data-ttu-id="81f58-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="81f58-108">Return Type</span></span>|<span data-ttu-id="81f58-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="81f58-109">Description</span></span>    |
|:--------------------------------------------------|:----------|:--------------|
|[<span data-ttu-id="81f58-110">Obter diário</span><span class="sxs-lookup"><span data-stu-id="81f58-110">Get journal</span></span>](../api/dynamics-journal-get.md)      |<span data-ttu-id="81f58-111">diário</span><span class="sxs-lookup"><span data-stu-id="81f58-111">journal</span></span>    |<span data-ttu-id="81f58-112">Obtém um diário.</span><span class="sxs-lookup"><span data-stu-id="81f58-112">Gets a journal.</span></span>   |
|[<span data-ttu-id="81f58-113">Diário de lançamentos</span><span class="sxs-lookup"><span data-stu-id="81f58-113">Post journal</span></span>](../api/dynamics-create-journal.md)  |<span data-ttu-id="81f58-114">diário</span><span class="sxs-lookup"><span data-stu-id="81f58-114">journal</span></span>    |<span data-ttu-id="81f58-115">Cria um diário.</span><span class="sxs-lookup"><span data-stu-id="81f58-115">Creates a journal.</span></span>|
|[<span data-ttu-id="81f58-116">Diário de patches</span><span class="sxs-lookup"><span data-stu-id="81f58-116">Patch journal</span></span>](../api/dynamics-journal-update.md) |<span data-ttu-id="81f58-117">diário</span><span class="sxs-lookup"><span data-stu-id="81f58-117">journal</span></span>    |<span data-ttu-id="81f58-118">Atualiza um diário.</span><span class="sxs-lookup"><span data-stu-id="81f58-118">Updates a journal.</span></span>|
|[<span data-ttu-id="81f58-119">Excluir diário</span><span class="sxs-lookup"><span data-stu-id="81f58-119">Delete journal</span></span>](../api/dynamics-journal-delete.md)|<span data-ttu-id="81f58-120">nenhuma</span><span class="sxs-lookup"><span data-stu-id="81f58-120">none</span></span>       |<span data-ttu-id="81f58-121">Exclui um diário.</span><span class="sxs-lookup"><span data-stu-id="81f58-121">Deletes a journal.</span></span>|

## <a name="properties"></a><span data-ttu-id="81f58-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="81f58-122">Properties</span></span>
| <span data-ttu-id="81f58-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81f58-123">Property</span></span>           | <span data-ttu-id="81f58-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="81f58-124">Type</span></span>                  |<span data-ttu-id="81f58-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="81f58-125">Description</span></span>                                           |
|:-------------------|:----------------------|:-----------------------------------------------------|
|<span data-ttu-id="81f58-126">id</span><span class="sxs-lookup"><span data-stu-id="81f58-126">id</span></span>                  |<span data-ttu-id="81f58-127">GUID</span><span class="sxs-lookup"><span data-stu-id="81f58-127">GUID</span></span>                   |<span data-ttu-id="81f58-128">A ID exclusiva do diário.</span><span class="sxs-lookup"><span data-stu-id="81f58-128">The unique ID of the journal.</span></span> <span data-ttu-id="81f58-129">Não editável.</span><span class="sxs-lookup"><span data-stu-id="81f58-129">Non-editable.</span></span>           |
|<span data-ttu-id="81f58-130">código</span><span class="sxs-lookup"><span data-stu-id="81f58-130">code</span></span>                |<span data-ttu-id="81f58-131">Cadeia de caracteres, tamanho máximo 10</span><span class="sxs-lookup"><span data-stu-id="81f58-131">string, maximum size 10</span></span>| <span data-ttu-id="81f58-132">O código do diário.</span><span class="sxs-lookup"><span data-stu-id="81f58-132">The code of the journal.</span></span>                             |
|<span data-ttu-id="81f58-133">displayName</span><span class="sxs-lookup"><span data-stu-id="81f58-133">displayName</span></span>         |<span data-ttu-id="81f58-134">Cadeia de caracteres, tamanho máximo 50</span><span class="sxs-lookup"><span data-stu-id="81f58-134">string, maximum size 50</span></span>| <span data-ttu-id="81f58-135">O nome de exibição do diário.</span><span class="sxs-lookup"><span data-stu-id="81f58-135">The display name of the journal.</span></span>                     |
|<span data-ttu-id="81f58-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="81f58-136">lastModifiedDateTime</span></span>|<span data-ttu-id="81f58-137">datetime</span><span class="sxs-lookup"><span data-stu-id="81f58-137">datetime</span></span>               |<span data-ttu-id="81f58-138">O último DateTime que o diário foi modificado.</span><span class="sxs-lookup"><span data-stu-id="81f58-138">The last datetime the journal was modified.</span></span> <span data-ttu-id="81f58-139">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="81f58-139">Read-Only.</span></span>|

## <a name="bound-actions"></a><span data-ttu-id="81f58-140">Ações associadas</span><span class="sxs-lookup"><span data-stu-id="81f58-140">Bound actions</span></span>
<span data-ttu-id="81f58-141">O tipo de recurso diário oferece uma ação associada `post` chamada que envia o lote de diário geral correspondente.</span><span class="sxs-lookup"><span data-stu-id="81f58-141">The journal resource type offers a bound action called `post` which posts the corresponding general journal batch.</span></span>

<span data-ttu-id="81f58-142">O lançamento do lote de diário geral é ilustrado no exemplo a seguir:</span><span class="sxs-lookup"><span data-stu-id="81f58-142">Posting the general journal batch is illustrated in the following example:</span></span>  
<span data-ttu-id="81f58-143">`POST https://graph.microsoft.com/beta/financials/companies{id}/journals{id}/post`.</span><span class="sxs-lookup"><span data-stu-id="81f58-143">`POST https://graph.microsoft.com/beta/financials/companies{id}/journals{id}/post`.</span></span>

<span data-ttu-id="81f58-144">A resposta não tem conteúdo; o código de resposta é 204.</span><span class="sxs-lookup"><span data-stu-id="81f58-144">The response has no content; the response code is 204.</span></span>

## <a name="json-representation"></a><span data-ttu-id="81f58-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="81f58-145">JSON representation</span></span>

<span data-ttu-id="81f58-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="81f58-146">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}
```

