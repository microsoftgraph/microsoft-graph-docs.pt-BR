---
title: Usando dicas de ordenação no Planner
description: '`)'
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: fa518e3820437ec02ee2b28e1b9a93fab3d4b100
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977686"
---
# <a name="using-order-hints-in-planner"></a><span data-ttu-id="4454c-103">Usando dicas de ordenação no Planner</span><span class="sxs-lookup"><span data-stu-id="4454c-103">Using order hints in Planner</span></span>

> <span data-ttu-id="4454c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4454c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4454c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4454c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4454c-p102">Objetos no planejador identificam sua ordem de classificação pelas dicas de ordenação. Os valores de dica de ordenação são cadeias de caracteres. Os clientes podem classificar as cadeias de caracteres com base no valor ordinal dos caracteres nelas para identificar a ordem dos itens. Os caracteres são comparados desde o início da cadeia de caracteres, até que uma diferença seja encontrada nos valores ordinais de caracteres ou uma cadeia de caracteres termina, caso em que a cadeia de caracteres mais curta seria classificada antes da mais longa. Os valores podem conter qualquer caractere ordinal entre 32 (espaço) e 126 (`~`)</span><span class="sxs-lookup"><span data-stu-id="4454c-p102">Objects in Planner identify their sort order by order hints. The order hint values are strings. The clients can sort the strings based on ordinal value of characters in them to identify the order of items. The characters are compared from the beginning of the string, until a difference is encountered in the ordinal values of characters, or one string ends, in which case the shorter string would be sorted before the longer. The values can contain any character between ordinals 32 (space) and 126 (`~`)</span></span>

<span data-ttu-id="4454c-p103">Por exemplo, um item com dica de ordenação `a` (valor ordinal 97) seria colocado antes de outro item com dica de ordenação `z` (valor ordinal 122). Um item com dica de ordenação `abc` (valores ordinais 97, 98, 99), seriam colocados antes de outro item com dica de ordenação `abd` (valores ordinais 97, 98, 100). Um item com dica de ordenação `a` seria colocado antes de outro item com dica de ordenação `ab` já que todos os caracteres existentes são os mesmos e `a` é mais curto.</span><span class="sxs-lookup"><span data-stu-id="4454c-p103">As an example, an item with order hint `a` (ordinal value 97) would be placed before another item with order hint `z` (ordinal value 122). An item with order hint `abc` (ordinal values 97, 98, 99), would be placed before another item with order hint `abd` (ordinal values 97, 98, 100). An item with order hint `a` would be placed before another item with order hint `ab` since all existing characters are the same, and `a` is shorter.</span></span>

<span data-ttu-id="4454c-p104">Os valores de todas as dicas de ordenação são calculados pelo serviço. O cliente pode reordenar os itens especificando a dica de ordenação do item que foi movido entre dois itens definindo a dica de ordenação do seguinte valor: `<previous order hint> <next order hint>!`, onde `<previous order hint>` deve ser substituído pela dica de ordenação do item que vem antes do novo local desejado e `<next order hint>` deve ser substituído pela dica de ordenação do item que vem depois do novo local desejado. Há um caractere de espaço entre esses valores de dica de ordenação e o valor inteiro tem o sufixo `!`. Se o item não estiver presente, deve ser usada uma cadeia de caracteres vazia. Esse valor também pode ser composto por cálculos anteriores e pode ser usado no cliente para classificar os itens exatamente como as dicas de ordenação retornadas pelo serviço. Depois que o cliente envia esses valores em uma atualização, o serviço calculará um valor curto que classifica no local desejado.</span><span class="sxs-lookup"><span data-stu-id="4454c-p104">The values for all order hints are calculated by the service. The client can reorder items by specifying the order hint for the item that got moved between two items with by setting the order hint to the following value: `<previous order hint> <next order hint>!`, where `<previous order hint>` is to be replaced by the order hint of the item that comes before the new desired location, and `<next order hint>` is to be replaced by the order hint of the item that comes after the new desired location. There is a space character between these order hint values, and the entire value is suffixed with `!`. If either item isn't present, empty string should be used instead. This value can also be composed of previous calculations, and can be used in the client to sort items exactly like service returned order hints. Once the client sends these values in an update, the service will calculate a short value that sorts in the desired location.</span></span>

> <span data-ttu-id="4454c-120">**Observação:** Nos exemplos a seguir, os valores de dica de ordem real são circundados em caracteres de aspas simples (`'`) para manter a clareza, porém esses não fazem parte dos dados e não devem ser enviados para o serviço.</span><span class="sxs-lookup"><span data-stu-id="4454c-120">**Note:** In the following examples, the actual order hint values are surrounded in single quote characters (`'`) for clarity, however these are not part of the data, and must not be sent to the service.</span></span>
 
<span data-ttu-id="4454c-121">Por exemplo, considere a seguinte lista de dicas de ordem de classificação:</span><span class="sxs-lookup"><span data-stu-id="4454c-121">As an example, consider the following list of sorted order hints:</span></span>

1. <span data-ttu-id="4454c-122">Item 1 (Dica de ordenação: `'5637'`)</span><span class="sxs-lookup"><span data-stu-id="4454c-122">Item 1 (Order Hint: `'5637'`)</span></span>
2. <span data-ttu-id="4454c-123">Item 2 (Dica de ordenação: `'adhg'`)</span><span class="sxs-lookup"><span data-stu-id="4454c-123">Item 2 (Order Hint: `'adhg'`)</span></span>

<span data-ttu-id="4454c-124">Colocar um Item 3 antes de um Item 1 e colocar o item 4 entre o Item 1 e o Item 2 e o item 5 depois do Item 2, criaria as seguintes dicas de ordenação no cliente.</span><span class="sxs-lookup"><span data-stu-id="4454c-124">Placing an Item 3 before Item 1, then placing item 4 between Item 1 and Item 2, and then placing item 5 after Item 2, would create the following order hints on the client.</span></span> 

1. <span data-ttu-id="4454c-125">Item 3 (Dica de ordenação: `' 5637!'`)</span><span class="sxs-lookup"><span data-stu-id="4454c-125">Item 3 (Order Hint: `' 5637!'`)</span></span>
2. <span data-ttu-id="4454c-126">Item 1 (Dica de ordenação: `'5637'`)</span><span class="sxs-lookup"><span data-stu-id="4454c-126">Item 1 (Order Hint: `'5637'`)</span></span>
3. <span data-ttu-id="4454c-127">Item 4 (Dica de ordenação: `'5637 adhg!'`)</span><span class="sxs-lookup"><span data-stu-id="4454c-127">Item 4 (Order Hint: `'5637 adhg!'`)</span></span>
4. <span data-ttu-id="4454c-128">Item 2 (Dica de ordenação: `'adhg'`)</span><span class="sxs-lookup"><span data-stu-id="4454c-128">Item 2 (Order Hint: `'adhg'`)</span></span>
5. <span data-ttu-id="4454c-129">Item 5 (Dica de ordenação: `'adhg !'`)</span><span class="sxs-lookup"><span data-stu-id="4454c-129">Item 5 (Order Hint: `'adhg !'`)</span></span>

<span data-ttu-id="4454c-130">Em seguida, mover o item 1 para o fim da lista geraria:</span><span class="sxs-lookup"><span data-stu-id="4454c-130">Then, moving item 1 to the end of the list would generate:</span></span>

1. <span data-ttu-id="4454c-131">Item 3 (Dica de ordenação: `' 5637!'`)</span><span class="sxs-lookup"><span data-stu-id="4454c-131">Item 3 (Order Hint: `' 5637!'`)</span></span>
2. <span data-ttu-id="4454c-132">Item 4 (Dica de ordenação: `'5637 adhg!'`)</span><span class="sxs-lookup"><span data-stu-id="4454c-132">Item 4 (Order Hint: `'5637 adhg!'`)</span></span>
3. <span data-ttu-id="4454c-133">Item 2 (Dica de ordenação: `'adhg'`)</span><span class="sxs-lookup"><span data-stu-id="4454c-133">Item 2 (Order Hint: `'adhg'`)</span></span>
4. <span data-ttu-id="4454c-134">Item 5 (Dica de ordenação: `'adhg !'`)</span><span class="sxs-lookup"><span data-stu-id="4454c-134">Item 5 (Order Hint: `'adhg !'`)</span></span>
5. <span data-ttu-id="4454c-135">Item 1 (Dica de ordenação: `'adhg ! !'`)</span><span class="sxs-lookup"><span data-stu-id="4454c-135">Item 1 (Order Hint: `'adhg ! !'`)</span></span>

<span data-ttu-id="4454c-136">Por fim, mover o Item 5 entre o Item 3 e o Item 4 geraria:</span><span class="sxs-lookup"><span data-stu-id="4454c-136">Finally moving Item 5 between Item 3 and Item 4 would generate:</span></span>

1. <span data-ttu-id="4454c-137">Item 3 (Dica de ordenação: `' 5637!'`)</span><span class="sxs-lookup"><span data-stu-id="4454c-137">Item 3 (Order Hint: `' 5637!'`)</span></span>
2. <span data-ttu-id="4454c-138">Item 5 (Dica de ordenação: `' 5637! 5637 adhg!!'`)</span><span class="sxs-lookup"><span data-stu-id="4454c-138">Item 5 (Order Hint: `' 5637! 5637 adhg!!'`)</span></span>
3. <span data-ttu-id="4454c-139">Item 4 (Dica de ordenação: `'5637 adhg!'`)</span><span class="sxs-lookup"><span data-stu-id="4454c-139">Item 4 (Order Hint: `'5637 adhg!'`)</span></span>
4. <span data-ttu-id="4454c-140">Item 2 (Dica de ordenação: `'adhg'`)</span><span class="sxs-lookup"><span data-stu-id="4454c-140">Item 2 (Order Hint: `'adhg'`)</span></span>
5. <span data-ttu-id="4454c-141">Item 1 (Dica de ordenação: `'adhg ! !'`)</span><span class="sxs-lookup"><span data-stu-id="4454c-141">Item 1 (Order Hint: `'adhg ! !'`)</span></span>

<span data-ttu-id="4454c-142">Quando essas alterações para valores de dica de ordem são enviadas para o serviço em solicitações de patch, o serviço irá calcular valores adequados que mantêm a ordem destinada pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4454c-142">When these changes to order hint values are sent to the service in patch requests, the service will calculate proper values that keep the order intended by the client.</span></span> <span data-ttu-id="4454c-143">O cliente pode obter a se imediata de valores do `Prefer: return=representation` especificado no cabeçalho de preferência o `PATCH` solicitações.</span><span class="sxs-lookup"><span data-stu-id="4454c-143">The client can obtain the values immediate if the `Prefer: return=representation` preference header is specified in the `PATCH` requests.</span></span> <span data-ttu-id="4454c-144">Os valores do caso acima podem ter a seguinte aparência (os valores reais podem diferir).</span><span class="sxs-lookup"><span data-stu-id="4454c-144">The values for the case above may look like the following (the actual values may differ).</span></span> 

1. <span data-ttu-id="4454c-145">Item 3 (Dica de ordenação: `'432b'`)</span><span class="sxs-lookup"><span data-stu-id="4454c-145">Item 3 (Order Hint: `'432b'`)</span></span>
2. <span data-ttu-id="4454c-146">Item 5 (Dica de ordenação: `'6F"#'`)</span><span class="sxs-lookup"><span data-stu-id="4454c-146">Item 5 (Order Hint: `'6F"#'`)</span></span>
3. <span data-ttu-id="4454c-147">Item 4 (Dica de ordenação: `'7A$6'`)</span><span class="sxs-lookup"><span data-stu-id="4454c-147">Item 4 (Order Hint: `'7A$6'`)</span></span>
4. <span data-ttu-id="4454c-148">Item 2 (Dica de ordenação: `'adhg'`)</span><span class="sxs-lookup"><span data-stu-id="4454c-148">Item 2 (Order Hint: `'adhg'`)</span></span>
5. <span data-ttu-id="4454c-149">Item 1 (Dica de ordenação: `'de5%'`)</span><span class="sxs-lookup"><span data-stu-id="4454c-149">Item 1 (Order Hint: `'de5%'`)</span></span>

<span data-ttu-id="4454c-p106">Dicas de ordenação podem ser especificadas para criar o primeiro item na lista como ` !`, pois nem um item anterior ou próximo existe nesse caso, porém isso é desnecessário, como o serviço gerará automaticamente valores para todos os valores de dica de ordenação nos itens se eles não forem especificados durante a criação do item. O exemplo a seguir ilustra as dicas de ordenação que devem ser usadas ao inserir itens em uma lista anteriormente vazia. Adicione o primeiro item:</span><span class="sxs-lookup"><span data-stu-id="4454c-p106">Order Hints can be specified for creating the first item in the list as ` !`, since neither a previous or a next item exists in that case, however this is unnecessary, as the service will auto-generate values for all order hint values on items if they are not specified during creation of the item. Following example illustrates the order hints should be used when placing items in a previously empty list. Add the first item:</span></span>

1. <span data-ttu-id="4454c-153">Item 1 (Dica de ordenação: `' !'`)</span><span class="sxs-lookup"><span data-stu-id="4454c-153">Item 1 (Order Hint: `' !'`)</span></span>

<span data-ttu-id="4454c-154">Adicione o segundo item ao topo:</span><span class="sxs-lookup"><span data-stu-id="4454c-154">Add the second item to top:</span></span>

1. <span data-ttu-id="4454c-155">Item 2 (Dica de ordenação: `'  !!'`)</span><span class="sxs-lookup"><span data-stu-id="4454c-155">Item 2 (Order Hint: `'  !!'`)</span></span>
2. <span data-ttu-id="4454c-156">Item 1 (Dica de ordenação: `' !'`)</span><span class="sxs-lookup"><span data-stu-id="4454c-156">Item 1 (Order Hint: `' !'`)</span></span>

<span data-ttu-id="4454c-157">Adicione o terceiro item à parte inferior:</span><span class="sxs-lookup"><span data-stu-id="4454c-157">Add the third item to bottom:</span></span>

1. <span data-ttu-id="4454c-158">Item 2 (Dica de ordenação: `'  !!'`)</span><span class="sxs-lookup"><span data-stu-id="4454c-158">Item 2 (Order Hint: `'  !!'`)</span></span>
2. <span data-ttu-id="4454c-159">Item 1 (Dica de ordenação: `' !'`)</span><span class="sxs-lookup"><span data-stu-id="4454c-159">Item 1 (Order Hint: `' !'`)</span></span>
3. <span data-ttu-id="4454c-160">Item 3 (Dica de ordenação: `' ! !'`)</span><span class="sxs-lookup"><span data-stu-id="4454c-160">Item 3 (Order Hint: `' ! !'`)</span></span>







