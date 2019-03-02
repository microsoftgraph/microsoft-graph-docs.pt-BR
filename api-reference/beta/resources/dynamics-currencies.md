---
title: tipo de recurso moedas
description: Um objeto Currency no Dynamics 365 Business central
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: c0d15b8d20e99537cb2f567a9f8fe12b45dbd389
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366624"
---
# <a name="currencies-resource-type"></a><span data-ttu-id="fc73a-103">tipo de recurso moedas</span><span class="sxs-lookup"><span data-stu-id="fc73a-103">currencies resource type</span></span>
<span data-ttu-id="fc73a-104">Representa uma moeda usada no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="fc73a-104">Represents a currency used in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="fc73a-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="fc73a-105">Methods</span></span>
| <span data-ttu-id="fc73a-106">Método</span><span class="sxs-lookup"><span data-stu-id="fc73a-106">Method</span></span>                                                  |<span data-ttu-id="fc73a-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fc73a-107">Return Type</span></span>|<span data-ttu-id="fc73a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc73a-108">Description</span></span>       |
|:--------------------------------------------------------|:----------|:-----------------|
|[<span data-ttu-id="fc73a-109">Obter moedas</span><span class="sxs-lookup"><span data-stu-id="fc73a-109">Get currencies</span></span>](../api/dynamics-currencies-get.md)      |<span data-ttu-id="fc73a-110">monetária</span><span class="sxs-lookup"><span data-stu-id="fc73a-110">currencies</span></span> |<span data-ttu-id="fc73a-111">Obter uma moeda.</span><span class="sxs-lookup"><span data-stu-id="fc73a-111">Get a Currency.</span></span>   |
|[<span data-ttu-id="fc73a-112">Lançar moedas</span><span class="sxs-lookup"><span data-stu-id="fc73a-112">Post currencies</span></span>](../api/dynamics-create-currencies.md)  |<span data-ttu-id="fc73a-113">monetária</span><span class="sxs-lookup"><span data-stu-id="fc73a-113">currencies</span></span> |<span data-ttu-id="fc73a-114">Criar uma moeda.</span><span class="sxs-lookup"><span data-stu-id="fc73a-114">Create a Currency.</span></span>|
|[<span data-ttu-id="fc73a-115">Corrigir moedas</span><span class="sxs-lookup"><span data-stu-id="fc73a-115">Patch currencies</span></span>](../api/dynamics-currencies-update.md) |<span data-ttu-id="fc73a-116">monetária</span><span class="sxs-lookup"><span data-stu-id="fc73a-116">currencies</span></span> |<span data-ttu-id="fc73a-117">Atualize uma moeda.</span><span class="sxs-lookup"><span data-stu-id="fc73a-117">Update a Currency.</span></span>|
|[<span data-ttu-id="fc73a-118">Excluir moedas</span><span class="sxs-lookup"><span data-stu-id="fc73a-118">Delete currencies</span></span>](../api/dynamics-currencies-delete.md)|<span data-ttu-id="fc73a-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="fc73a-119">none</span></span>       |<span data-ttu-id="fc73a-120">Excluir uma moeda.</span><span class="sxs-lookup"><span data-stu-id="fc73a-120">Delete a Currency.</span></span>|

## <a name="properties"></a><span data-ttu-id="fc73a-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fc73a-121">Properties</span></span>
| <span data-ttu-id="fc73a-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc73a-122">Property</span></span>              | <span data-ttu-id="fc73a-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc73a-123">Type</span></span>   |<span data-ttu-id="fc73a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc73a-124">Description</span></span>                                                   |
|:----------------------|:-------|:-------------------------------------------------------------|
|<span data-ttu-id="fc73a-125">id</span><span class="sxs-lookup"><span data-stu-id="fc73a-125">id</span></span>                     |<span data-ttu-id="fc73a-126">GUID</span><span class="sxs-lookup"><span data-stu-id="fc73a-126">GUID</span></span>    |<span data-ttu-id="fc73a-127">A identificação exclusiva da moeda.</span><span class="sxs-lookup"><span data-stu-id="fc73a-127">The unique ID of the currency.</span></span> <span data-ttu-id="fc73a-128">Não editável.</span><span class="sxs-lookup"><span data-stu-id="fc73a-128">Non-editable.</span></span>                  |
|<span data-ttu-id="fc73a-129">código</span><span class="sxs-lookup"><span data-stu-id="fc73a-129">code</span></span>                   |<span data-ttu-id="fc73a-130">string</span><span class="sxs-lookup"><span data-stu-id="fc73a-130">string</span></span>  |<span data-ttu-id="fc73a-131">Especifica o código da moeda.</span><span class="sxs-lookup"><span data-stu-id="fc73a-131">Specifies the currency code.</span></span>                                  |
|<span data-ttu-id="fc73a-132">displayName</span><span class="sxs-lookup"><span data-stu-id="fc73a-132">displayName</span></span>            |<span data-ttu-id="fc73a-133">string</span><span class="sxs-lookup"><span data-stu-id="fc73a-133">string</span></span>  |<span data-ttu-id="fc73a-134">Especifica o nome de exibição da moeda.</span><span class="sxs-lookup"><span data-stu-id="fc73a-134">Specifies the currency display name.</span></span>                          |
|<span data-ttu-id="fc73a-135">formato</span><span class="sxs-lookup"><span data-stu-id="fc73a-135">symbol</span></span>                 |<span data-ttu-id="fc73a-136">string</span><span class="sxs-lookup"><span data-stu-id="fc73a-136">string</span></span>  |<span data-ttu-id="fc73a-137">Especifica o símbolo para esta moeda que aparece nos cheques.</span><span class="sxs-lookup"><span data-stu-id="fc73a-137">Specifies the symbol for this currency that appears on checks.</span></span>|
|<span data-ttu-id="fc73a-138">amountDecimalPlaces</span><span class="sxs-lookup"><span data-stu-id="fc73a-138">amountDecimalPlaces</span></span>    |<span data-ttu-id="fc73a-139">string</span><span class="sxs-lookup"><span data-stu-id="fc73a-139">string</span></span>  |<span data-ttu-id="fc73a-140">Especifica o número de casas decimais que o sistema exibirá em valores dessa moeda.</span><span class="sxs-lookup"><span data-stu-id="fc73a-140">Specifies the number of decimal places the system will display on amounts for this currency.</span></span>|
|<span data-ttu-id="fc73a-141">amountRoundingPrecision</span><span class="sxs-lookup"><span data-stu-id="fc73a-141">amountRoundingPrecision</span></span>|<span data-ttu-id="fc73a-142">dígitos</span><span class="sxs-lookup"><span data-stu-id="fc73a-142">decimal</span></span> |<span data-ttu-id="fc73a-143">Especifica o tamanho do intervalo a ser usado ao arredondar valores para esta moeda.</span><span class="sxs-lookup"><span data-stu-id="fc73a-143">Specifies the size of the interval to be used when rounding amounts for this currency.</span></span>|
|<span data-ttu-id="fc73a-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fc73a-144">lastModifiedDateTime</span></span>   |<span data-ttu-id="fc73a-145">DateTime</span><span class="sxs-lookup"><span data-stu-id="fc73a-145">datetime</span></span>|<span data-ttu-id="fc73a-146">O último DateTime que a moeda foi modificada.</span><span class="sxs-lookup"><span data-stu-id="fc73a-146">The last datetime the currency was modified.</span></span> <span data-ttu-id="fc73a-147">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="fc73a-147">Read-Only.</span></span>       |  


## <a name="relationships"></a><span data-ttu-id="fc73a-148">Relações</span><span class="sxs-lookup"><span data-stu-id="fc73a-148">Relationships</span></span>
<span data-ttu-id="fc73a-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fc73a-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc73a-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fc73a-150">JSON representation</span></span>

<span data-ttu-id="fc73a-151">Veja a seguir uma representação JSON das moedas.</span><span class="sxs-lookup"><span data-stu-id="fc73a-151">Here is a JSON representation of the currencies.</span></span>


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

