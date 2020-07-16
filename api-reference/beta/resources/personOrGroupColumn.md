---
author: simonhult
description: O recurso personOrGroupColumn em uma columnDefinition indica que os valores da coluna representam uma pessoa ou grupo escolhido no diretório.
ms.date: 09/11/2017
title: PersonOrGroupColumn
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: c2b10d24acb1c4004de486904a8f2091c0a3db15
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845733"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="cc2b0-103">Tipo de recurso PersonOrGroupColumn</span><span class="sxs-lookup"><span data-stu-id="cc2b0-103">PersonOrGroupColumn resource type</span></span>

<span data-ttu-id="cc2b0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc2b0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc2b0-105">O recurso **personOrGroupColumn** em uma [columnDefinition](columndefinition.md) indica que os valores da coluna representam uma pessoa ou grupo escolhido no diretório.</span><span class="sxs-lookup"><span data-stu-id="cc2b0-105">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc2b0-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cc2b0-106">JSON representation</span></span>

<span data-ttu-id="cc2b0-107">Aqui está uma representação JSON de um recurso **personOrGroupColumn**.</span><span class="sxs-lookup"><span data-stu-id="cc2b0-107">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="cc2b0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cc2b0-108">Properties</span></span>

| <span data-ttu-id="cc2b0-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="cc2b0-109">Property name</span></span>              | <span data-ttu-id="cc2b0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc2b0-110">Type</span></span>    | <span data-ttu-id="cc2b0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc2b0-111">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="cc2b0-112">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="cc2b0-112">**allowMultipleSelection**</span></span> | <span data-ttu-id="cc2b0-113">booliano</span><span class="sxs-lookup"><span data-stu-id="cc2b0-113">boolean</span></span> | <span data-ttu-id="cc2b0-114">Indica se vários valores podem ser selecionados da origem.</span><span class="sxs-lookup"><span data-stu-id="cc2b0-114">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="cc2b0-115">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="cc2b0-115">**displayAs**</span></span>              | <span data-ttu-id="cc2b0-116">string</span><span class="sxs-lookup"><span data-stu-id="cc2b0-116">string</span></span>  | <span data-ttu-id="cc2b0-117">Como exibir as informações sobre a pessoa ou grupo escolhido.</span><span class="sxs-lookup"><span data-stu-id="cc2b0-117">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="cc2b0-118">Veja a seguir.</span><span class="sxs-lookup"><span data-stu-id="cc2b0-118">See below.</span></span>
| <span data-ttu-id="cc2b0-119">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="cc2b0-119">**chooseFromType**</span></span>         | <span data-ttu-id="cc2b0-120">string</span><span class="sxs-lookup"><span data-stu-id="cc2b0-120">string</span></span>  | <span data-ttu-id="cc2b0-121">Se permite somente a seleção de pessoas, ou de pessoas e grupos.</span><span class="sxs-lookup"><span data-stu-id="cc2b0-121">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="cc2b0-122">Deve ser `peopleAndGroups` ou `peopleOnly`.</span><span class="sxs-lookup"><span data-stu-id="cc2b0-122">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-values"></a><span data-ttu-id="cc2b0-123">Valores de displayAs</span><span class="sxs-lookup"><span data-stu-id="cc2b0-123">DisplayAs values</span></span>

| <span data-ttu-id="cc2b0-124">Valor de displayAs</span><span class="sxs-lookup"><span data-stu-id="cc2b0-124">DisplayAs value</span></span>               | <span data-ttu-id="cc2b0-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc2b0-125">Description</span></span>                                                                                                 |
|:------------------------------|:------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="cc2b0-126">**account**</span><span class="sxs-lookup"><span data-stu-id="cc2b0-126">**account**</span></span>                   | <span data-ttu-id="cc2b0-127">A cadeia de caracteres de declaração codificada bruta do SharePoint para a pessoa ou grupo (por exemplo.</span><span class="sxs-lookup"><span data-stu-id="cc2b0-127">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="cc2b0-128">`i:0#.f|membership|jane@contoso.com`).</span><span class="sxs-lookup"><span data-stu-id="cc2b0-128">`i:0#.f|membership|jane@contoso.com`).</span></span> |
| <span data-ttu-id="cc2b0-129">**department**</span><span class="sxs-lookup"><span data-stu-id="cc2b0-129">**department**</span></span>                | <span data-ttu-id="cc2b0-130">O departamento da pessoa ou grupo.</span><span class="sxs-lookup"><span data-stu-id="cc2b0-130">The person or group's department.</span></span>                                                                           |
| <span data-ttu-id="cc2b0-131">**firstName**</span><span class="sxs-lookup"><span data-stu-id="cc2b0-131">**firstName**</span></span>                 | <span data-ttu-id="cc2b0-132">O primeiro nome da pessoa.</span><span class="sxs-lookup"><span data-stu-id="cc2b0-132">The person's first name.</span></span>                                                                                    |
| <span data-ttu-id="cc2b0-133">**id**</span><span class="sxs-lookup"><span data-stu-id="cc2b0-133">**id**</span></span>                        | <span data-ttu-id="cc2b0-134">A id da pessoa ou grupo no diretório.</span><span class="sxs-lookup"><span data-stu-id="cc2b0-134">The id of the person or group in the directory.</span></span>                                                             |
| <span data-ttu-id="cc2b0-135">**lastName**</span><span class="sxs-lookup"><span data-stu-id="cc2b0-135">**lastName**</span></span>                  | <span data-ttu-id="cc2b0-136">O sobrenome da pessoa.</span><span class="sxs-lookup"><span data-stu-id="cc2b0-136">The person's last name.</span></span>                                                                                     |
| <span data-ttu-id="cc2b0-137">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="cc2b0-137">**mobilePhone**</span></span>               | <span data-ttu-id="cc2b0-138">O número de celular da pessoa.</span><span class="sxs-lookup"><span data-stu-id="cc2b0-138">The person's mobile phone number.</span></span>                                                                           |
| <span data-ttu-id="cc2b0-139">**name**</span><span class="sxs-lookup"><span data-stu-id="cc2b0-139">**name**</span></span>                      | <span data-ttu-id="cc2b0-140">O nome da pessoa.</span><span class="sxs-lookup"><span data-stu-id="cc2b0-140">The person's name.</span></span>                                                                                          |
| <span data-ttu-id="cc2b0-141">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="cc2b0-141">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="cc2b0-142">O nome da pessoa com sua imagem e detalhes adicionais.</span><span class="sxs-lookup"><span data-stu-id="cc2b0-142">The person's name along with their picture and additional details.</span></span>                                          |
| <span data-ttu-id="cc2b0-143">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="cc2b0-143">**nameWithPresence**</span></span>          | <span data-ttu-id="cc2b0-144">Padrão.</span><span class="sxs-lookup"><span data-stu-id="cc2b0-144">Default.</span></span> <span data-ttu-id="cc2b0-145">O nome da pessoa com um ícone indicador de presença (disponível/ocupado/etc.)</span><span class="sxs-lookup"><span data-stu-id="cc2b0-145">The person's name with a presence indicator icon (available/busy/etc.)</span></span>                             |
| <span data-ttu-id="cc2b0-146">**office**</span><span class="sxs-lookup"><span data-stu-id="cc2b0-146">**office**</span></span>                    | <span data-ttu-id="cc2b0-147">O número comercial da pessoa.</span><span class="sxs-lookup"><span data-stu-id="cc2b0-147">The person's office number.</span></span>                                                                                 |
| <span data-ttu-id="cc2b0-148">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="cc2b0-148">**pictureOnly36x36**</span></span>          | <span data-ttu-id="cc2b0-149">Imagem da pessoa, delimitada por um quadrado de 36 x 36 pixels.</span><span class="sxs-lookup"><span data-stu-id="cc2b0-149">The person's picture, bounded by a 36x36 px square.</span></span>                                                         |
| <span data-ttu-id="cc2b0-150">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="cc2b0-150">**pictureOnly48x48**</span></span>          | <span data-ttu-id="cc2b0-151">Imagem da pessoa, delimitada por um quadrado de 48 x 48 pixels.</span><span class="sxs-lookup"><span data-stu-id="cc2b0-151">The person's picture, bounded by a 48x48 px square.</span></span>                                                         |
| <span data-ttu-id="cc2b0-152">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="cc2b0-152">**pictureOnly72x72**</span></span>          | <span data-ttu-id="cc2b0-153">Imagem da pessoa, delimitada por um quadrado de 72 x 72 pixels.</span><span class="sxs-lookup"><span data-stu-id="cc2b0-153">The person's picture, bounded by a 72x72 px square.</span></span>                                                         |
| <span data-ttu-id="cc2b0-154">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="cc2b0-154">**sipAddress**</span></span>                | <span data-ttu-id="cc2b0-155">O endereço sip da pessoa.</span><span class="sxs-lookup"><span data-stu-id="cc2b0-155">The person's sip address.</span></span>                                                                                   |
| <span data-ttu-id="cc2b0-156">**title**</span><span class="sxs-lookup"><span data-stu-id="cc2b0-156">**title**</span></span>                     | <span data-ttu-id="cc2b0-157">O cargo da pessoa na organização.</span><span class="sxs-lookup"><span data-stu-id="cc2b0-157">The person's title in the organization.</span></span>                                                                     |
| <span data-ttu-id="cc2b0-158">**userName**</span><span class="sxs-lookup"><span data-stu-id="cc2b0-158">**userName**</span></span>                  | <span data-ttu-id="cc2b0-159">O nome de usuário da pessoa ou grupo.</span><span class="sxs-lookup"><span data-stu-id="cc2b0-159">The person or group's user name.</span></span>                                                                            |
| <span data-ttu-id="cc2b0-160">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="cc2b0-160">**workEmail**</span></span>                 | <span data-ttu-id="cc2b0-161">O endereço de email da pessoa ou grupo.</span><span class="sxs-lookup"><span data-stu-id="cc2b0-161">The person or group's email address.</span></span>                                                                        |
| <span data-ttu-id="cc2b0-162">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="cc2b0-162">**workPhone**</span></span>                 | <span data-ttu-id="cc2b0-163">O número de telefone comercial da pessoa.</span><span class="sxs-lookup"><span data-stu-id="cc2b0-163">The person's work phone number.</span></span>                                                                             |

<span data-ttu-id="cc2b0-164">Observação: podem ser retornados tipos adicionais de DisplayAs.</span><span class="sxs-lookup"><span data-stu-id="cc2b0-164">Note: Additional DisplayAs types may be returned.</span></span>

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
