---
title: tipo de recurso diário
description: Um diário no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: ecbeba91828ba06b9927af08ac8d75a177e27cea
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013829"
---
# <a name="journal-resource-type"></a><span data-ttu-id="87dfa-103">tipo de recurso diário</span><span class="sxs-lookup"><span data-stu-id="87dfa-103">journal resource type</span></span>

<span data-ttu-id="87dfa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87dfa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87dfa-105">Representa um diário no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="87dfa-105">Represents a journal in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="87dfa-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="87dfa-106">Methods</span></span>

| <span data-ttu-id="87dfa-107">Método</span><span class="sxs-lookup"><span data-stu-id="87dfa-107">Method</span></span>                                            |<span data-ttu-id="87dfa-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="87dfa-108">Return Type</span></span>|<span data-ttu-id="87dfa-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="87dfa-109">Description</span></span>    |
|:--------------------------------------------------|:----------|:--------------|
|[<span data-ttu-id="87dfa-110">Obter diário</span><span class="sxs-lookup"><span data-stu-id="87dfa-110">Get journal</span></span>](../api/dynamics-journal-get.md)      |<span data-ttu-id="87dfa-111">diário</span><span class="sxs-lookup"><span data-stu-id="87dfa-111">journal</span></span>    |<span data-ttu-id="87dfa-112">Obtém um diário.</span><span class="sxs-lookup"><span data-stu-id="87dfa-112">Gets a journal.</span></span>   |
|[<span data-ttu-id="87dfa-113">Diário de lançamentos</span><span class="sxs-lookup"><span data-stu-id="87dfa-113">Post journal</span></span>](../api/dynamics-create-journal.md)  |<span data-ttu-id="87dfa-114">diário</span><span class="sxs-lookup"><span data-stu-id="87dfa-114">journal</span></span>    |<span data-ttu-id="87dfa-115">Cria um diário.</span><span class="sxs-lookup"><span data-stu-id="87dfa-115">Creates a journal.</span></span>|
|[<span data-ttu-id="87dfa-116">Diário de patches</span><span class="sxs-lookup"><span data-stu-id="87dfa-116">Patch journal</span></span>](../api/dynamics-journal-update.md) |<span data-ttu-id="87dfa-117">diário</span><span class="sxs-lookup"><span data-stu-id="87dfa-117">journal</span></span>    |<span data-ttu-id="87dfa-118">Atualiza um diário.</span><span class="sxs-lookup"><span data-stu-id="87dfa-118">Updates a journal.</span></span>|
|[<span data-ttu-id="87dfa-119">Excluir diário</span><span class="sxs-lookup"><span data-stu-id="87dfa-119">Delete journal</span></span>](../api/dynamics-journal-delete.md)|<span data-ttu-id="87dfa-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="87dfa-120">none</span></span>       |<span data-ttu-id="87dfa-121">Exclui um diário.</span><span class="sxs-lookup"><span data-stu-id="87dfa-121">Deletes a journal.</span></span>|

## <a name="properties"></a><span data-ttu-id="87dfa-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="87dfa-122">Properties</span></span>
| <span data-ttu-id="87dfa-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87dfa-123">Property</span></span>           | <span data-ttu-id="87dfa-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="87dfa-124">Type</span></span>                  |<span data-ttu-id="87dfa-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="87dfa-125">Description</span></span>                                           |
|:-------------------|:----------------------|:-----------------------------------------------------|
|<span data-ttu-id="87dfa-126">id</span><span class="sxs-lookup"><span data-stu-id="87dfa-126">id</span></span>                  |<span data-ttu-id="87dfa-127">GUID</span><span class="sxs-lookup"><span data-stu-id="87dfa-127">GUID</span></span>                   |<span data-ttu-id="87dfa-128">A ID exclusiva do diário.</span><span class="sxs-lookup"><span data-stu-id="87dfa-128">The unique ID of the journal.</span></span> <span data-ttu-id="87dfa-129">Não editável.</span><span class="sxs-lookup"><span data-stu-id="87dfa-129">Non-editable.</span></span>           |
|<span data-ttu-id="87dfa-130">código</span><span class="sxs-lookup"><span data-stu-id="87dfa-130">code</span></span>                |<span data-ttu-id="87dfa-131">Cadeia de caracteres, tamanho máximo 10</span><span class="sxs-lookup"><span data-stu-id="87dfa-131">string, maximum size 10</span></span>| <span data-ttu-id="87dfa-132">O código do diário.</span><span class="sxs-lookup"><span data-stu-id="87dfa-132">The code of the journal.</span></span>                             |
|<span data-ttu-id="87dfa-133">Nome para exibição</span><span class="sxs-lookup"><span data-stu-id="87dfa-133">displayName</span></span>         |<span data-ttu-id="87dfa-134">Cadeia de caracteres, tamanho máximo 50</span><span class="sxs-lookup"><span data-stu-id="87dfa-134">string, maximum size 50</span></span>| <span data-ttu-id="87dfa-135">O nome de exibição do diário.</span><span class="sxs-lookup"><span data-stu-id="87dfa-135">The display name of the journal.</span></span>                     |
|<span data-ttu-id="87dfa-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="87dfa-136">lastModifiedDateTime</span></span>|<span data-ttu-id="87dfa-137">datetime</span><span class="sxs-lookup"><span data-stu-id="87dfa-137">datetime</span></span>               |<span data-ttu-id="87dfa-138">O último DateTime que o diário foi modificado.</span><span class="sxs-lookup"><span data-stu-id="87dfa-138">The last datetime the journal was modified.</span></span> <span data-ttu-id="87dfa-139">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="87dfa-139">Read-Only.</span></span>|

## <a name="bound-actions"></a><span data-ttu-id="87dfa-140">Ações associadas</span><span class="sxs-lookup"><span data-stu-id="87dfa-140">Bound actions</span></span>
<span data-ttu-id="87dfa-141">O tipo de recurso diário oferece uma ação associada chamada `post` que envia o lote de diário geral correspondente.</span><span class="sxs-lookup"><span data-stu-id="87dfa-141">The journal resource type offers a bound action called `post` which posts the corresponding general journal batch.</span></span>

<span data-ttu-id="87dfa-142">O lançamento do lote de diário geral é ilustrado no exemplo a seguir:</span><span class="sxs-lookup"><span data-stu-id="87dfa-142">Posting the general journal batch is illustrated in the following example:</span></span>  
<span data-ttu-id="87dfa-143">`POST https://graph.microsoft.com/beta/financials/companies{id}/journals{id}/post`.</span><span class="sxs-lookup"><span data-stu-id="87dfa-143">`POST https://graph.microsoft.com/beta/financials/companies{id}/journals{id}/post`.</span></span>

<span data-ttu-id="87dfa-144">A resposta não tem conteúdo; o código de resposta é 204.</span><span class="sxs-lookup"><span data-stu-id="87dfa-144">The response has no content; the response code is 204.</span></span>

## <a name="json-representation"></a><span data-ttu-id="87dfa-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="87dfa-145">JSON representation</span></span>

<span data-ttu-id="87dfa-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="87dfa-146">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}
```



