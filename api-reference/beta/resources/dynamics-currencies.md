---
title: tipo de recurso moedas
description: Um objeto Currency no Dynamics 365 Business central
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: ba8ad750831394e2a84fab7ca87d76754838db60
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012615"
---
# <a name="currencies-resource-type"></a><span data-ttu-id="10a5c-103">tipo de recurso moedas</span><span class="sxs-lookup"><span data-stu-id="10a5c-103">currencies resource type</span></span>
<span data-ttu-id="10a5c-104">Representa uma moeda usada no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="10a5c-104">Represents a currency used in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="10a5c-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="10a5c-105">Methods</span></span>
| <span data-ttu-id="10a5c-106">Método</span><span class="sxs-lookup"><span data-stu-id="10a5c-106">Method</span></span>                                                  |<span data-ttu-id="10a5c-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="10a5c-107">Return Type</span></span>|<span data-ttu-id="10a5c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="10a5c-108">Description</span></span>       |
|:--------------------------------------------------------|:----------|:-----------------|
|[<span data-ttu-id="10a5c-109">Obter moedas</span><span class="sxs-lookup"><span data-stu-id="10a5c-109">Get currencies</span></span>](../api/dynamics-currencies-get.md)      |<span data-ttu-id="10a5c-110">monetária</span><span class="sxs-lookup"><span data-stu-id="10a5c-110">currencies</span></span> |<span data-ttu-id="10a5c-111">Obter uma moeda.</span><span class="sxs-lookup"><span data-stu-id="10a5c-111">Get a Currency.</span></span>   |
|[<span data-ttu-id="10a5c-112">Lançar moedas</span><span class="sxs-lookup"><span data-stu-id="10a5c-112">Post currencies</span></span>](../api/dynamics-create-currencies.md)  |<span data-ttu-id="10a5c-113">monetária</span><span class="sxs-lookup"><span data-stu-id="10a5c-113">currencies</span></span> |<span data-ttu-id="10a5c-114">Criar uma moeda.</span><span class="sxs-lookup"><span data-stu-id="10a5c-114">Create a Currency.</span></span>|
|[<span data-ttu-id="10a5c-115">Corrigir moedas</span><span class="sxs-lookup"><span data-stu-id="10a5c-115">Patch currencies</span></span>](../api/dynamics-currencies-update.md) |<span data-ttu-id="10a5c-116">monetária</span><span class="sxs-lookup"><span data-stu-id="10a5c-116">currencies</span></span> |<span data-ttu-id="10a5c-117">Atualize uma moeda.</span><span class="sxs-lookup"><span data-stu-id="10a5c-117">Update a Currency.</span></span>|
|[<span data-ttu-id="10a5c-118">Excluir moedas</span><span class="sxs-lookup"><span data-stu-id="10a5c-118">Delete currencies</span></span>](../api/dynamics-currencies-delete.md)|<span data-ttu-id="10a5c-119">none</span><span class="sxs-lookup"><span data-stu-id="10a5c-119">none</span></span>       |<span data-ttu-id="10a5c-120">Excluir uma moeda.</span><span class="sxs-lookup"><span data-stu-id="10a5c-120">Delete a Currency.</span></span>|

## <a name="properties"></a><span data-ttu-id="10a5c-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="10a5c-121">Properties</span></span>
| <span data-ttu-id="10a5c-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10a5c-122">Property</span></span>              | <span data-ttu-id="10a5c-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="10a5c-123">Type</span></span>   |<span data-ttu-id="10a5c-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="10a5c-124">Description</span></span>                                                   |
|:----------------------|:-------|:-------------------------------------------------------------|
|<span data-ttu-id="10a5c-125">id</span><span class="sxs-lookup"><span data-stu-id="10a5c-125">id</span></span>                     |<span data-ttu-id="10a5c-126">GUID</span><span class="sxs-lookup"><span data-stu-id="10a5c-126">GUID</span></span>    |<span data-ttu-id="10a5c-127">A identificação exclusiva da moeda.</span><span class="sxs-lookup"><span data-stu-id="10a5c-127">The unique ID of the currency.</span></span> <span data-ttu-id="10a5c-128">Não editável.</span><span class="sxs-lookup"><span data-stu-id="10a5c-128">Non-editable.</span></span>                  |
|<span data-ttu-id="10a5c-129">código</span><span class="sxs-lookup"><span data-stu-id="10a5c-129">code</span></span>                   |<span data-ttu-id="10a5c-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10a5c-130">string</span></span>  |<span data-ttu-id="10a5c-131">Especifica o código da moeda.</span><span class="sxs-lookup"><span data-stu-id="10a5c-131">Specifies the currency code.</span></span>                                  |
|<span data-ttu-id="10a5c-132">displayName</span><span class="sxs-lookup"><span data-stu-id="10a5c-132">displayName</span></span>            |<span data-ttu-id="10a5c-133">string</span><span class="sxs-lookup"><span data-stu-id="10a5c-133">string</span></span>  |<span data-ttu-id="10a5c-134">Especifica o nome de exibição da moeda.</span><span class="sxs-lookup"><span data-stu-id="10a5c-134">Specifies the currency display name.</span></span>                          |
|<span data-ttu-id="10a5c-135">formato</span><span class="sxs-lookup"><span data-stu-id="10a5c-135">symbol</span></span>                 |<span data-ttu-id="10a5c-136">string</span><span class="sxs-lookup"><span data-stu-id="10a5c-136">string</span></span>  |<span data-ttu-id="10a5c-137">Especifica o símbolo para esta moeda que aparece nos cheques.</span><span class="sxs-lookup"><span data-stu-id="10a5c-137">Specifies the symbol for this currency that appears on checks.</span></span>|
|<span data-ttu-id="10a5c-138">amountDecimalPlaces</span><span class="sxs-lookup"><span data-stu-id="10a5c-138">amountDecimalPlaces</span></span>    |<span data-ttu-id="10a5c-139">string</span><span class="sxs-lookup"><span data-stu-id="10a5c-139">string</span></span>  |<span data-ttu-id="10a5c-140">Especifica o número de casas decimais que o sistema exibirá em valores dessa moeda.</span><span class="sxs-lookup"><span data-stu-id="10a5c-140">Specifies the number of decimal places the system will display on amounts for this currency.</span></span>|
|<span data-ttu-id="10a5c-141">amountRoundingPrecision</span><span class="sxs-lookup"><span data-stu-id="10a5c-141">amountRoundingPrecision</span></span>|<span data-ttu-id="10a5c-142">dígitos</span><span class="sxs-lookup"><span data-stu-id="10a5c-142">decimal</span></span> |<span data-ttu-id="10a5c-143">Especifica o tamanho do intervalo a ser usado ao arredondar valores para esta moeda.</span><span class="sxs-lookup"><span data-stu-id="10a5c-143">Specifies the size of the interval to be used when rounding amounts for this currency.</span></span>|
|<span data-ttu-id="10a5c-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="10a5c-144">lastModifiedDateTime</span></span>   |<span data-ttu-id="10a5c-145">DateTime</span><span class="sxs-lookup"><span data-stu-id="10a5c-145">datetime</span></span>|<span data-ttu-id="10a5c-146">O último DateTime que a moeda foi modificada.</span><span class="sxs-lookup"><span data-stu-id="10a5c-146">The last datetime the currency was modified.</span></span> <span data-ttu-id="10a5c-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="10a5c-147">Read-Only.</span></span>       |  


## <a name="relationships"></a><span data-ttu-id="10a5c-148">Relações</span><span class="sxs-lookup"><span data-stu-id="10a5c-148">Relationships</span></span>
<span data-ttu-id="10a5c-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="10a5c-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="10a5c-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="10a5c-150">JSON representation</span></span>

<span data-ttu-id="10a5c-151">Veja a seguir uma representação JSON das moedas.</span><span class="sxs-lookup"><span data-stu-id="10a5c-151">Here is a JSON representation of the currencies.</span></span>


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

