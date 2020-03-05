---
title: tipo de recurso generalLedgerEntries
description: Uma entrada de contabilidade no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: f1dc4ec7bb3fa30f7dc6362c850893953c4aa6aa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503975"
---
# <a name="generalledgerentries-resource-type"></a><span data-ttu-id="dca7d-103">tipo de recurso generalLedgerEntries</span><span class="sxs-lookup"><span data-stu-id="dca7d-103">generalLedgerEntries resource type</span></span>

<span data-ttu-id="dca7d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="dca7d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dca7d-105">Representa um objeto generalLedgerEntry no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="dca7d-105">Represents a generalLedgerEntry object in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="dca7d-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="dca7d-106">Methods</span></span>

| <span data-ttu-id="dca7d-107">Método</span><span class="sxs-lookup"><span data-stu-id="dca7d-107">Method</span></span>       | <span data-ttu-id="dca7d-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="dca7d-108">Return Type</span></span>  |<span data-ttu-id="dca7d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="dca7d-109">Description</span></span>|
|:-------------|:-------------|:----------|
|[<span data-ttu-id="dca7d-110">Obter generalLedgerEntries</span><span class="sxs-lookup"><span data-stu-id="dca7d-110">Get generalLedgerEntries</span></span>](../api/dynamics-generalledgerentries-get.md)|<span data-ttu-id="dca7d-111">generalLedgerEntries</span><span class="sxs-lookup"><span data-stu-id="dca7d-111">generalLedgerEntries</span></span>|<span data-ttu-id="dca7d-112">Obter um objeto de entrada G/L.</span><span class="sxs-lookup"><span data-stu-id="dca7d-112">Get a G/L entry object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dca7d-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dca7d-113">Properties</span></span>
| <span data-ttu-id="dca7d-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dca7d-114">Property</span></span>           | <span data-ttu-id="dca7d-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="dca7d-115">Type</span></span>                  |<span data-ttu-id="dca7d-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="dca7d-116">Description</span></span>                                  |
|:-------------------|:----------------------|:--------------------------------------------|
|<span data-ttu-id="dca7d-117">id</span><span class="sxs-lookup"><span data-stu-id="dca7d-117">id</span></span>                  |<span data-ttu-id="dca7d-118">numéricos</span><span class="sxs-lookup"><span data-stu-id="dca7d-118">numeric</span></span>                |<span data-ttu-id="dca7d-119">A identificação exclusiva da entrada G/L.</span><span class="sxs-lookup"><span data-stu-id="dca7d-119">The unique ID of the G/L Entry.</span></span>              |
|<span data-ttu-id="dca7d-120">postingDate</span><span class="sxs-lookup"><span data-stu-id="dca7d-120">postingDate</span></span>         |<span data-ttu-id="dca7d-121">data</span><span class="sxs-lookup"><span data-stu-id="dca7d-121">date</span></span>                   |<span data-ttu-id="dca7d-122">Especifica a data de lançamento da entrada G/L.</span><span class="sxs-lookup"><span data-stu-id="dca7d-122">Specifies the posting date of the G/L Entry.</span></span> |
|<span data-ttu-id="dca7d-123">documentNumber</span><span class="sxs-lookup"><span data-stu-id="dca7d-123">documentNumber</span></span>      |<span data-ttu-id="dca7d-124">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="dca7d-124">string, maximum size 20</span></span>|<span data-ttu-id="dca7d-125">Especifica o número do documento da entrada G/L.</span><span class="sxs-lookup"><span data-stu-id="dca7d-125">Specifies the document number of the G/L Entry.</span></span>|
|<span data-ttu-id="dca7d-126">documentType</span><span class="sxs-lookup"><span data-stu-id="dca7d-126">documentType</span></span>        |<span data-ttu-id="dca7d-127">string</span><span class="sxs-lookup"><span data-stu-id="dca7d-127">string</span></span>                 |<span data-ttu-id="dca7d-128">Especifica o tipo de documento da entrada G/L.</span><span class="sxs-lookup"><span data-stu-id="dca7d-128">Specifies the document type of the G/L Entry.</span></span>|
|<span data-ttu-id="dca7d-129">accountId</span><span class="sxs-lookup"><span data-stu-id="dca7d-129">accountId</span></span>           |<span data-ttu-id="dca7d-130">GUID</span><span class="sxs-lookup"><span data-stu-id="dca7d-130">GUID</span></span>                   |<span data-ttu-id="dca7d-131">Especifica a AccountId da entrada G/L.</span><span class="sxs-lookup"><span data-stu-id="dca7d-131">Specifies the accountId of the G/L Entry.</span></span>    |
|<span data-ttu-id="dca7d-132">accountNumber</span><span class="sxs-lookup"><span data-stu-id="dca7d-132">accountNumber</span></span>       |<span data-ttu-id="dca7d-133">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="dca7d-133">string, maximum size 20</span></span>|<span data-ttu-id="dca7d-134">Especifica o accountNumber da entrada G/L.</span><span class="sxs-lookup"><span data-stu-id="dca7d-134">Specifies the accountNumber of the G/L Entry.</span></span>|
|<span data-ttu-id="dca7d-135">description</span><span class="sxs-lookup"><span data-stu-id="dca7d-135">description</span></span>         |<span data-ttu-id="dca7d-136">Cadeia de caracteres, tamanho máximo 50</span><span class="sxs-lookup"><span data-stu-id="dca7d-136">string, maximum size 50</span></span>|<span data-ttu-id="dca7d-137">Especifica a descrição da entrada G/L.</span><span class="sxs-lookup"><span data-stu-id="dca7d-137">Specifies the description of the G/L Entry.</span></span>  |
|<span data-ttu-id="dca7d-138">debitAmount</span><span class="sxs-lookup"><span data-stu-id="dca7d-138">debitAmount</span></span>         |<span data-ttu-id="dca7d-139">numéricos</span><span class="sxs-lookup"><span data-stu-id="dca7d-139">numeric</span></span>                |<span data-ttu-id="dca7d-140">Especifica o debitAmount da entrada G/L.</span><span class="sxs-lookup"><span data-stu-id="dca7d-140">Specifies the debitAmount of the G/L Entry.</span></span>  |
|<span data-ttu-id="dca7d-141">creditAmount</span><span class="sxs-lookup"><span data-stu-id="dca7d-141">creditAmount</span></span>        |<span data-ttu-id="dca7d-142">numéricos</span><span class="sxs-lookup"><span data-stu-id="dca7d-142">numeric</span></span>                |<span data-ttu-id="dca7d-143">Especifica o creditAmount da entrada G/L.</span><span class="sxs-lookup"><span data-stu-id="dca7d-143">Specifies the creditAmount of the G/L Entry.</span></span> |
|<span data-ttu-id="dca7d-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dca7d-144">lastModifiedDateTime</span></span>|<span data-ttu-id="dca7d-145">datetime</span><span class="sxs-lookup"><span data-stu-id="dca7d-145">datetime</span></span>               |<span data-ttu-id="dca7d-146">A última data/hora em que a entrada G/L foi modificada.</span><span class="sxs-lookup"><span data-stu-id="dca7d-146">The last datetime the G/L Entry was modified.</span></span>|


## <a name="relationships"></a><span data-ttu-id="dca7d-147">Relações</span><span class="sxs-lookup"><span data-stu-id="dca7d-147">Relationships</span></span>
<span data-ttu-id="dca7d-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dca7d-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dca7d-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dca7d-149">JSON representation</span></span>

<span data-ttu-id="dca7d-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dca7d-150">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "int",
  "postingDate": "Date",
  "documentNumber": "string",
  "documentType": "string",
  "accountId": "GUID",
  "accountNumber": "string",
  "description": "string",
  "debitAmount": "decimal",
  "creditAmount": "decimal",
  "lastModifiedDateTime": "datetime"
}

```

