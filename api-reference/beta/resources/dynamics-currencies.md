---
title: tipo de recurso moedas
description: Um objeto Currency no Dynamics 365 Business central
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: e986777d277e84246104561e5e275d7508b41b7b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42504731"
---
# <a name="currencies-resource-type"></a><span data-ttu-id="ecc17-103">tipo de recurso moedas</span><span class="sxs-lookup"><span data-stu-id="ecc17-103">currencies resource type</span></span>

<span data-ttu-id="ecc17-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ecc17-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ecc17-105">Representa uma moeda usada no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="ecc17-105">Represents a currency used in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="ecc17-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="ecc17-106">Methods</span></span>
| <span data-ttu-id="ecc17-107">Método</span><span class="sxs-lookup"><span data-stu-id="ecc17-107">Method</span></span>                                                  |<span data-ttu-id="ecc17-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ecc17-108">Return Type</span></span>|<span data-ttu-id="ecc17-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecc17-109">Description</span></span>       |
|:--------------------------------------------------------|:----------|:-----------------|
|[<span data-ttu-id="ecc17-110">Obter moedas</span><span class="sxs-lookup"><span data-stu-id="ecc17-110">Get currencies</span></span>](../api/dynamics-currencies-get.md)      |<span data-ttu-id="ecc17-111">monetária</span><span class="sxs-lookup"><span data-stu-id="ecc17-111">currencies</span></span> |<span data-ttu-id="ecc17-112">Obter uma moeda.</span><span class="sxs-lookup"><span data-stu-id="ecc17-112">Get a Currency.</span></span>   |
|[<span data-ttu-id="ecc17-113">Lançar moedas</span><span class="sxs-lookup"><span data-stu-id="ecc17-113">Post currencies</span></span>](../api/dynamics-create-currencies.md)  |<span data-ttu-id="ecc17-114">monetária</span><span class="sxs-lookup"><span data-stu-id="ecc17-114">currencies</span></span> |<span data-ttu-id="ecc17-115">Criar uma moeda.</span><span class="sxs-lookup"><span data-stu-id="ecc17-115">Create a Currency.</span></span>|
|[<span data-ttu-id="ecc17-116">Corrigir moedas</span><span class="sxs-lookup"><span data-stu-id="ecc17-116">Patch currencies</span></span>](../api/dynamics-currencies-update.md) |<span data-ttu-id="ecc17-117">monetária</span><span class="sxs-lookup"><span data-stu-id="ecc17-117">currencies</span></span> |<span data-ttu-id="ecc17-118">Atualize uma moeda.</span><span class="sxs-lookup"><span data-stu-id="ecc17-118">Update a Currency.</span></span>|
|[<span data-ttu-id="ecc17-119">Excluir moedas</span><span class="sxs-lookup"><span data-stu-id="ecc17-119">Delete currencies</span></span>](../api/dynamics-currencies-delete.md)|<span data-ttu-id="ecc17-120">nenhuma</span><span class="sxs-lookup"><span data-stu-id="ecc17-120">none</span></span>       |<span data-ttu-id="ecc17-121">Excluir uma moeda.</span><span class="sxs-lookup"><span data-stu-id="ecc17-121">Delete a Currency.</span></span>|

## <a name="properties"></a><span data-ttu-id="ecc17-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ecc17-122">Properties</span></span>
| <span data-ttu-id="ecc17-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ecc17-123">Property</span></span>              | <span data-ttu-id="ecc17-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="ecc17-124">Type</span></span>   |<span data-ttu-id="ecc17-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecc17-125">Description</span></span>                                                   |
|:----------------------|:-------|:-------------------------------------------------------------|
|<span data-ttu-id="ecc17-126">id</span><span class="sxs-lookup"><span data-stu-id="ecc17-126">id</span></span>                     |<span data-ttu-id="ecc17-127">GUID</span><span class="sxs-lookup"><span data-stu-id="ecc17-127">GUID</span></span>    |<span data-ttu-id="ecc17-128">A identificação exclusiva da moeda.</span><span class="sxs-lookup"><span data-stu-id="ecc17-128">The unique ID of the currency.</span></span> <span data-ttu-id="ecc17-129">Não editável.</span><span class="sxs-lookup"><span data-stu-id="ecc17-129">Non-editable.</span></span>                  |
|<span data-ttu-id="ecc17-130">código</span><span class="sxs-lookup"><span data-stu-id="ecc17-130">code</span></span>                   |<span data-ttu-id="ecc17-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ecc17-131">string</span></span>  |<span data-ttu-id="ecc17-132">Especifica o código da moeda.</span><span class="sxs-lookup"><span data-stu-id="ecc17-132">Specifies the currency code.</span></span>                                  |
|<span data-ttu-id="ecc17-133">displayName</span><span class="sxs-lookup"><span data-stu-id="ecc17-133">displayName</span></span>            |<span data-ttu-id="ecc17-134">string</span><span class="sxs-lookup"><span data-stu-id="ecc17-134">string</span></span>  |<span data-ttu-id="ecc17-135">Especifica o nome de exibição da moeda.</span><span class="sxs-lookup"><span data-stu-id="ecc17-135">Specifies the currency display name.</span></span>                          |
|<span data-ttu-id="ecc17-136">formato</span><span class="sxs-lookup"><span data-stu-id="ecc17-136">symbol</span></span>                 |<span data-ttu-id="ecc17-137">string</span><span class="sxs-lookup"><span data-stu-id="ecc17-137">string</span></span>  |<span data-ttu-id="ecc17-138">Especifica o símbolo para esta moeda que aparece nos cheques.</span><span class="sxs-lookup"><span data-stu-id="ecc17-138">Specifies the symbol for this currency that appears on checks.</span></span>|
|<span data-ttu-id="ecc17-139">amountDecimalPlaces</span><span class="sxs-lookup"><span data-stu-id="ecc17-139">amountDecimalPlaces</span></span>    |<span data-ttu-id="ecc17-140">string</span><span class="sxs-lookup"><span data-stu-id="ecc17-140">string</span></span>  |<span data-ttu-id="ecc17-141">Especifica o número de casas decimais que o sistema exibirá em valores dessa moeda.</span><span class="sxs-lookup"><span data-stu-id="ecc17-141">Specifies the number of decimal places the system will display on amounts for this currency.</span></span>|
|<span data-ttu-id="ecc17-142">amountRoundingPrecision</span><span class="sxs-lookup"><span data-stu-id="ecc17-142">amountRoundingPrecision</span></span>|<span data-ttu-id="ecc17-143">dígitos</span><span class="sxs-lookup"><span data-stu-id="ecc17-143">decimal</span></span> |<span data-ttu-id="ecc17-144">Especifica o tamanho do intervalo a ser usado ao arredondar valores para esta moeda.</span><span class="sxs-lookup"><span data-stu-id="ecc17-144">Specifies the size of the interval to be used when rounding amounts for this currency.</span></span>|
|<span data-ttu-id="ecc17-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ecc17-145">lastModifiedDateTime</span></span>   |<span data-ttu-id="ecc17-146">datetime</span><span class="sxs-lookup"><span data-stu-id="ecc17-146">datetime</span></span>|<span data-ttu-id="ecc17-147">O último DateTime que a moeda foi modificada.</span><span class="sxs-lookup"><span data-stu-id="ecc17-147">The last datetime the currency was modified.</span></span> <span data-ttu-id="ecc17-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ecc17-148">Read-Only.</span></span>       |  


## <a name="relationships"></a><span data-ttu-id="ecc17-149">Relações</span><span class="sxs-lookup"><span data-stu-id="ecc17-149">Relationships</span></span>
<span data-ttu-id="ecc17-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ecc17-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ecc17-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ecc17-151">JSON representation</span></span>

<span data-ttu-id="ecc17-152">Veja a seguir uma representação JSON das moedas.</span><span class="sxs-lookup"><span data-stu-id="ecc17-152">Here is a JSON representation of the currencies.</span></span>


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

