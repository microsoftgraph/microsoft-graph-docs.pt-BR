---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
description: Aqui está uma representação JSON de um recurso ColumnDefinition.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: aae4b71055c7a6574cc4abbaa506fad8961991d9
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/17/2020
ms.locfileid: "48581223"
---
# <a name="columndefinition-resource"></a><span data-ttu-id="8a1d2-103">Recurso ColumnDefinition</span><span class="sxs-lookup"><span data-stu-id="8a1d2-103">ColumnDefinition resource</span></span>

<span data-ttu-id="8a1d2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a1d2-104">Namespace: microsoft.graph</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a1d2-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8a1d2-105">JSON representation</span></span>

<span data-ttu-id="8a1d2-106">Aqui está uma representação JSON de um recurso ColumnDefinition.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-106">Here is a JSON representation of a ColumnDefinition resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.columnDefinition"
}-->

```json
{
  "columnGroup": "string",
  "description": "description",
  "displayName": "friendly name",
  "enforceUniqueValues": "true",
  "hidden": false,
  "id": "string",
  "indexed": true,
  "name": "staticNameForApi",
  "readOnly": false,
  "required": false,
  "boolean": { "@odata.type": "microsoft.graph.booleanColumn" },
  "calculated": { "@odata.type": "microsoft.graph.calculatedColumn" },
  "choice": { "@odata.type": "microsoft.graph.choiceColumn" },
  "currency": { "@odata.type": "microsoft.graph.currencyColumn" },
  "dateTime": { "@odata.type": "microsoft.graph.dateTimeColumn" },
  "defaultValue": { "@odata.type": "microsoft.graph.defaultColumnValue" },
  "geolocation": { "@odata.type": "microsoft.graph.geolocationColumn" },
  "lookup": { "@odata.type": "microsoft.graph.lookupColumn" },
  "number": { "@odata.type": "microsoft.graph.numberColumn" },
  "personOrGroup": { "@odata.type": "microsoft.graph.personOrGroupColumn" },
  "text": { "@odata.type": "microsoft.graph.textColumn" }
}
```

## <a name="properties"></a><span data-ttu-id="8a1d2-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8a1d2-107">Properties</span></span>

<span data-ttu-id="8a1d2-108">O recurso **columnDefinition** tem as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-108">The **columnDefinition** resource has the following properties.</span></span>

| <span data-ttu-id="8a1d2-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="8a1d2-109">Property name</span></span>           | <span data-ttu-id="8a1d2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a1d2-110">Type</span></span>    | <span data-ttu-id="8a1d2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a1d2-111">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="8a1d2-112">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="8a1d2-112">**columnGroup**</span></span>         | <span data-ttu-id="8a1d2-113">string</span><span class="sxs-lookup"><span data-stu-id="8a1d2-113">string</span></span>  | <span data-ttu-id="8a1d2-114">Para colunas de site, o nome do grupo ao qual esta coluna pertence.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-114">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="8a1d2-115">Ajuda a organizar as colunas relacionadas.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-115">Helps organize related columns.</span></span>
| <span data-ttu-id="8a1d2-116">**description**</span><span class="sxs-lookup"><span data-stu-id="8a1d2-116">**description**</span></span>         | <span data-ttu-id="8a1d2-117">string</span><span class="sxs-lookup"><span data-stu-id="8a1d2-117">string</span></span>  | <span data-ttu-id="8a1d2-118">A descrição voltado para o usuário da coluna.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-118">The user-facing description of the column.</span></span>
| <span data-ttu-id="8a1d2-119">**displayName**</span><span class="sxs-lookup"><span data-stu-id="8a1d2-119">**displayName**</span></span>         | <span data-ttu-id="8a1d2-120">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a1d2-120">string</span></span>  | <span data-ttu-id="8a1d2-121">O nome voltado para o usuário da coluna.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-121">The user-facing name of the column.</span></span>
| <span data-ttu-id="8a1d2-122">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="8a1d2-122">**enforceUniqueValues**</span></span> | <span data-ttu-id="8a1d2-123">booliano</span><span class="sxs-lookup"><span data-stu-id="8a1d2-123">boolean</span></span> | <span data-ttu-id="8a1d2-124">Se for verdadeiro, esse mesmo valor não constará em dois itens de lista nessa coluna.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-124">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="8a1d2-125">**hidden**</span><span class="sxs-lookup"><span data-stu-id="8a1d2-125">**hidden**</span></span>              | <span data-ttu-id="8a1d2-126">booliano</span><span class="sxs-lookup"><span data-stu-id="8a1d2-126">boolean</span></span> | <span data-ttu-id="8a1d2-127">Especifica se a coluna é exibida na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-127">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="8a1d2-128">**id**</span><span class="sxs-lookup"><span data-stu-id="8a1d2-128">**id**</span></span>                  | <span data-ttu-id="8a1d2-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a1d2-129">string</span></span>  | <span data-ttu-id="8a1d2-130">O identificador exclusivo da coluna.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-130">The unique identifier for the column.</span></span>
| <span data-ttu-id="8a1d2-131">**indexed**</span><span class="sxs-lookup"><span data-stu-id="8a1d2-131">**indexed**</span></span>             | <span data-ttu-id="8a1d2-132">booliano</span><span class="sxs-lookup"><span data-stu-id="8a1d2-132">boolean</span></span> | <span data-ttu-id="8a1d2-133">Especifica se os valores da coluna podem ser usados para classificação e pesquisa.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-133">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="8a1d2-134">**name**</span><span class="sxs-lookup"><span data-stu-id="8a1d2-134">**name**</span></span>                | <span data-ttu-id="8a1d2-135">string</span><span class="sxs-lookup"><span data-stu-id="8a1d2-135">string</span></span>  | <span data-ttu-id="8a1d2-136">O nome voltado para a API da coluna, conforme ele aparece nos [campos][] em uma [listItem][].</span><span class="sxs-lookup"><span data-stu-id="8a1d2-136">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="8a1d2-137">Para o nome voltado ao usuário, consulte **displayName**.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-137">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="8a1d2-138">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="8a1d2-138">**readOnly**</span></span>            | <span data-ttu-id="8a1d2-139">bool</span><span class="sxs-lookup"><span data-stu-id="8a1d2-139">bool</span></span>    | <span data-ttu-id="8a1d2-140">Especifica se os valores da coluna podem ser modificados.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-140">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="8a1d2-141">**required**</span><span class="sxs-lookup"><span data-stu-id="8a1d2-141">**required**</span></span>            | <span data-ttu-id="8a1d2-142">booliano</span><span class="sxs-lookup"><span data-stu-id="8a1d2-142">boolean</span></span> | <span data-ttu-id="8a1d2-143">Especifica se o valor da coluna não é opcional.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-143">Specifies whether the column value is not optional.</span></span>

<span data-ttu-id="8a1d2-144">As colunas podem conter dados de vários tipos.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-144">Columns can hold data of various types.</span></span>
<span data-ttu-id="8a1d2-145">As propriedades a seguir indicam qual tipo de dados uma coluna armazena, bem como configurações adicionais para esses dados.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-145">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="8a1d2-146">Essas propriedades são mutuamente exclusivas: uma coluna só pode ter uma delas especificada.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-146">These properties are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="8a1d2-147">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="8a1d2-147">Property name</span></span>     | <span data-ttu-id="8a1d2-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a1d2-148">Type</span></span>                    | <span data-ttu-id="8a1d2-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a1d2-149">Description</span></span>
|:------------------|:------------------------|:-------------------------------
| <span data-ttu-id="8a1d2-150">**boolean**</span><span class="sxs-lookup"><span data-stu-id="8a1d2-150">**boolean**</span></span>       | <span data-ttu-id="8a1d2-151">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="8a1d2-151">[booleanColumn][]</span></span>       | <span data-ttu-id="8a1d2-152">Esta coluna armazena valores boolianos.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-152">This column stores boolean values.</span></span>
| <span data-ttu-id="8a1d2-153">**calculated**</span><span class="sxs-lookup"><span data-stu-id="8a1d2-153">**calculated**</span></span>    | <span data-ttu-id="8a1d2-154">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="8a1d2-154">[calculatedColumn][]</span></span>    | <span data-ttu-id="8a1d2-155">Os dados dessa coluna são calculados com base em outras colunas.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-155">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="8a1d2-156">**choice**</span><span class="sxs-lookup"><span data-stu-id="8a1d2-156">**choice**</span></span>        | <span data-ttu-id="8a1d2-157">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="8a1d2-157">[choiceColumn][]</span></span>        | <span data-ttu-id="8a1d2-158">Esta coluna armazena dados de uma lista de opções.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-158">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="8a1d2-159">**currency**</span><span class="sxs-lookup"><span data-stu-id="8a1d2-159">**currency**</span></span>      | <span data-ttu-id="8a1d2-160">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="8a1d2-160">[currencyColumn][]</span></span>      | <span data-ttu-id="8a1d2-161">Esta coluna armazena valores monetários.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-161">This column stores currency values.</span></span>
| <span data-ttu-id="8a1d2-162">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="8a1d2-162">**dateTime**</span></span>      | <span data-ttu-id="8a1d2-163">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="8a1d2-163">[dateTimeColumn][]</span></span>      | <span data-ttu-id="8a1d2-164">Esta coluna armazena valores de datetime.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-164">This column stores DateTime values.</span></span>
| <span data-ttu-id="8a1d2-165">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="8a1d2-165">**defaultValue**</span></span>  | <span data-ttu-id="8a1d2-166">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="8a1d2-166">[defaultColumnValue][]</span></span>  | <span data-ttu-id="8a1d2-167">O valor padrão dessa coluna.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-167">The default value for this column.</span></span>
| <span data-ttu-id="8a1d2-168">**localização geográfica**</span><span class="sxs-lookup"><span data-stu-id="8a1d2-168">**geolocation**</span></span>   | <span data-ttu-id="8a1d2-169">[geolocationColumn][]</span><span class="sxs-lookup"><span data-stu-id="8a1d2-169">[geolocationColumn][]</span></span>   | <span data-ttu-id="8a1d2-170">Esta coluna armazena uma localização geográfica.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-170">This column stores a geolocation.</span></span>
| <span data-ttu-id="8a1d2-171">**lookup**</span><span class="sxs-lookup"><span data-stu-id="8a1d2-171">**lookup**</span></span>        | <span data-ttu-id="8a1d2-172">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="8a1d2-172">[lookupColumn][]</span></span>        | <span data-ttu-id="8a1d2-173">Os dados dessa coluna são procurados por outra fonte no site.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-173">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="8a1d2-174">**number**</span><span class="sxs-lookup"><span data-stu-id="8a1d2-174">**number**</span></span>        | <span data-ttu-id="8a1d2-175">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="8a1d2-175">[numberColumn][]</span></span>        | <span data-ttu-id="8a1d2-176">Esta coluna armazena valores numéricos.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-176">This column stores number values.</span></span>
| <span data-ttu-id="8a1d2-177">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="8a1d2-177">**personOrGroup**</span></span> | <span data-ttu-id="8a1d2-178">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="8a1d2-178">[personOrGroupColumn][]</span></span> | <span data-ttu-id="8a1d2-179">Esta coluna armazena valores de Pessoa ou Grupo.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-179">This column stores Person or Group values.</span></span>
| <span data-ttu-id="8a1d2-180">**text**</span><span class="sxs-lookup"><span data-stu-id="8a1d2-180">**text**</span></span>          | <span data-ttu-id="8a1d2-181">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="8a1d2-181">[textColumn][]</span></span>          | <span data-ttu-id="8a1d2-182">Esta coluna armazena valores de texto.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-182">This column stores text values.</span></span>

<span data-ttu-id="8a1d2-183">Observação: essas propriedades correspondem à enumeração [SPFieldType][] do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-183">Note: These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="8a1d2-184">Embora os tipos de campo mais comuns sejam representados acima, essa API ainda não tem alguns.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-184">While the most common field types are represented above, this API is still missing some.</span></span>
<span data-ttu-id="8a1d2-185">nestes casos, nenhuma das facetas do tipo de coluna serão preenchidas, e a coluna só terá as propriedades básicas.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-185">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="8a1d2-186">Comentários</span><span class="sxs-lookup"><span data-stu-id="8a1d2-186">Remarks</span></span>

<span data-ttu-id="8a1d2-187">Os valores ColumnDefinitions e valores de campo para colunas `hidden` não são mostrados por padrão.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-187">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="8a1d2-188">Para vê-los ao listar **columnDefinitions**, inclua `hidden` na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-188">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="8a1d2-189">Para vê-los ao exibir valores **field** em [listItems][listItem], inclua as colunas desejadas por nome na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="8a1d2-189">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

[booleanColumn]: booleancolumn.md
[calculatedColumn]: calculatedcolumn.md
[choiceColumn]: choicecolumn.md
[currencyColumn]: currencycolumn.md
[dateTimeColumn]: datetimecolumn.md
[defaultColumnValue]: defaultcolumnvalue.md
[geolocationColumn]: geolocationcolumn.md
[lookupColumn]: lookupcolumn.md
[numberColumn]: numbercolumn.md
[personOrGroupColumn]: personorgroupcolumn.md
[textColumn]: textcolumn.md
[fieldValueSet]: fieldvalueset.md
[campos]: fieldvalueset.md
[fields]: fieldvalueset.md
[listItem]: listitem.md

<span data-ttu-id="8a1d2-203">
  [SPFieldType]: /previous-versions/office/sharepoint-server/ms428806(v=office.15)</span><span class="sxs-lookup"><span data-stu-id="8a1d2-203">[SPFieldType]: /previous-versions/office/sharepoint-server/ms428806(v=office.15)</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition"
} -->