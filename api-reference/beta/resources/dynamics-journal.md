---
title: tipo de recurso diário
description: Um diário no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 7cfc723a4370c2b30440dcd4e33b50ed066ac89b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006589"
---
# <a name="journal-resource-type"></a><span data-ttu-id="9f032-103">tipo de recurso diário</span><span class="sxs-lookup"><span data-stu-id="9f032-103">journal resource type</span></span>
<span data-ttu-id="9f032-104">Representa um diário no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="9f032-104">Represents a journal in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="9f032-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="9f032-105">Methods</span></span>

| <span data-ttu-id="9f032-106">Método</span><span class="sxs-lookup"><span data-stu-id="9f032-106">Method</span></span>                                            |<span data-ttu-id="9f032-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9f032-107">Return Type</span></span>|<span data-ttu-id="9f032-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f032-108">Description</span></span>    |
|:--------------------------------------------------|:----------|:--------------|
|[<span data-ttu-id="9f032-109">Obter diário</span><span class="sxs-lookup"><span data-stu-id="9f032-109">Get journal</span></span>](../api/dynamics-journal-get.md)      |<span data-ttu-id="9f032-110">diário</span><span class="sxs-lookup"><span data-stu-id="9f032-110">journal</span></span>    |<span data-ttu-id="9f032-111">Obtém um diário.</span><span class="sxs-lookup"><span data-stu-id="9f032-111">Gets a journal.</span></span>   |
|[<span data-ttu-id="9f032-112">Diário de lançamentos</span><span class="sxs-lookup"><span data-stu-id="9f032-112">Post journal</span></span>](../api/dynamics-create-journal.md)  |<span data-ttu-id="9f032-113">diário</span><span class="sxs-lookup"><span data-stu-id="9f032-113">journal</span></span>    |<span data-ttu-id="9f032-114">Cria um diário.</span><span class="sxs-lookup"><span data-stu-id="9f032-114">Creates a journal.</span></span>|
|[<span data-ttu-id="9f032-115">Diário de patches</span><span class="sxs-lookup"><span data-stu-id="9f032-115">Patch journal</span></span>](../api/dynamics-journal-update.md) |<span data-ttu-id="9f032-116">diário</span><span class="sxs-lookup"><span data-stu-id="9f032-116">journal</span></span>    |<span data-ttu-id="9f032-117">Atualiza um diário.</span><span class="sxs-lookup"><span data-stu-id="9f032-117">Updates a journal.</span></span>|
|[<span data-ttu-id="9f032-118">Excluir diário</span><span class="sxs-lookup"><span data-stu-id="9f032-118">Delete journal</span></span>](../api/dynamics-journal-delete.md)|<span data-ttu-id="9f032-119">none</span><span class="sxs-lookup"><span data-stu-id="9f032-119">none</span></span>       |<span data-ttu-id="9f032-120">Exclui um diário.</span><span class="sxs-lookup"><span data-stu-id="9f032-120">Deletes a journal.</span></span>|

## <a name="properties"></a><span data-ttu-id="9f032-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9f032-121">Properties</span></span>
| <span data-ttu-id="9f032-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9f032-122">Property</span></span>           | <span data-ttu-id="9f032-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f032-123">Type</span></span>                  |<span data-ttu-id="9f032-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f032-124">Description</span></span>                                           |
|:-------------------|:----------------------|:-----------------------------------------------------|
|<span data-ttu-id="9f032-125">id</span><span class="sxs-lookup"><span data-stu-id="9f032-125">id</span></span>                  |<span data-ttu-id="9f032-126">GUID</span><span class="sxs-lookup"><span data-stu-id="9f032-126">GUID</span></span>                   |<span data-ttu-id="9f032-127">A ID exclusiva do diário.</span><span class="sxs-lookup"><span data-stu-id="9f032-127">The unique ID of the journal.</span></span> <span data-ttu-id="9f032-128">Não editável.</span><span class="sxs-lookup"><span data-stu-id="9f032-128">Non-editable.</span></span>           |
|<span data-ttu-id="9f032-129">código</span><span class="sxs-lookup"><span data-stu-id="9f032-129">code</span></span>                |<span data-ttu-id="9f032-130">Cadeia de caracteres, tamanho máximo 10</span><span class="sxs-lookup"><span data-stu-id="9f032-130">string, maximum size 10</span></span>| <span data-ttu-id="9f032-131">O código do diário.</span><span class="sxs-lookup"><span data-stu-id="9f032-131">The code of the journal.</span></span>                             |
|<span data-ttu-id="9f032-132">displayName</span><span class="sxs-lookup"><span data-stu-id="9f032-132">displayName</span></span>         |<span data-ttu-id="9f032-133">Cadeia de caracteres, tamanho máximo 50</span><span class="sxs-lookup"><span data-stu-id="9f032-133">string, maximum size 50</span></span>| <span data-ttu-id="9f032-134">O nome de exibição do diário.</span><span class="sxs-lookup"><span data-stu-id="9f032-134">The display name of the journal.</span></span>                     |
|<span data-ttu-id="9f032-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f032-135">lastModifiedDateTime</span></span>|<span data-ttu-id="9f032-136">DateTime</span><span class="sxs-lookup"><span data-stu-id="9f032-136">datetime</span></span>               |<span data-ttu-id="9f032-137">O último DateTime que o diário foi modificado.</span><span class="sxs-lookup"><span data-stu-id="9f032-137">The last datetime the journal was modified.</span></span> <span data-ttu-id="9f032-138">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="9f032-138">Read-Only.</span></span>|

## <a name="bound-actions"></a><span data-ttu-id="9f032-139">Ações associadas</span><span class="sxs-lookup"><span data-stu-id="9f032-139">Bound actions</span></span>
<span data-ttu-id="9f032-140">O tipo de recurso diário oferece uma ação associada `post` chamada que envia o lote de diário geral correspondente.</span><span class="sxs-lookup"><span data-stu-id="9f032-140">The journal resource type offers a bound action called `post` which posts the corresponding general journal batch.</span></span>

<span data-ttu-id="9f032-141">O lançamento do lote de diário geral é ilustrado no exemplo a seguir:</span><span class="sxs-lookup"><span data-stu-id="9f032-141">Posting the general journal batch is illustrated in the following example:</span></span>  
<span data-ttu-id="9f032-142">`POST https://graph.microsoft.com/beta/financials/companies{id}/journals{id}/post`.</span><span class="sxs-lookup"><span data-stu-id="9f032-142"></span></span>

<span data-ttu-id="9f032-143">A resposta não tem conteúdo; o código de resposta é 204.</span><span class="sxs-lookup"><span data-stu-id="9f032-143">The response has no content; the response code is 204.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9f032-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9f032-144">JSON representation</span></span>

<span data-ttu-id="9f032-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9f032-145">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}
```

