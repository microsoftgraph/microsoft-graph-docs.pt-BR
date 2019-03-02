---
title: tipo de recurso generalLedgerEntries
description: Uma entrada de contabilidade no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 0a5701451bf96773428b12b6bb715320e2ba81b5
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365756"
---
# <a name="generalledgerentries-resource-type"></a><span data-ttu-id="a3c68-103">tipo de recurso generalLedgerEntries</span><span class="sxs-lookup"><span data-stu-id="a3c68-103">generalLedgerEntries resource type</span></span>
<span data-ttu-id="a3c68-104">Representa um objeto generalLedgerEntry no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="a3c68-104">Represents a generalLedgerEntry object in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="a3c68-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="a3c68-105">Methods</span></span>

| <span data-ttu-id="a3c68-106">Método</span><span class="sxs-lookup"><span data-stu-id="a3c68-106">Method</span></span>       | <span data-ttu-id="a3c68-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a3c68-107">Return Type</span></span>  |<span data-ttu-id="a3c68-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3c68-108">Description</span></span>|
|:-------------|:-------------|:----------|
|[<span data-ttu-id="a3c68-109">Obter generalLedgerEntries</span><span class="sxs-lookup"><span data-stu-id="a3c68-109">Get generalLedgerEntries</span></span>](../api/dynamics-generalledgerentries-get.md)|<span data-ttu-id="a3c68-110">generalLedgerEntries</span><span class="sxs-lookup"><span data-stu-id="a3c68-110">generalLedgerEntries</span></span>|<span data-ttu-id="a3c68-111">Obter um objeto de entrada G/L.</span><span class="sxs-lookup"><span data-stu-id="a3c68-111">Get a G/L entry object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a3c68-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a3c68-112">Properties</span></span>
| <span data-ttu-id="a3c68-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a3c68-113">Property</span></span>           | <span data-ttu-id="a3c68-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3c68-114">Type</span></span>                  |<span data-ttu-id="a3c68-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3c68-115">Description</span></span>                                  |
|:-------------------|:----------------------|:--------------------------------------------|
|<span data-ttu-id="a3c68-116">id</span><span class="sxs-lookup"><span data-stu-id="a3c68-116">id</span></span>                  |<span data-ttu-id="a3c68-117">numéricos</span><span class="sxs-lookup"><span data-stu-id="a3c68-117">numeric</span></span>                |<span data-ttu-id="a3c68-118">A identificação exclusiva da entrada G/L.</span><span class="sxs-lookup"><span data-stu-id="a3c68-118">The unique ID of the G/L Entry.</span></span>              |
|<span data-ttu-id="a3c68-119">postingDate</span><span class="sxs-lookup"><span data-stu-id="a3c68-119">postingDate</span></span>         |<span data-ttu-id="a3c68-120">data</span><span class="sxs-lookup"><span data-stu-id="a3c68-120">date</span></span>                   |<span data-ttu-id="a3c68-121">Especifica a data de lançamento da entrada G/L.</span><span class="sxs-lookup"><span data-stu-id="a3c68-121">Specifies the posting date of the G/L Entry.</span></span> |
|<span data-ttu-id="a3c68-122">documentNumber</span><span class="sxs-lookup"><span data-stu-id="a3c68-122">documentNumber</span></span>      |<span data-ttu-id="a3c68-123">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="a3c68-123">string, maximum size 20</span></span>|<span data-ttu-id="a3c68-124">Especifica o número do documento da entrada G/L.</span><span class="sxs-lookup"><span data-stu-id="a3c68-124">Specifies the document number of the G/L Entry.</span></span>|
|<span data-ttu-id="a3c68-125">documentType</span><span class="sxs-lookup"><span data-stu-id="a3c68-125">documentType</span></span>        |<span data-ttu-id="a3c68-126">string</span><span class="sxs-lookup"><span data-stu-id="a3c68-126">string</span></span>                 |<span data-ttu-id="a3c68-127">Especifica o tipo de documento da entrada G/L.</span><span class="sxs-lookup"><span data-stu-id="a3c68-127">Specifies the document type of the G/L Entry.</span></span>|
|<span data-ttu-id="a3c68-128">accountId</span><span class="sxs-lookup"><span data-stu-id="a3c68-128">accountId</span></span>           |<span data-ttu-id="a3c68-129">GUID</span><span class="sxs-lookup"><span data-stu-id="a3c68-129">GUID</span></span>                   |<span data-ttu-id="a3c68-130">Especifica a AccountId da entrada G/L.</span><span class="sxs-lookup"><span data-stu-id="a3c68-130">Specifies the accountId of the G/L Entry.</span></span>    |
|<span data-ttu-id="a3c68-131">accountNumber</span><span class="sxs-lookup"><span data-stu-id="a3c68-131">accountNumber</span></span>       |<span data-ttu-id="a3c68-132">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="a3c68-132">string, maximum size 20</span></span>|<span data-ttu-id="a3c68-133">Especifica o accountNumber da entrada G/L.</span><span class="sxs-lookup"><span data-stu-id="a3c68-133">Specifies the accountNumber of the G/L Entry.</span></span>|
|<span data-ttu-id="a3c68-134">description</span><span class="sxs-lookup"><span data-stu-id="a3c68-134">description</span></span>         |<span data-ttu-id="a3c68-135">Cadeia de caracteres, tamanho máximo 50</span><span class="sxs-lookup"><span data-stu-id="a3c68-135">string, maximum size 50</span></span>|<span data-ttu-id="a3c68-136">Especifica a descrição da entrada G/L.</span><span class="sxs-lookup"><span data-stu-id="a3c68-136">Specifies the description of the G/L Entry.</span></span>  |
|<span data-ttu-id="a3c68-137">debitAmount</span><span class="sxs-lookup"><span data-stu-id="a3c68-137">debitAmount</span></span>         |<span data-ttu-id="a3c68-138">numéricos</span><span class="sxs-lookup"><span data-stu-id="a3c68-138">numeric</span></span>                |<span data-ttu-id="a3c68-139">Especifica o debitAmount da entrada G/L.</span><span class="sxs-lookup"><span data-stu-id="a3c68-139">Specifies the debitAmount of the G/L Entry.</span></span>  |
|<span data-ttu-id="a3c68-140">creditAmount</span><span class="sxs-lookup"><span data-stu-id="a3c68-140">creditAmount</span></span>        |<span data-ttu-id="a3c68-141">numéricos</span><span class="sxs-lookup"><span data-stu-id="a3c68-141">numeric</span></span>                |<span data-ttu-id="a3c68-142">Especifica o creditAmount da entrada G/L.</span><span class="sxs-lookup"><span data-stu-id="a3c68-142">Specifies the creditAmount of the G/L Entry.</span></span> |
|<span data-ttu-id="a3c68-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a3c68-143">lastModifiedDateTime</span></span>|<span data-ttu-id="a3c68-144">DateTime</span><span class="sxs-lookup"><span data-stu-id="a3c68-144">datetime</span></span>               |<span data-ttu-id="a3c68-145">A última data/hora em que a entrada G/L foi modificada.</span><span class="sxs-lookup"><span data-stu-id="a3c68-145">The last datetime the G/L Entry was modified.</span></span>|


## <a name="relationships"></a><span data-ttu-id="a3c68-146">Relações</span><span class="sxs-lookup"><span data-stu-id="a3c68-146">Relationships</span></span>
<span data-ttu-id="a3c68-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a3c68-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3c68-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a3c68-148">JSON representation</span></span>

<span data-ttu-id="a3c68-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a3c68-149">Here is a JSON representation of the resource.</span></span>


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

