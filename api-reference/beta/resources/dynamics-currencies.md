---
title: tipo de recurso moedas
description: Um objeto Currency no Dynamics 365 Business central
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 42dc5fec859aff758b2f46812a63b10f49f0498a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071364"
---
# <a name="currencies-resource-type"></a><span data-ttu-id="8153a-103">tipo de recurso moedas</span><span class="sxs-lookup"><span data-stu-id="8153a-103">currencies resource type</span></span>

<span data-ttu-id="8153a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8153a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8153a-105">Representa uma moeda usada no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="8153a-105">Represents a currency used in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="8153a-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="8153a-106">Methods</span></span>
| <span data-ttu-id="8153a-107">Método</span><span class="sxs-lookup"><span data-stu-id="8153a-107">Method</span></span>                                                  |<span data-ttu-id="8153a-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8153a-108">Return Type</span></span>|<span data-ttu-id="8153a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8153a-109">Description</span></span>       |
|:--------------------------------------------------------|:----------|:-----------------|
|[<span data-ttu-id="8153a-110">Obter moedas</span><span class="sxs-lookup"><span data-stu-id="8153a-110">Get currencies</span></span>](../api/dynamics-currencies-get.md)      |<span data-ttu-id="8153a-111">monetária</span><span class="sxs-lookup"><span data-stu-id="8153a-111">currencies</span></span> |<span data-ttu-id="8153a-112">Obter uma moeda.</span><span class="sxs-lookup"><span data-stu-id="8153a-112">Get a Currency.</span></span>   |
|[<span data-ttu-id="8153a-113">Lançar moedas</span><span class="sxs-lookup"><span data-stu-id="8153a-113">Post currencies</span></span>](../api/dynamics-create-currencies.md)  |<span data-ttu-id="8153a-114">monetária</span><span class="sxs-lookup"><span data-stu-id="8153a-114">currencies</span></span> |<span data-ttu-id="8153a-115">Criar uma moeda.</span><span class="sxs-lookup"><span data-stu-id="8153a-115">Create a Currency.</span></span>|
|[<span data-ttu-id="8153a-116">Corrigir moedas</span><span class="sxs-lookup"><span data-stu-id="8153a-116">Patch currencies</span></span>](../api/dynamics-currencies-update.md) |<span data-ttu-id="8153a-117">monetária</span><span class="sxs-lookup"><span data-stu-id="8153a-117">currencies</span></span> |<span data-ttu-id="8153a-118">Atualize uma moeda.</span><span class="sxs-lookup"><span data-stu-id="8153a-118">Update a Currency.</span></span>|
|[<span data-ttu-id="8153a-119">Excluir moedas</span><span class="sxs-lookup"><span data-stu-id="8153a-119">Delete currencies</span></span>](../api/dynamics-currencies-delete.md)|<span data-ttu-id="8153a-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="8153a-120">none</span></span>       |<span data-ttu-id="8153a-121">Excluir uma moeda.</span><span class="sxs-lookup"><span data-stu-id="8153a-121">Delete a Currency.</span></span>|

## <a name="properties"></a><span data-ttu-id="8153a-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8153a-122">Properties</span></span>
| <span data-ttu-id="8153a-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8153a-123">Property</span></span>              | <span data-ttu-id="8153a-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="8153a-124">Type</span></span>   |<span data-ttu-id="8153a-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="8153a-125">Description</span></span>                                                   |
|:----------------------|:-------|:-------------------------------------------------------------|
|<span data-ttu-id="8153a-126">id</span><span class="sxs-lookup"><span data-stu-id="8153a-126">id</span></span>                     |<span data-ttu-id="8153a-127">GUID</span><span class="sxs-lookup"><span data-stu-id="8153a-127">GUID</span></span>    |<span data-ttu-id="8153a-128">A identificação exclusiva da moeda.</span><span class="sxs-lookup"><span data-stu-id="8153a-128">The unique ID of the currency.</span></span> <span data-ttu-id="8153a-129">Não editável.</span><span class="sxs-lookup"><span data-stu-id="8153a-129">Non-editable.</span></span>                  |
|<span data-ttu-id="8153a-130">código</span><span class="sxs-lookup"><span data-stu-id="8153a-130">code</span></span>                   |<span data-ttu-id="8153a-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8153a-131">string</span></span>  |<span data-ttu-id="8153a-132">Especifica o código da moeda.</span><span class="sxs-lookup"><span data-stu-id="8153a-132">Specifies the currency code.</span></span>                                  |
|<span data-ttu-id="8153a-133">displayName</span><span class="sxs-lookup"><span data-stu-id="8153a-133">displayName</span></span>            |<span data-ttu-id="8153a-134">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8153a-134">string</span></span>  |<span data-ttu-id="8153a-135">Especifica o nome de exibição da moeda.</span><span class="sxs-lookup"><span data-stu-id="8153a-135">Specifies the currency display name.</span></span>                          |
|<span data-ttu-id="8153a-136">formato</span><span class="sxs-lookup"><span data-stu-id="8153a-136">symbol</span></span>                 |<span data-ttu-id="8153a-137">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8153a-137">string</span></span>  |<span data-ttu-id="8153a-138">Especifica o símbolo para esta moeda que aparece nos cheques.</span><span class="sxs-lookup"><span data-stu-id="8153a-138">Specifies the symbol for this currency that appears on checks.</span></span>|
|<span data-ttu-id="8153a-139">amountDecimalPlaces</span><span class="sxs-lookup"><span data-stu-id="8153a-139">amountDecimalPlaces</span></span>    |<span data-ttu-id="8153a-140">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8153a-140">string</span></span>  |<span data-ttu-id="8153a-141">Especifica o número de casas decimais que o sistema exibirá em valores dessa moeda.</span><span class="sxs-lookup"><span data-stu-id="8153a-141">Specifies the number of decimal places the system will display on amounts for this currency.</span></span>|
|<span data-ttu-id="8153a-142">amountRoundingPrecision</span><span class="sxs-lookup"><span data-stu-id="8153a-142">amountRoundingPrecision</span></span>|<span data-ttu-id="8153a-143">dígitos</span><span class="sxs-lookup"><span data-stu-id="8153a-143">decimal</span></span> |<span data-ttu-id="8153a-144">Especifica o tamanho do intervalo a ser usado ao arredondar valores para esta moeda.</span><span class="sxs-lookup"><span data-stu-id="8153a-144">Specifies the size of the interval to be used when rounding amounts for this currency.</span></span>|
|<span data-ttu-id="8153a-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8153a-145">lastModifiedDateTime</span></span>   |<span data-ttu-id="8153a-146">datetime</span><span class="sxs-lookup"><span data-stu-id="8153a-146">datetime</span></span>|<span data-ttu-id="8153a-147">O último DateTime que a moeda foi modificada.</span><span class="sxs-lookup"><span data-stu-id="8153a-147">The last datetime the currency was modified.</span></span> <span data-ttu-id="8153a-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8153a-148">Read-Only.</span></span>       |  


## <a name="relationships"></a><span data-ttu-id="8153a-149">Relações</span><span class="sxs-lookup"><span data-stu-id="8153a-149">Relationships</span></span>
<span data-ttu-id="8153a-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8153a-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8153a-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8153a-151">JSON representation</span></span>

<span data-ttu-id="8153a-152">Veja a seguir uma representação JSON das moedas.</span><span class="sxs-lookup"><span data-stu-id="8153a-152">Here is a JSON representation of the currencies.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "symbol": "string",
  "amountDecimalPlaces": "string",
  "amountRoundingPrecision": "decimal",
  "lastModifiedDateTime": "datetime"
}

```



