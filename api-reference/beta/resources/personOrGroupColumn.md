---
author: simonhult
description: O recurso personOrGroupColumn em uma columnDefinition indica que os valores da coluna representam uma pessoa ou grupo escolhido no diretório.
ms.date: 09/11/2017
title: PersonOrGroupColumn
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 9b7901b52bcd877df16f5507c450425484ada703
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521929"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="23b02-103">Tipo de recurso PersonOrGroupColumn</span><span class="sxs-lookup"><span data-stu-id="23b02-103">PersonOrGroupColumn resource type</span></span>

<span data-ttu-id="23b02-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="23b02-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23b02-105">O recurso **personOrGroupColumn** em uma [columnDefinition](columndefinition.md) indica que os valores da coluna representam uma pessoa ou grupo escolhido no diretório.</span><span class="sxs-lookup"><span data-stu-id="23b02-105">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="23b02-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23b02-106">JSON representation</span></span>

<span data-ttu-id="23b02-107">Aqui está uma representação JSON de um recurso **personOrGroupColumn**.</span><span class="sxs-lookup"><span data-stu-id="23b02-107">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="23b02-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23b02-108">Properties</span></span>

| <span data-ttu-id="23b02-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="23b02-109">Property name</span></span>              | <span data-ttu-id="23b02-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="23b02-110">Type</span></span>    | <span data-ttu-id="23b02-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="23b02-111">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="23b02-112">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="23b02-112">**allowMultipleSelection**</span></span> | <span data-ttu-id="23b02-113">booliano</span><span class="sxs-lookup"><span data-stu-id="23b02-113">boolean</span></span> | <span data-ttu-id="23b02-114">Indica se vários valores podem ser selecionados da origem.</span><span class="sxs-lookup"><span data-stu-id="23b02-114">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="23b02-115">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="23b02-115">**displayAs**</span></span>              | <span data-ttu-id="23b02-116">string</span><span class="sxs-lookup"><span data-stu-id="23b02-116">string</span></span>  | <span data-ttu-id="23b02-117">Como exibir as informações sobre a pessoa ou grupo escolhido.</span><span class="sxs-lookup"><span data-stu-id="23b02-117">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="23b02-118">Veja a seguir.</span><span class="sxs-lookup"><span data-stu-id="23b02-118">See below.</span></span>
| <span data-ttu-id="23b02-119">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="23b02-119">**chooseFromType**</span></span>         | <span data-ttu-id="23b02-120">string</span><span class="sxs-lookup"><span data-stu-id="23b02-120">string</span></span>  | <span data-ttu-id="23b02-121">Se permite somente a seleção de pessoas, ou de pessoas e grupos.</span><span class="sxs-lookup"><span data-stu-id="23b02-121">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="23b02-122">Deve ser `peopleAndGroups` ou `peopleOnly`.</span><span class="sxs-lookup"><span data-stu-id="23b02-122">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-values"></a><span data-ttu-id="23b02-123">Valores de displayAs</span><span class="sxs-lookup"><span data-stu-id="23b02-123">DisplayAs values</span></span>

| <span data-ttu-id="23b02-124">Valor de displayAs</span><span class="sxs-lookup"><span data-stu-id="23b02-124">DisplayAs value</span></span>               | <span data-ttu-id="23b02-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="23b02-125">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="23b02-126">**account**</span><span class="sxs-lookup"><span data-stu-id="23b02-126">**account**</span></span>                   | <span data-ttu-id="23b02-127">A cadeia de caracteres de declaração codificada bruta do SharePoint para a pessoa ou grupo (por exemplo.</span><span class="sxs-lookup"><span data-stu-id="23b02-127">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="23b02-128">i:0#.f</span><span class="sxs-lookup"><span data-stu-id="23b02-128">i:0#.f</span></span>|<span data-ttu-id="23b02-129">membership</span><span class="sxs-lookup"><span data-stu-id="23b02-129">membership</span></span>|<span data-ttu-id="23b02-130">jane@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="23b02-130">jane@contoso.com).</span></span>
| <span data-ttu-id="23b02-131">**department**</span><span class="sxs-lookup"><span data-stu-id="23b02-131">**department**</span></span>                | <span data-ttu-id="23b02-132">O departamento da pessoa ou grupo.</span><span class="sxs-lookup"><span data-stu-id="23b02-132">The person or group's department.</span></span>
| <span data-ttu-id="23b02-133">**firstName**</span><span class="sxs-lookup"><span data-stu-id="23b02-133">**firstName**</span></span>                 | <span data-ttu-id="23b02-134">O primeiro nome da pessoa.</span><span class="sxs-lookup"><span data-stu-id="23b02-134">The person's first name.</span></span>
| <span data-ttu-id="23b02-135">**id**</span><span class="sxs-lookup"><span data-stu-id="23b02-135">**id**</span></span>                        | <span data-ttu-id="23b02-136">A id da pessoa ou grupo no diretório.</span><span class="sxs-lookup"><span data-stu-id="23b02-136">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="23b02-137">**lastName**</span><span class="sxs-lookup"><span data-stu-id="23b02-137">**lastName**</span></span>                  | <span data-ttu-id="23b02-138">O sobrenome da pessoa.</span><span class="sxs-lookup"><span data-stu-id="23b02-138">The person's last name.</span></span>
| <span data-ttu-id="23b02-139">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="23b02-139">**mobilePhone**</span></span>               | <span data-ttu-id="23b02-140">O número de celular da pessoa.</span><span class="sxs-lookup"><span data-stu-id="23b02-140">The person's mobile phone number.</span></span>
| <span data-ttu-id="23b02-141">**name**</span><span class="sxs-lookup"><span data-stu-id="23b02-141">**name**</span></span>                      | <span data-ttu-id="23b02-142">O nome da pessoa.</span><span class="sxs-lookup"><span data-stu-id="23b02-142">The person's name.</span></span>
| <span data-ttu-id="23b02-143">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="23b02-143">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="23b02-144">O nome da pessoa com sua imagem e detalhes adicionais.</span><span class="sxs-lookup"><span data-stu-id="23b02-144">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="23b02-145">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="23b02-145">**nameWithPresence**</span></span>          | <span data-ttu-id="23b02-146">Padrão.</span><span class="sxs-lookup"><span data-stu-id="23b02-146">Default.</span></span> <span data-ttu-id="23b02-147">O nome da pessoa com um ícone indicador de presença (disponível/ocupado/etc.)</span><span class="sxs-lookup"><span data-stu-id="23b02-147">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="23b02-148">**office**</span><span class="sxs-lookup"><span data-stu-id="23b02-148">**office**</span></span>                    | <span data-ttu-id="23b02-149">O número comercial da pessoa.</span><span class="sxs-lookup"><span data-stu-id="23b02-149">The person's office number.</span></span>
| <span data-ttu-id="23b02-150">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="23b02-150">**pictureOnly36x36**</span></span>          | <span data-ttu-id="23b02-151">Imagem da pessoa, delimitada por um quadrado de 36 x 36 pixels.</span><span class="sxs-lookup"><span data-stu-id="23b02-151">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="23b02-152">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="23b02-152">**pictureOnly48x48**</span></span>          | <span data-ttu-id="23b02-153">Imagem da pessoa, delimitada por um quadrado de 48 x 48 pixels.</span><span class="sxs-lookup"><span data-stu-id="23b02-153">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="23b02-154">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="23b02-154">**pictureOnly72x72**</span></span>          | <span data-ttu-id="23b02-155">Imagem da pessoa, delimitada por um quadrado de 72 x 72 pixels.</span><span class="sxs-lookup"><span data-stu-id="23b02-155">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="23b02-156">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="23b02-156">**sipAddress**</span></span>                | <span data-ttu-id="23b02-157">O endereço sip da pessoa.</span><span class="sxs-lookup"><span data-stu-id="23b02-157">The person's sip address.</span></span>
| <span data-ttu-id="23b02-158">**title**</span><span class="sxs-lookup"><span data-stu-id="23b02-158">**title**</span></span>                     | <span data-ttu-id="23b02-159">O cargo da pessoa na organização.</span><span class="sxs-lookup"><span data-stu-id="23b02-159">The person's title in the organization.</span></span>
| <span data-ttu-id="23b02-160">**userName**</span><span class="sxs-lookup"><span data-stu-id="23b02-160">**userName**</span></span>                  | <span data-ttu-id="23b02-161">O nome de usuário da pessoa ou grupo.</span><span class="sxs-lookup"><span data-stu-id="23b02-161">The person or group's user name.</span></span>
| <span data-ttu-id="23b02-162">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="23b02-162">**workEmail**</span></span>                 | <span data-ttu-id="23b02-163">O endereço de email da pessoa ou grupo.</span><span class="sxs-lookup"><span data-stu-id="23b02-163">The person or group's email address.</span></span>
| <span data-ttu-id="23b02-164">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="23b02-164">**workPhone**</span></span>                 | <span data-ttu-id="23b02-165">O número de telefone comercial da pessoa.</span><span class="sxs-lookup"><span data-stu-id="23b02-165">The person's work phone number.</span></span>

<span data-ttu-id="23b02-166">Observação: podem ser retornados tipos adicionais de DisplayAs.</span><span class="sxs-lookup"><span data-stu-id="23b02-166">Note: Additional DisplayAs types may be returned.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/PersonOrGroupColumn",
  "suppressions": []
}
-->
