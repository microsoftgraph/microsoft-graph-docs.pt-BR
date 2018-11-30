---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ColumnDefinition
ms.openlocfilehash: 9b99abe78b009786d489ec7f0c0fdce1e2945b1d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033275"
---
# <a name="columndefinition-resource-type"></a><span data-ttu-id="17e9f-102">tipo de recurso columnDefinition</span><span class="sxs-lookup"><span data-stu-id="17e9f-102">columnDefinition resource type</span></span>

> <span data-ttu-id="17e9f-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="17e9f-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17e9f-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="17e9f-104">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="17e9f-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="17e9f-105">JSON representation</span></span>

<span data-ttu-id="17e9f-106">Aqui está uma representação JSON de um recurso columnDefinition.</span><span class="sxs-lookup"><span data-stu-id="17e9f-106">Here is a JSON representation of a columnDefinition resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="17e9f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="17e9f-107">Properties</span></span>

<span data-ttu-id="17e9f-108">As colunas podem conter dados de vários tipos.</span><span class="sxs-lookup"><span data-stu-id="17e9f-108">Columns can hold data of various types.</span></span>
<span data-ttu-id="17e9f-109">As propriedades a seguir indicam qual tipo de dados uma coluna armazena, bem como configurações adicionais para esses dados.</span><span class="sxs-lookup"><span data-stu-id="17e9f-109">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="17e9f-110">As propriedades relacionadas a tipo (booleana, calculada, escolha, moeda, data/hora, pesquisa, número, personOrGroup, texto) são mutuamente exclusivas--uma coluna só pode ter um deles especificado.</span><span class="sxs-lookup"><span data-stu-id="17e9f-110">The type-related properties (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="17e9f-111">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="17e9f-111">Property name</span></span>           | <span data-ttu-id="17e9f-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="17e9f-112">Type</span></span>    | <span data-ttu-id="17e9f-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="17e9f-113">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="17e9f-114">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="17e9f-114">**columnGroup**</span></span>         | <span data-ttu-id="17e9f-115">string</span><span class="sxs-lookup"><span data-stu-id="17e9f-115">string</span></span>  | <span data-ttu-id="17e9f-116">Para colunas de site, o nome do grupo ao qual esta coluna pertence.</span><span class="sxs-lookup"><span data-stu-id="17e9f-116">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="17e9f-117">Ajuda a organizar as colunas relacionadas.</span><span class="sxs-lookup"><span data-stu-id="17e9f-117">Helps organize related columns.</span></span>
| <span data-ttu-id="17e9f-118">**description**</span><span class="sxs-lookup"><span data-stu-id="17e9f-118">**description**</span></span>         | <span data-ttu-id="17e9f-119">string</span><span class="sxs-lookup"><span data-stu-id="17e9f-119">string</span></span>  | <span data-ttu-id="17e9f-120">A descrição voltado para o usuário da coluna.</span><span class="sxs-lookup"><span data-stu-id="17e9f-120">The user-facing description of the column.</span></span>
| <span data-ttu-id="17e9f-121">**displayName**</span><span class="sxs-lookup"><span data-stu-id="17e9f-121">**displayName**</span></span>         | <span data-ttu-id="17e9f-122">string</span><span class="sxs-lookup"><span data-stu-id="17e9f-122">string</span></span>  | <span data-ttu-id="17e9f-123">O nome voltado para o usuário da coluna.</span><span class="sxs-lookup"><span data-stu-id="17e9f-123">The user-facing name of the column.</span></span>
| <span data-ttu-id="17e9f-124">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="17e9f-124">**enforceUniqueValues**</span></span> | <span data-ttu-id="17e9f-125">booliano</span><span class="sxs-lookup"><span data-stu-id="17e9f-125">boolean</span></span> | <span data-ttu-id="17e9f-126">Se for verdadeiro, esse mesmo valor não constará em dois itens de lista nessa coluna.</span><span class="sxs-lookup"><span data-stu-id="17e9f-126">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="17e9f-127">**hidden**</span><span class="sxs-lookup"><span data-stu-id="17e9f-127">**hidden**</span></span>              | <span data-ttu-id="17e9f-128">booliano</span><span class="sxs-lookup"><span data-stu-id="17e9f-128">boolean</span></span> | <span data-ttu-id="17e9f-129">Especifica se a coluna é exibida na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="17e9f-129">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="17e9f-130">**id**</span><span class="sxs-lookup"><span data-stu-id="17e9f-130">**id**</span></span>                  | <span data-ttu-id="17e9f-131">string</span><span class="sxs-lookup"><span data-stu-id="17e9f-131">string</span></span>  | <span data-ttu-id="17e9f-132">O identificador exclusivo da coluna.</span><span class="sxs-lookup"><span data-stu-id="17e9f-132">The unique identifier for the column.</span></span>
| <span data-ttu-id="17e9f-133">**indexed**</span><span class="sxs-lookup"><span data-stu-id="17e9f-133">**indexed**</span></span>             | <span data-ttu-id="17e9f-134">booliano</span><span class="sxs-lookup"><span data-stu-id="17e9f-134">boolean</span></span> | <span data-ttu-id="17e9f-135">Especifica se os valores da coluna podem ser usados para classificação e pesquisa.</span><span class="sxs-lookup"><span data-stu-id="17e9f-135">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="17e9f-136">**name**</span><span class="sxs-lookup"><span data-stu-id="17e9f-136">**name**</span></span>                | <span data-ttu-id="17e9f-137">string</span><span class="sxs-lookup"><span data-stu-id="17e9f-137">string</span></span>  | <span data-ttu-id="17e9f-138">O nome voltado para a API da coluna, conforme ele aparece nos [campos][] em uma [listItem][].</span><span class="sxs-lookup"><span data-stu-id="17e9f-138">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="17e9f-139">Para o nome voltado ao usuário, consulte **displayName**.</span><span class="sxs-lookup"><span data-stu-id="17e9f-139">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="17e9f-140">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="17e9f-140">**readOnly**</span></span>            | <span data-ttu-id="17e9f-141">bool</span><span class="sxs-lookup"><span data-stu-id="17e9f-141">bool</span></span>    | <span data-ttu-id="17e9f-142">Especifica se os valores da coluna podem ser modificados.</span><span class="sxs-lookup"><span data-stu-id="17e9f-142">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="17e9f-143">**required**</span><span class="sxs-lookup"><span data-stu-id="17e9f-143">**required**</span></span>            | <span data-ttu-id="17e9f-144">booliano</span><span class="sxs-lookup"><span data-stu-id="17e9f-144">boolean</span></span> | <span data-ttu-id="17e9f-145">Especifica se o valor da coluna não é opcional.</span><span class="sxs-lookup"><span data-stu-id="17e9f-145">Specifies whether the column value is not optional.</span></span>
| <span data-ttu-id="17e9f-146">**boolean**</span><span class="sxs-lookup"><span data-stu-id="17e9f-146">**boolean**</span></span>       | <span data-ttu-id="17e9f-147">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="17e9f-147">[booleanColumn][]</span></span>       | <span data-ttu-id="17e9f-148">Esta coluna armazena valores boolianos.</span><span class="sxs-lookup"><span data-stu-id="17e9f-148">This column stores boolean values.</span></span>
| <span data-ttu-id="17e9f-149">**calculated**</span><span class="sxs-lookup"><span data-stu-id="17e9f-149">**calculated**</span></span>    | <span data-ttu-id="17e9f-150">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="17e9f-150">[calculatedColumn][]</span></span>    | <span data-ttu-id="17e9f-151">Os dados dessa coluna são calculados com base em outras colunas.</span><span class="sxs-lookup"><span data-stu-id="17e9f-151">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="17e9f-152">**choice**</span><span class="sxs-lookup"><span data-stu-id="17e9f-152">**choice**</span></span>        | <span data-ttu-id="17e9f-153">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="17e9f-153">[choiceColumn][]</span></span>        | <span data-ttu-id="17e9f-154">Esta coluna armazena dados de uma lista de opções.</span><span class="sxs-lookup"><span data-stu-id="17e9f-154">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="17e9f-155">**currency**</span><span class="sxs-lookup"><span data-stu-id="17e9f-155">**currency**</span></span>      | <span data-ttu-id="17e9f-156">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="17e9f-156">[currencyColumn][]</span></span>      | <span data-ttu-id="17e9f-157">Esta coluna armazena valores monetários.</span><span class="sxs-lookup"><span data-stu-id="17e9f-157">This column stores currency values.</span></span>
| <span data-ttu-id="17e9f-158">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="17e9f-158">**dateTime**</span></span>      | <span data-ttu-id="17e9f-159">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="17e9f-159">[dateTimeColumn][]</span></span>      | <span data-ttu-id="17e9f-160">Esta coluna armazena valores de datetime.</span><span class="sxs-lookup"><span data-stu-id="17e9f-160">This column stores DateTime values.</span></span>
| <span data-ttu-id="17e9f-161">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="17e9f-161">**defaultValue**</span></span>  | <span data-ttu-id="17e9f-162">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="17e9f-162">[defaultColumnValue][]</span></span>  | <span data-ttu-id="17e9f-163">O valor padrão dessa coluna.</span><span class="sxs-lookup"><span data-stu-id="17e9f-163">The default value for this column.</span></span>
| <span data-ttu-id="17e9f-164">**localização geográfica**</span><span class="sxs-lookup"><span data-stu-id="17e9f-164">**geolocation**</span></span>   | <span data-ttu-id="17e9f-165">[geolocationColumn][]</span><span class="sxs-lookup"><span data-stu-id="17e9f-165">[geolocationColumn][]</span></span>   | <span data-ttu-id="17e9f-166">Essa coluna armazena uma localização geográfica.</span><span class="sxs-lookup"><span data-stu-id="17e9f-166">This column stores a geolocation.</span></span>
| <span data-ttu-id="17e9f-167">**lookup**</span><span class="sxs-lookup"><span data-stu-id="17e9f-167">**lookup**</span></span>        | <span data-ttu-id="17e9f-168">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="17e9f-168">[lookupColumn][]</span></span>        | <span data-ttu-id="17e9f-169">Os dados dessa coluna são procurados por outra fonte no site.</span><span class="sxs-lookup"><span data-stu-id="17e9f-169">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="17e9f-170">**number**</span><span class="sxs-lookup"><span data-stu-id="17e9f-170">**number**</span></span>        | <span data-ttu-id="17e9f-171">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="17e9f-171">[numberColumn][]</span></span>        | <span data-ttu-id="17e9f-172">Esta coluna armazena valores numéricos.</span><span class="sxs-lookup"><span data-stu-id="17e9f-172">This column stores number values.</span></span>
| <span data-ttu-id="17e9f-173">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="17e9f-173">**personOrGroup**</span></span> | <span data-ttu-id="17e9f-174">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="17e9f-174">[personOrGroupColumn][]</span></span> | <span data-ttu-id="17e9f-175">Esta coluna armazena valores de Pessoa ou Grupo.</span><span class="sxs-lookup"><span data-stu-id="17e9f-175">This column stores Person or Group values.</span></span>
| <span data-ttu-id="17e9f-176">**text**</span><span class="sxs-lookup"><span data-stu-id="17e9f-176">**text**</span></span>          | <span data-ttu-id="17e9f-177">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="17e9f-177">[textColumn][]</span></span>          | <span data-ttu-id="17e9f-178">Esta coluna armazena valores de texto.</span><span class="sxs-lookup"><span data-stu-id="17e9f-178">This column stores text values.</span></span>

><span data-ttu-id="17e9f-179">**Observação:** Essas propriedades correspondem às enumeração de [SPFieldType][] do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="17e9f-179">**Note:** These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="17e9f-180">Enquanto os tipos mais comuns de campo são representados na tabela anterior, essa versão beta API ainda faltam alguns.</span><span class="sxs-lookup"><span data-stu-id="17e9f-180">While the most common field types are represented in the previous table, this beta API is still missing some.</span></span>
<span data-ttu-id="17e9f-181">nestes casos, nenhuma das facetas do tipo de coluna serão preenchidas, e a coluna só terá as propriedades básicas.</span><span class="sxs-lookup"><span data-stu-id="17e9f-181">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="17e9f-182">Comentários</span><span class="sxs-lookup"><span data-stu-id="17e9f-182">Remarks</span></span>

<span data-ttu-id="17e9f-183">Os valores ColumnDefinitions e valores de campo para colunas `hidden` não são mostrados por padrão.</span><span class="sxs-lookup"><span data-stu-id="17e9f-183">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="17e9f-184">Para vê-los ao listar **columnDefinitions**, inclua `hidden` na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="17e9f-184">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="17e9f-185">Para vê-los ao exibir valores **field** em [listItems][listItem], inclua as colunas desejadas por nome na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="17e9f-185">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

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
[fields]: fieldvalueset.md
[listItem]: listitem.md

<span data-ttu-id="17e9f-199">
  [SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx</span><span class="sxs-lookup"><span data-stu-id="17e9f-199">[SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition"
} -->
