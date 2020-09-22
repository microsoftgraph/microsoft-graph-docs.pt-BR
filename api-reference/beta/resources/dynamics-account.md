---
title: tipo de recurso de contas
description: Um objeto Account no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 671d81da52b28558fa5c24b13060b766c8d908c9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076453"
---
# <a name="accounts-resource-type"></a><span data-ttu-id="c9d82-103">tipo de recurso de contas</span><span class="sxs-lookup"><span data-stu-id="c9d82-103">accounts resource type</span></span>

<span data-ttu-id="c9d82-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9d82-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9d82-105">Representa um objeto Account no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="c9d82-105">Represents an account object in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="c9d82-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="c9d82-106">Methods</span></span>

| <span data-ttu-id="c9d82-107">Método</span><span class="sxs-lookup"><span data-stu-id="c9d82-107">Method</span></span>       | <span data-ttu-id="c9d82-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c9d82-108">Return Type</span></span>  |<span data-ttu-id="c9d82-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9d82-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c9d82-110">Obter contas</span><span class="sxs-lookup"><span data-stu-id="c9d82-110">Get accounts</span></span>](../api/dynamics-account-get.md)|<span data-ttu-id="c9d82-111">contas</span><span class="sxs-lookup"><span data-stu-id="c9d82-111">accounts</span></span>|<span data-ttu-id="c9d82-112">Obtém o objeto accounts.</span><span class="sxs-lookup"><span data-stu-id="c9d82-112">Get accounts object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c9d82-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c9d82-113">Properties</span></span>
| <span data-ttu-id="c9d82-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9d82-114">Property</span></span>     | <span data-ttu-id="c9d82-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9d82-115">Type</span></span>   |<span data-ttu-id="c9d82-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9d82-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9d82-117">id</span><span class="sxs-lookup"><span data-stu-id="c9d82-117">id</span></span>|<span data-ttu-id="c9d82-118">GUID</span><span class="sxs-lookup"><span data-stu-id="c9d82-118">GUID</span></span>|<span data-ttu-id="c9d82-119">A identificação exclusiva da conta.</span><span class="sxs-lookup"><span data-stu-id="c9d82-119">The unique ID of the account.</span></span>|
|<span data-ttu-id="c9d82-120">number</span><span class="sxs-lookup"><span data-stu-id="c9d82-120">number</span></span>|<span data-ttu-id="c9d82-121">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="c9d82-121">string, maximum size 20</span></span>|<span data-ttu-id="c9d82-122">Especifica o número da conta G/L.</span><span class="sxs-lookup"><span data-stu-id="c9d82-122">Specifies the number of the G/L account.</span></span>|
|<span data-ttu-id="c9d82-123">displayName</span><span class="sxs-lookup"><span data-stu-id="c9d82-123">displayName</span></span>|<span data-ttu-id="c9d82-124">Cadeia de caracteres, tamanho máximo 50</span><span class="sxs-lookup"><span data-stu-id="c9d82-124">string, maximum size 50</span></span>|<span data-ttu-id="c9d82-125">Especifica o nome da conta de G/L.</span><span class="sxs-lookup"><span data-stu-id="c9d82-125">Specifies the name of the G/L account.</span></span>|
|<span data-ttu-id="c9d82-126">category</span><span class="sxs-lookup"><span data-stu-id="c9d82-126">category</span></span>|<span data-ttu-id="c9d82-127">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="c9d82-127">string, maximum size 20</span></span>|<span data-ttu-id="c9d82-128">Especifica a categoria da conta de G/L.</span><span class="sxs-lookup"><span data-stu-id="c9d82-128">Specifies the category of the G/L account.</span></span>|
|<span data-ttu-id="c9d82-129">Subcategoria</span><span class="sxs-lookup"><span data-stu-id="c9d82-129">subCategory</span></span>|<span data-ttu-id="c9d82-130">Cadeia de caracteres, tamanho máximo 80</span><span class="sxs-lookup"><span data-stu-id="c9d82-130">string, maximum size 80</span></span>|<span data-ttu-id="c9d82-131">Especifica a subcategoria da categoria de conta da conta G/L.</span><span class="sxs-lookup"><span data-stu-id="c9d82-131">Specifies the subcategory of the account category of the G/L account.</span></span>|
|<span data-ttu-id="c9d82-132">bloqueou</span><span class="sxs-lookup"><span data-stu-id="c9d82-132">blocked</span></span>|<span data-ttu-id="c9d82-133">booliano</span><span class="sxs-lookup"><span data-stu-id="c9d82-133">boolean</span></span>|<span data-ttu-id="c9d82-134">Especifica que não é possível postar entradas na conta G/L.</span><span class="sxs-lookup"><span data-stu-id="c9d82-134">Specifies that entries cannot be posted to the G/L account.</span></span> <span data-ttu-id="c9d82-135">**True** indica que a conta está bloqueada e o lançamento não é permitido.</span><span class="sxs-lookup"><span data-stu-id="c9d82-135">**True** indicates account is blocked and posting is not allowed.</span></span>|
|<span data-ttu-id="c9d82-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9d82-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c9d82-137">datetime</span><span class="sxs-lookup"><span data-stu-id="c9d82-137">datetime</span></span>|<span data-ttu-id="c9d82-138">O último DateTime que a conta foi modificada.</span><span class="sxs-lookup"><span data-stu-id="c9d82-138">The last datetime the account was modified.</span></span>|


## <a name="relationships"></a><span data-ttu-id="c9d82-139">Relações</span><span class="sxs-lookup"><span data-stu-id="c9d82-139">Relationships</span></span>
<span data-ttu-id="c9d82-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c9d82-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c9d82-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c9d82-141">JSON representation</span></span>

<span data-ttu-id="c9d82-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c9d82-142">Here is a JSON representation of the resource.</span></span>


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


