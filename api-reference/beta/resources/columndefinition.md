---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
ms.openlocfilehash: ddd6b3c6d3048bf7a6d3ab2dbc8ff7259651ee2f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460616"
---
# <a name="columndefinition-resource-type"></a><span data-ttu-id="b8427-102">tipo de recurso columnDefinition</span><span class="sxs-lookup"><span data-stu-id="b8427-102">columnDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="b8427-103">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b8427-103">JSON representation</span></span>

<span data-ttu-id="b8427-104">Veja a seguir uma representação JSON de um recurso columnDefinition.</span><span class="sxs-lookup"><span data-stu-id="b8427-104">Here is a JSON representation of a columnDefinition resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="b8427-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b8427-105">Properties</span></span>

<span data-ttu-id="b8427-106">As colunas podem conter dados de vários tipos.</span><span class="sxs-lookup"><span data-stu-id="b8427-106">Columns can hold data of various types.</span></span>
<span data-ttu-id="b8427-107">As propriedades a seguir indicam qual tipo de dados uma coluna armazena, bem como configurações adicionais para esses dados.</span><span class="sxs-lookup"><span data-stu-id="b8427-107">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="b8427-108">As propriedades relacionadas ao tipo (Boolean, calculado, Choice, Currency, dateTime, Lookup, Number, personOrGroup, Text) são mutuamente excludentes--uma coluna só pode ter uma delas especificada.</span><span class="sxs-lookup"><span data-stu-id="b8427-108">The type-related properties (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="b8427-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="b8427-109">Property name</span></span>           | <span data-ttu-id="b8427-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8427-110">Type</span></span>    | <span data-ttu-id="b8427-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8427-111">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="b8427-112">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="b8427-112">**columnGroup**</span></span>         | <span data-ttu-id="b8427-113">string</span><span class="sxs-lookup"><span data-stu-id="b8427-113">string</span></span>  | <span data-ttu-id="b8427-114">Para colunas de site, o nome do grupo ao qual esta coluna pertence.</span><span class="sxs-lookup"><span data-stu-id="b8427-114">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="b8427-115">Ajuda a organizar as colunas relacionadas.</span><span class="sxs-lookup"><span data-stu-id="b8427-115">Helps organize related columns.</span></span>
| <span data-ttu-id="b8427-116">**description**</span><span class="sxs-lookup"><span data-stu-id="b8427-116">**description**</span></span>         | <span data-ttu-id="b8427-117">string</span><span class="sxs-lookup"><span data-stu-id="b8427-117">string</span></span>  | <span data-ttu-id="b8427-118">A descrição voltado para o usuário da coluna.</span><span class="sxs-lookup"><span data-stu-id="b8427-118">The user-facing description of the column.</span></span>
| <span data-ttu-id="b8427-119">**displayName**</span><span class="sxs-lookup"><span data-stu-id="b8427-119">**displayName**</span></span>         | <span data-ttu-id="b8427-120">string</span><span class="sxs-lookup"><span data-stu-id="b8427-120">string</span></span>  | <span data-ttu-id="b8427-121">O nome voltado para o usuário da coluna.</span><span class="sxs-lookup"><span data-stu-id="b8427-121">The user-facing name of the column.</span></span>
| <span data-ttu-id="b8427-122">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="b8427-122">**enforceUniqueValues**</span></span> | <span data-ttu-id="b8427-123">booliano</span><span class="sxs-lookup"><span data-stu-id="b8427-123">boolean</span></span> | <span data-ttu-id="b8427-124">Se for verdadeiro, esse mesmo valor não constará em dois itens de lista nessa coluna.</span><span class="sxs-lookup"><span data-stu-id="b8427-124">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="b8427-125">**hidden**</span><span class="sxs-lookup"><span data-stu-id="b8427-125">**hidden**</span></span>              | <span data-ttu-id="b8427-126">booliano</span><span class="sxs-lookup"><span data-stu-id="b8427-126">boolean</span></span> | <span data-ttu-id="b8427-127">Especifica se a coluna é exibida na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="b8427-127">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="b8427-128">**id**</span><span class="sxs-lookup"><span data-stu-id="b8427-128">**id**</span></span>                  | <span data-ttu-id="b8427-129">string</span><span class="sxs-lookup"><span data-stu-id="b8427-129">string</span></span>  | <span data-ttu-id="b8427-130">O identificador exclusivo da coluna.</span><span class="sxs-lookup"><span data-stu-id="b8427-130">The unique identifier for the column.</span></span>
| <span data-ttu-id="b8427-131">**indexed**</span><span class="sxs-lookup"><span data-stu-id="b8427-131">**indexed**</span></span>             | <span data-ttu-id="b8427-132">booliano</span><span class="sxs-lookup"><span data-stu-id="b8427-132">boolean</span></span> | <span data-ttu-id="b8427-133">Especifica se os valores da coluna podem ser usados para classificação e pesquisa.</span><span class="sxs-lookup"><span data-stu-id="b8427-133">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="b8427-134">**name**</span><span class="sxs-lookup"><span data-stu-id="b8427-134">**name**</span></span>                | <span data-ttu-id="b8427-135">string</span><span class="sxs-lookup"><span data-stu-id="b8427-135">string</span></span>  | <span data-ttu-id="b8427-136">O nome voltado para a API da coluna, conforme ele aparece nos [campos][] em uma [listItem][].</span><span class="sxs-lookup"><span data-stu-id="b8427-136">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="b8427-137">Para o nome voltado ao usuário, consulte **displayName**.</span><span class="sxs-lookup"><span data-stu-id="b8427-137">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="b8427-138">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="b8427-138">**readOnly**</span></span>            | <span data-ttu-id="b8427-139">bool</span><span class="sxs-lookup"><span data-stu-id="b8427-139">bool</span></span>    | <span data-ttu-id="b8427-140">Especifica se os valores da coluna podem ser modificados.</span><span class="sxs-lookup"><span data-stu-id="b8427-140">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="b8427-141">**required**</span><span class="sxs-lookup"><span data-stu-id="b8427-141">**required**</span></span>            | <span data-ttu-id="b8427-142">booliano</span><span class="sxs-lookup"><span data-stu-id="b8427-142">boolean</span></span> | <span data-ttu-id="b8427-143">Especifica se o valor da coluna não é opcional.</span><span class="sxs-lookup"><span data-stu-id="b8427-143">Specifies whether the column value is not optional.</span></span>
| <span data-ttu-id="b8427-144">**boolean**</span><span class="sxs-lookup"><span data-stu-id="b8427-144">**boolean**</span></span>       | <span data-ttu-id="b8427-145">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="b8427-145">[booleanColumn][]</span></span>       | <span data-ttu-id="b8427-146">Esta coluna armazena valores boolianos.</span><span class="sxs-lookup"><span data-stu-id="b8427-146">This column stores boolean values.</span></span>
| <span data-ttu-id="b8427-147">**calculated**</span><span class="sxs-lookup"><span data-stu-id="b8427-147">**calculated**</span></span>    | <span data-ttu-id="b8427-148">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="b8427-148">[calculatedColumn][]</span></span>    | <span data-ttu-id="b8427-149">Os dados dessa coluna são calculados com base em outras colunas.</span><span class="sxs-lookup"><span data-stu-id="b8427-149">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="b8427-150">**choice**</span><span class="sxs-lookup"><span data-stu-id="b8427-150">**choice**</span></span>        | <span data-ttu-id="b8427-151">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="b8427-151">[choiceColumn][]</span></span>        | <span data-ttu-id="b8427-152">Esta coluna armazena dados de uma lista de opções.</span><span class="sxs-lookup"><span data-stu-id="b8427-152">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="b8427-153">**currency**</span><span class="sxs-lookup"><span data-stu-id="b8427-153">**currency**</span></span>      | <span data-ttu-id="b8427-154">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="b8427-154">[currencyColumn][]</span></span>      | <span data-ttu-id="b8427-155">Esta coluna armazena valores monetários.</span><span class="sxs-lookup"><span data-stu-id="b8427-155">This column stores currency values.</span></span>
| <span data-ttu-id="b8427-156">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="b8427-156">**dateTime**</span></span>      | <span data-ttu-id="b8427-157">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="b8427-157">[dateTimeColumn][]</span></span>      | <span data-ttu-id="b8427-158">Esta coluna armazena valores de datetime.</span><span class="sxs-lookup"><span data-stu-id="b8427-158">This column stores DateTime values.</span></span>
| <span data-ttu-id="b8427-159">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="b8427-159">**defaultValue**</span></span>  | <span data-ttu-id="b8427-160">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="b8427-160">[defaultColumnValue][]</span></span>  | <span data-ttu-id="b8427-161">O valor padrão dessa coluna.</span><span class="sxs-lookup"><span data-stu-id="b8427-161">The default value for this column.</span></span>
| <span data-ttu-id="b8427-162">**localização geográfica**</span><span class="sxs-lookup"><span data-stu-id="b8427-162">**geolocation**</span></span>   | <span data-ttu-id="b8427-163">[geolocationColumn][]</span><span class="sxs-lookup"><span data-stu-id="b8427-163">[geolocationColumn][]</span></span>   | <span data-ttu-id="b8427-164">Esta coluna armazena uma localização geográfica.</span><span class="sxs-lookup"><span data-stu-id="b8427-164">This column stores a geolocation.</span></span>
| <span data-ttu-id="b8427-165">**lookup**</span><span class="sxs-lookup"><span data-stu-id="b8427-165">**lookup**</span></span>        | <span data-ttu-id="b8427-166">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="b8427-166">[lookupColumn][]</span></span>        | <span data-ttu-id="b8427-167">Os dados dessa coluna são procurados por outra fonte no site.</span><span class="sxs-lookup"><span data-stu-id="b8427-167">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="b8427-168">**number**</span><span class="sxs-lookup"><span data-stu-id="b8427-168">**number**</span></span>        | <span data-ttu-id="b8427-169">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="b8427-169">[numberColumn][]</span></span>        | <span data-ttu-id="b8427-170">Esta coluna armazena valores numéricos.</span><span class="sxs-lookup"><span data-stu-id="b8427-170">This column stores number values.</span></span>
| <span data-ttu-id="b8427-171">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="b8427-171">**personOrGroup**</span></span> | <span data-ttu-id="b8427-172">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="b8427-172">[personOrGroupColumn][]</span></span> | <span data-ttu-id="b8427-173">Esta coluna armazena valores de Pessoa ou Grupo.</span><span class="sxs-lookup"><span data-stu-id="b8427-173">This column stores Person or Group values.</span></span>
| <span data-ttu-id="b8427-174">**text**</span><span class="sxs-lookup"><span data-stu-id="b8427-174">**text**</span></span>          | <span data-ttu-id="b8427-175">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="b8427-175">[textColumn][]</span></span>          | <span data-ttu-id="b8427-176">Esta coluna armazena valores de texto.</span><span class="sxs-lookup"><span data-stu-id="b8427-176">This column stores text values.</span></span>

><span data-ttu-id="b8427-177">**Observação:** Essas propriedades correspondem à enumeração de [][] UserField do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b8427-177">**Note:** These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="b8427-178">Enquanto os tipos de campo mais comuns são representados na tabela anterior, esta API beta ainda não tem alguns.</span><span class="sxs-lookup"><span data-stu-id="b8427-178">While the most common field types are represented in the previous table, this beta API is still missing some.</span></span>
<span data-ttu-id="b8427-179">nestes casos, nenhuma das facetas do tipo de coluna serão preenchidas, e a coluna só terá as propriedades básicas.</span><span class="sxs-lookup"><span data-stu-id="b8427-179">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="b8427-180">Comentários</span><span class="sxs-lookup"><span data-stu-id="b8427-180">Remarks</span></span>

<span data-ttu-id="b8427-181">Os valores ColumnDefinitions e valores de campo para colunas `hidden` não são mostrados por padrão.</span><span class="sxs-lookup"><span data-stu-id="b8427-181">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="b8427-182">Para vê-los ao listar **columnDefinitions**, inclua `hidden` na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="b8427-182">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="b8427-183">Para vê-los ao exibir valores **field** em [listItems][listItem], inclua as colunas desejadas por nome na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="b8427-183">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

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

<span data-ttu-id="b8427-197">
  [SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx</span><span class="sxs-lookup"><span data-stu-id="b8427-197">[SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition",
  "suppressions": [
    "Error: /api-reference/beta/resources/columndefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
