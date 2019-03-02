---
title: tipo de recurso de contas
description: Um objeto Account no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4252c20e9d11f67a6de40871b1649a165cbd787c
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365455"
---
# <a name="accounts-resource-type"></a><span data-ttu-id="2063f-103">tipo de recurso de contas</span><span class="sxs-lookup"><span data-stu-id="2063f-103">accounts resource type</span></span>
<span data-ttu-id="2063f-104">Representa um objeto Account no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="2063f-104">Represents an account object in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="2063f-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="2063f-105">Methods</span></span>

| <span data-ttu-id="2063f-106">Método</span><span class="sxs-lookup"><span data-stu-id="2063f-106">Method</span></span>       | <span data-ttu-id="2063f-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2063f-107">Return Type</span></span>  |<span data-ttu-id="2063f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="2063f-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2063f-109">Obter contas</span><span class="sxs-lookup"><span data-stu-id="2063f-109">Get accounts</span></span>](../api/dynamics-account-get.md)|<span data-ttu-id="2063f-110">las</span><span class="sxs-lookup"><span data-stu-id="2063f-110">accounts</span></span>|<span data-ttu-id="2063f-111">Obtém o objeto accounts.</span><span class="sxs-lookup"><span data-stu-id="2063f-111">Get accounts object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2063f-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2063f-112">Properties</span></span>
| <span data-ttu-id="2063f-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2063f-113">Property</span></span>     | <span data-ttu-id="2063f-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="2063f-114">Type</span></span>   |<span data-ttu-id="2063f-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="2063f-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2063f-116">id</span><span class="sxs-lookup"><span data-stu-id="2063f-116">id</span></span>|<span data-ttu-id="2063f-117">GUID</span><span class="sxs-lookup"><span data-stu-id="2063f-117">GUID</span></span>|<span data-ttu-id="2063f-118">A identificação exclusiva da conta.</span><span class="sxs-lookup"><span data-stu-id="2063f-118">The unique ID of the account.</span></span>|
|<span data-ttu-id="2063f-119">number</span><span class="sxs-lookup"><span data-stu-id="2063f-119">number</span></span>|<span data-ttu-id="2063f-120">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="2063f-120">string, maximum size 20</span></span>|<span data-ttu-id="2063f-121">Especifica o número da conta G/L.</span><span class="sxs-lookup"><span data-stu-id="2063f-121">Specifies the number of the G/L account.</span></span>|
|<span data-ttu-id="2063f-122">displayName</span><span class="sxs-lookup"><span data-stu-id="2063f-122">displayName</span></span>|<span data-ttu-id="2063f-123">Cadeia de caracteres, tamanho máximo 50</span><span class="sxs-lookup"><span data-stu-id="2063f-123">string, maximum size 50</span></span>|<span data-ttu-id="2063f-124">Especifica o nome da conta de G/L.</span><span class="sxs-lookup"><span data-stu-id="2063f-124">Specifies the name of the G/L account.</span></span>|
|<span data-ttu-id="2063f-125">category</span><span class="sxs-lookup"><span data-stu-id="2063f-125">category</span></span>|<span data-ttu-id="2063f-126">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="2063f-126">string, maximum size 20</span></span>|<span data-ttu-id="2063f-127">Especifica a categoria da conta de G/L.</span><span class="sxs-lookup"><span data-stu-id="2063f-127">Specifies the category of the G/L account.</span></span>|
|<span data-ttu-id="2063f-128">Subcategoria</span><span class="sxs-lookup"><span data-stu-id="2063f-128">subCategory</span></span>|<span data-ttu-id="2063f-129">Cadeia de caracteres, tamanho máximo 80</span><span class="sxs-lookup"><span data-stu-id="2063f-129">string, maximum size 80</span></span>|<span data-ttu-id="2063f-130">Especifica a subcategoria da categoria de conta da conta G/L.</span><span class="sxs-lookup"><span data-stu-id="2063f-130">Specifies the subcategory of the account category of the G/L account.</span></span>|
|<span data-ttu-id="2063f-131">bloqueou</span><span class="sxs-lookup"><span data-stu-id="2063f-131">blocked</span></span>|<span data-ttu-id="2063f-132">boolean</span><span class="sxs-lookup"><span data-stu-id="2063f-132">boolean</span></span>|<span data-ttu-id="2063f-133">Especifica que não é possível postar entradas na conta G/L.</span><span class="sxs-lookup"><span data-stu-id="2063f-133">Specifies that entries cannot be posted to the G/L account.</span></span> <span data-ttu-id="2063f-134">**True** indica que a conta está bloqueada e o lançamento não é permitido.</span><span class="sxs-lookup"><span data-stu-id="2063f-134">**True** indicates account is blocked and posting is not allowed.</span></span>|
|<span data-ttu-id="2063f-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2063f-135">lastModifiedDateTime</span></span>|<span data-ttu-id="2063f-136">DateTime</span><span class="sxs-lookup"><span data-stu-id="2063f-136">datetime</span></span>|<span data-ttu-id="2063f-137">O último DateTime que a conta foi modificada.</span><span class="sxs-lookup"><span data-stu-id="2063f-137">The last datetime the account was modified.</span></span>|


## <a name="relationships"></a><span data-ttu-id="2063f-138">Relações</span><span class="sxs-lookup"><span data-stu-id="2063f-138">Relationships</span></span>
<span data-ttu-id="2063f-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2063f-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2063f-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2063f-140">JSON representation</span></span>

<span data-ttu-id="2063f-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2063f-141">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "GUID",
  "number": "string",
  "displayName": "string",
  "category": "string",
  "subCategory": "string",
  "blocked": "boolean",
  "lastModifiedDateTime": "datetime"
}

```
