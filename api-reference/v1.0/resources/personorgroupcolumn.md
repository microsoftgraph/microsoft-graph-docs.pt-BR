---
author: simonhult
ms.date: 09/11/2017
title: PersonOrGroupColumn
localization_priority: Normal
ms.prod: insights
description: O recurso personOrGroupColumn em uma columnDefinition indica que os valores da coluna representam uma pessoa ou grupo escolhido no diretório.
doc_type: resourcePageType
ms.openlocfilehash: d8ce31e7eb044e588f73afefb2b370e161fa7cdf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035515"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="9d634-103">Tipo de recurso PersonOrGroupColumn</span><span class="sxs-lookup"><span data-stu-id="9d634-103">PersonOrGroupColumn resource type</span></span>

<span data-ttu-id="9d634-104">O recurso **personOrGroupColumn** em uma [columnDefinition](columndefinition.md) indica que os valores da coluna representam uma pessoa ou grupo escolhido no diretório.</span><span class="sxs-lookup"><span data-stu-id="9d634-104">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d634-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9d634-105">JSON representation</span></span>

<span data-ttu-id="9d634-106">Aqui está uma representação JSON de um recurso **personOrGroupColumn**.</span><span class="sxs-lookup"><span data-stu-id="9d634-106">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="9d634-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9d634-107">Properties</span></span>

| <span data-ttu-id="9d634-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="9d634-108">Property name</span></span>              | <span data-ttu-id="9d634-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d634-109">Type</span></span>    | <span data-ttu-id="9d634-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d634-110">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="9d634-111">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="9d634-111">**allowMultipleSelection**</span></span> | <span data-ttu-id="9d634-112">booliano</span><span class="sxs-lookup"><span data-stu-id="9d634-112">boolean</span></span> | <span data-ttu-id="9d634-113">Indica se vários valores podem ser selecionados da origem.</span><span class="sxs-lookup"><span data-stu-id="9d634-113">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="9d634-114">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="9d634-114">**displayAs**</span></span>              | <span data-ttu-id="9d634-115">string</span><span class="sxs-lookup"><span data-stu-id="9d634-115">string</span></span>  | <span data-ttu-id="9d634-116">Como exibir as informações sobre a pessoa ou grupo escolhido.</span><span class="sxs-lookup"><span data-stu-id="9d634-116">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="9d634-117">Veja a seguir.</span><span class="sxs-lookup"><span data-stu-id="9d634-117">See below.</span></span>
| <span data-ttu-id="9d634-118">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="9d634-118">**chooseFromType**</span></span>         | <span data-ttu-id="9d634-119">string</span><span class="sxs-lookup"><span data-stu-id="9d634-119">string</span></span>  | <span data-ttu-id="9d634-120">Se permite somente a seleção de pessoas, ou de pessoas e grupos.</span><span class="sxs-lookup"><span data-stu-id="9d634-120">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="9d634-121">Deve ser `peopleAndGroups` ou `peopleOnly`.</span><span class="sxs-lookup"><span data-stu-id="9d634-121">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-options"></a><span data-ttu-id="9d634-122">Opções de displayas</span><span class="sxs-lookup"><span data-stu-id="9d634-122">DisplayAs options</span></span>

| <span data-ttu-id="9d634-123">Valor de displayAs</span><span class="sxs-lookup"><span data-stu-id="9d634-123">DisplayAs value</span></span>               | <span data-ttu-id="9d634-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d634-124">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="9d634-125">**account**</span><span class="sxs-lookup"><span data-stu-id="9d634-125">**account**</span></span>                   | <span data-ttu-id="9d634-126">A cadeia de caracteres de declaração codificada bruta do SharePoint para a pessoa ou grupo (por exemplo.</span><span class="sxs-lookup"><span data-stu-id="9d634-126">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="9d634-127">i:0#.f</span><span class="sxs-lookup"><span data-stu-id="9d634-127">i:0#.f</span></span>|<span data-ttu-id="9d634-128">membership</span><span class="sxs-lookup"><span data-stu-id="9d634-128">membership</span></span>|<span data-ttu-id="9d634-129">jane@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="9d634-129">jane@contoso.com).</span></span>
| <span data-ttu-id="9d634-130">**department**</span><span class="sxs-lookup"><span data-stu-id="9d634-130">**department**</span></span>                | <span data-ttu-id="9d634-131">O departamento da pessoa ou grupo.</span><span class="sxs-lookup"><span data-stu-id="9d634-131">The person or group's department.</span></span>
| <span data-ttu-id="9d634-132">**firstName**</span><span class="sxs-lookup"><span data-stu-id="9d634-132">**firstName**</span></span>                 | <span data-ttu-id="9d634-133">O primeiro nome da pessoa.</span><span class="sxs-lookup"><span data-stu-id="9d634-133">The person's first name.</span></span>
| <span data-ttu-id="9d634-134">**id**</span><span class="sxs-lookup"><span data-stu-id="9d634-134">**id**</span></span>                        | <span data-ttu-id="9d634-135">A id da pessoa ou grupo no diretório.</span><span class="sxs-lookup"><span data-stu-id="9d634-135">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="9d634-136">**lastName**</span><span class="sxs-lookup"><span data-stu-id="9d634-136">**lastName**</span></span>                  | <span data-ttu-id="9d634-137">O sobrenome da pessoa.</span><span class="sxs-lookup"><span data-stu-id="9d634-137">The person's last name.</span></span>
| <span data-ttu-id="9d634-138">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="9d634-138">**mobilePhone**</span></span>               | <span data-ttu-id="9d634-139">O número de celular da pessoa.</span><span class="sxs-lookup"><span data-stu-id="9d634-139">The person's mobile phone number.</span></span>
| <span data-ttu-id="9d634-140">**name**</span><span class="sxs-lookup"><span data-stu-id="9d634-140">**name**</span></span>                      | <span data-ttu-id="9d634-141">O nome da pessoa.</span><span class="sxs-lookup"><span data-stu-id="9d634-141">The person's name.</span></span>
| <span data-ttu-id="9d634-142">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="9d634-142">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="9d634-143">O nome da pessoa com sua imagem e detalhes adicionais.</span><span class="sxs-lookup"><span data-stu-id="9d634-143">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="9d634-144">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="9d634-144">**nameWithPresence**</span></span>          | <span data-ttu-id="9d634-145">Padrão.</span><span class="sxs-lookup"><span data-stu-id="9d634-145">Default.</span></span> <span data-ttu-id="9d634-146">O nome da pessoa com um ícone indicador de presença (disponível/ocupado/etc.)</span><span class="sxs-lookup"><span data-stu-id="9d634-146">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="9d634-147">**office**</span><span class="sxs-lookup"><span data-stu-id="9d634-147">**office**</span></span>                    | <span data-ttu-id="9d634-148">O número comercial da pessoa.</span><span class="sxs-lookup"><span data-stu-id="9d634-148">The person's office number.</span></span>
| <span data-ttu-id="9d634-149">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="9d634-149">**pictureOnly36x36**</span></span>          | <span data-ttu-id="9d634-150">Imagem da pessoa, delimitada por um quadrado de 36 x 36 pixels.</span><span class="sxs-lookup"><span data-stu-id="9d634-150">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="9d634-151">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="9d634-151">**pictureOnly48x48**</span></span>          | <span data-ttu-id="9d634-152">Imagem da pessoa, delimitada por um quadrado de 48 x 48 pixels.</span><span class="sxs-lookup"><span data-stu-id="9d634-152">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="9d634-153">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="9d634-153">**pictureOnly72x72**</span></span>          | <span data-ttu-id="9d634-154">Imagem da pessoa, delimitada por um quadrado de 72 x 72 pixels.</span><span class="sxs-lookup"><span data-stu-id="9d634-154">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="9d634-155">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="9d634-155">**sipAddress**</span></span>                | <span data-ttu-id="9d634-156">O endereço sip da pessoa.</span><span class="sxs-lookup"><span data-stu-id="9d634-156">The person's sip address.</span></span>
| <span data-ttu-id="9d634-157">**title**</span><span class="sxs-lookup"><span data-stu-id="9d634-157">**title**</span></span>                     | <span data-ttu-id="9d634-158">O cargo da pessoa na organização.</span><span class="sxs-lookup"><span data-stu-id="9d634-158">The person's title in the organization.</span></span>
| <span data-ttu-id="9d634-159">**userName**</span><span class="sxs-lookup"><span data-stu-id="9d634-159">**userName**</span></span>                  | <span data-ttu-id="9d634-160">O nome de usuário da pessoa ou grupo.</span><span class="sxs-lookup"><span data-stu-id="9d634-160">The person or group's user name.</span></span>
| <span data-ttu-id="9d634-161">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="9d634-161">**workEmail**</span></span>                 | <span data-ttu-id="9d634-162">O endereço de email da pessoa ou grupo.</span><span class="sxs-lookup"><span data-stu-id="9d634-162">The person or group's email address.</span></span>
| <span data-ttu-id="9d634-163">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="9d634-163">**workPhone**</span></span>                 | <span data-ttu-id="9d634-164">O número de telefone comercial da pessoa.</span><span class="sxs-lookup"><span data-stu-id="9d634-164">The person's work phone number.</span></span>

<span data-ttu-id="9d634-165">Observação: podem ser retornados tipos adicionais de DisplayAs.</span><span class="sxs-lookup"><span data-stu-id="9d634-165">Note: Additional DisplayAs types may be returned.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/personorgroupcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(peopleAndGroups,peopleOnly) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/personorgroupcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(account,contentType,created,department,...) are in resource, but () are in table"
  ],
  "tocPath": "Resources/PersonOrGroupColumn"
} -->
