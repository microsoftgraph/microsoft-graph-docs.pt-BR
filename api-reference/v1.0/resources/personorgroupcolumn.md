---
author: simonhult
ms.date: 09/11/2017
title: PersonOrGroupColumn
localization_priority: Normal
ms.prod: insights
description: O recurso personOrGroupColumn em uma columnDefinition indica que os valores da coluna representam uma pessoa ou grupo escolhido no diretório.
doc_type: resourcePageType
ms.openlocfilehash: b9c3774405dbb8d2e98a9823a84be97d5df09b0b
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845474"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="c8ff1-103">Tipo de recurso PersonOrGroupColumn</span><span class="sxs-lookup"><span data-stu-id="c8ff1-103">PersonOrGroupColumn resource type</span></span>

<span data-ttu-id="c8ff1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8ff1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c8ff1-105">O recurso **personOrGroupColumn** em uma [columnDefinition](columndefinition.md) indica que os valores da coluna representam uma pessoa ou grupo escolhido no diretório.</span><span class="sxs-lookup"><span data-stu-id="c8ff1-105">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8ff1-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c8ff1-106">JSON representation</span></span>

<span data-ttu-id="c8ff1-107">Aqui está uma representação JSON de um recurso **personOrGroupColumn**.</span><span class="sxs-lookup"><span data-stu-id="c8ff1-107">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="c8ff1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c8ff1-108">Properties</span></span>

| <span data-ttu-id="c8ff1-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="c8ff1-109">Property name</span></span>              | <span data-ttu-id="c8ff1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8ff1-110">Type</span></span>    | <span data-ttu-id="c8ff1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8ff1-111">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="c8ff1-112">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="c8ff1-112">**allowMultipleSelection**</span></span> | <span data-ttu-id="c8ff1-113">booliano</span><span class="sxs-lookup"><span data-stu-id="c8ff1-113">boolean</span></span> | <span data-ttu-id="c8ff1-114">Indica se vários valores podem ser selecionados da origem.</span><span class="sxs-lookup"><span data-stu-id="c8ff1-114">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="c8ff1-115">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="c8ff1-115">**displayAs**</span></span>              | <span data-ttu-id="c8ff1-116">string</span><span class="sxs-lookup"><span data-stu-id="c8ff1-116">string</span></span>  | <span data-ttu-id="c8ff1-117">Como exibir as informações sobre a pessoa ou grupo escolhido.</span><span class="sxs-lookup"><span data-stu-id="c8ff1-117">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="c8ff1-118">Veja a seguir.</span><span class="sxs-lookup"><span data-stu-id="c8ff1-118">See below.</span></span>
| <span data-ttu-id="c8ff1-119">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="c8ff1-119">**chooseFromType**</span></span>         | <span data-ttu-id="c8ff1-120">string</span><span class="sxs-lookup"><span data-stu-id="c8ff1-120">string</span></span>  | <span data-ttu-id="c8ff1-121">Se permite somente a seleção de pessoas, ou de pessoas e grupos.</span><span class="sxs-lookup"><span data-stu-id="c8ff1-121">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="c8ff1-122">Deve ser `peopleAndGroups` ou `peopleOnly`.</span><span class="sxs-lookup"><span data-stu-id="c8ff1-122">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-options"></a><span data-ttu-id="c8ff1-123">Opções de displayas</span><span class="sxs-lookup"><span data-stu-id="c8ff1-123">DisplayAs options</span></span>

| <span data-ttu-id="c8ff1-124">Valor de displayAs</span><span class="sxs-lookup"><span data-stu-id="c8ff1-124">DisplayAs value</span></span>               | <span data-ttu-id="c8ff1-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8ff1-125">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="c8ff1-126">**account**</span><span class="sxs-lookup"><span data-stu-id="c8ff1-126">**account**</span></span>                   | <span data-ttu-id="c8ff1-127">A cadeia de caracteres de declaração codificada bruta do SharePoint para a pessoa ou grupo (por exemplo.</span><span class="sxs-lookup"><span data-stu-id="c8ff1-127">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="c8ff1-128">`i:0#.f|membership|jane@contoso.com`).</span><span class="sxs-lookup"><span data-stu-id="c8ff1-128">`i:0#.f|membership|jane@contoso.com`).</span></span>
| <span data-ttu-id="c8ff1-129">**department**</span><span class="sxs-lookup"><span data-stu-id="c8ff1-129">**department**</span></span>                | <span data-ttu-id="c8ff1-130">O departamento da pessoa ou grupo.</span><span class="sxs-lookup"><span data-stu-id="c8ff1-130">The person or group's department.</span></span>
| <span data-ttu-id="c8ff1-131">**firstName**</span><span class="sxs-lookup"><span data-stu-id="c8ff1-131">**firstName**</span></span>                 | <span data-ttu-id="c8ff1-132">O primeiro nome da pessoa.</span><span class="sxs-lookup"><span data-stu-id="c8ff1-132">The person's first name.</span></span>
| <span data-ttu-id="c8ff1-133">**id**</span><span class="sxs-lookup"><span data-stu-id="c8ff1-133">**id**</span></span>                        | <span data-ttu-id="c8ff1-134">A id da pessoa ou grupo no diretório.</span><span class="sxs-lookup"><span data-stu-id="c8ff1-134">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="c8ff1-135">**lastName**</span><span class="sxs-lookup"><span data-stu-id="c8ff1-135">**lastName**</span></span>                  | <span data-ttu-id="c8ff1-136">O sobrenome da pessoa.</span><span class="sxs-lookup"><span data-stu-id="c8ff1-136">The person's last name.</span></span>
| <span data-ttu-id="c8ff1-137">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="c8ff1-137">**mobilePhone**</span></span>               | <span data-ttu-id="c8ff1-138">O número de celular da pessoa.</span><span class="sxs-lookup"><span data-stu-id="c8ff1-138">The person's mobile phone number.</span></span>
| <span data-ttu-id="c8ff1-139">**name**</span><span class="sxs-lookup"><span data-stu-id="c8ff1-139">**name**</span></span>                      | <span data-ttu-id="c8ff1-140">O nome da pessoa.</span><span class="sxs-lookup"><span data-stu-id="c8ff1-140">The person's name.</span></span>
| <span data-ttu-id="c8ff1-141">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="c8ff1-141">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="c8ff1-142">O nome da pessoa com sua imagem e detalhes adicionais.</span><span class="sxs-lookup"><span data-stu-id="c8ff1-142">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="c8ff1-143">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="c8ff1-143">**nameWithPresence**</span></span>          | <span data-ttu-id="c8ff1-144">Padrão.</span><span class="sxs-lookup"><span data-stu-id="c8ff1-144">Default.</span></span> <span data-ttu-id="c8ff1-145">O nome da pessoa com um ícone indicador de presença (disponível/ocupado/etc.)</span><span class="sxs-lookup"><span data-stu-id="c8ff1-145">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="c8ff1-146">**office**</span><span class="sxs-lookup"><span data-stu-id="c8ff1-146">**office**</span></span>                    | <span data-ttu-id="c8ff1-147">O número comercial da pessoa.</span><span class="sxs-lookup"><span data-stu-id="c8ff1-147">The person's office number.</span></span>
| <span data-ttu-id="c8ff1-148">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="c8ff1-148">**pictureOnly36x36**</span></span>          | <span data-ttu-id="c8ff1-149">Imagem da pessoa, delimitada por um quadrado de 36 x 36 pixels.</span><span class="sxs-lookup"><span data-stu-id="c8ff1-149">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="c8ff1-150">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="c8ff1-150">**pictureOnly48x48**</span></span>          | <span data-ttu-id="c8ff1-151">Imagem da pessoa, delimitada por um quadrado de 48 x 48 pixels.</span><span class="sxs-lookup"><span data-stu-id="c8ff1-151">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="c8ff1-152">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="c8ff1-152">**pictureOnly72x72**</span></span>          | <span data-ttu-id="c8ff1-153">Imagem da pessoa, delimitada por um quadrado de 72 x 72 pixels.</span><span class="sxs-lookup"><span data-stu-id="c8ff1-153">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="c8ff1-154">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="c8ff1-154">**sipAddress**</span></span>                | <span data-ttu-id="c8ff1-155">O endereço sip da pessoa.</span><span class="sxs-lookup"><span data-stu-id="c8ff1-155">The person's sip address.</span></span>
| <span data-ttu-id="c8ff1-156">**title**</span><span class="sxs-lookup"><span data-stu-id="c8ff1-156">**title**</span></span>                     | <span data-ttu-id="c8ff1-157">O cargo da pessoa na organização.</span><span class="sxs-lookup"><span data-stu-id="c8ff1-157">The person's title in the organization.</span></span>
| <span data-ttu-id="c8ff1-158">**userName**</span><span class="sxs-lookup"><span data-stu-id="c8ff1-158">**userName**</span></span>                  | <span data-ttu-id="c8ff1-159">O nome de usuário da pessoa ou grupo.</span><span class="sxs-lookup"><span data-stu-id="c8ff1-159">The person or group's user name.</span></span>
| <span data-ttu-id="c8ff1-160">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="c8ff1-160">**workEmail**</span></span>                 | <span data-ttu-id="c8ff1-161">O endereço de email da pessoa ou grupo.</span><span class="sxs-lookup"><span data-stu-id="c8ff1-161">The person or group's email address.</span></span>
| <span data-ttu-id="c8ff1-162">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="c8ff1-162">**workPhone**</span></span>                 | <span data-ttu-id="c8ff1-163">O número de telefone comercial da pessoa.</span><span class="sxs-lookup"><span data-stu-id="c8ff1-163">The person's work phone number.</span></span>

<span data-ttu-id="c8ff1-164">Observação: podem ser retornados tipos adicionais de DisplayAs.</span><span class="sxs-lookup"><span data-stu-id="c8ff1-164">Note: Additional DisplayAs types may be returned.</span></span>

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
