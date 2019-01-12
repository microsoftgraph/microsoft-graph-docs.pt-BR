---
author: simonhult
ms.date: 09/11/2017
title: PersonOrGroupColumn
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: a1eb5b36f2af7b66da7fd891ccd324fa325504c3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923464"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="a4aad-102">Tipo de recurso PersonOrGroupColumn</span><span class="sxs-lookup"><span data-stu-id="a4aad-102">PersonOrGroupColumn resource type</span></span>

> <span data-ttu-id="a4aad-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a4aad-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a4aad-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a4aad-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a4aad-105">O recurso **personOrGroupColumn** em uma [columnDefinition](columndefinition.md) indica que os valores da coluna representam uma pessoa ou grupo escolhido no diretório.</span><span class="sxs-lookup"><span data-stu-id="a4aad-105">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4aad-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a4aad-106">JSON representation</span></span>

<span data-ttu-id="a4aad-107">Aqui está uma representação JSON de um recurso **personOrGroupColumn**.</span><span class="sxs-lookup"><span data-stu-id="a4aad-107">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="a4aad-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a4aad-108">Properties</span></span>

| <span data-ttu-id="a4aad-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="a4aad-109">Property name</span></span>              | <span data-ttu-id="a4aad-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4aad-110">Type</span></span>    | <span data-ttu-id="a4aad-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4aad-111">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="a4aad-112">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="a4aad-112">**allowMultipleSelection**</span></span> | <span data-ttu-id="a4aad-113">booliano</span><span class="sxs-lookup"><span data-stu-id="a4aad-113">boolean</span></span> | <span data-ttu-id="a4aad-114">Indica se vários valores podem ser selecionados da origem.</span><span class="sxs-lookup"><span data-stu-id="a4aad-114">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="a4aad-115">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="a4aad-115">**displayAs**</span></span>              | <span data-ttu-id="a4aad-116">string</span><span class="sxs-lookup"><span data-stu-id="a4aad-116">string</span></span>  | <span data-ttu-id="a4aad-117">Como exibir as informações sobre a pessoa ou grupo escolhido.</span><span class="sxs-lookup"><span data-stu-id="a4aad-117">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="a4aad-118">Veja a seguir.</span><span class="sxs-lookup"><span data-stu-id="a4aad-118">See below.</span></span>
| <span data-ttu-id="a4aad-119">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="a4aad-119">**chooseFromType**</span></span>         | <span data-ttu-id="a4aad-120">string</span><span class="sxs-lookup"><span data-stu-id="a4aad-120">string</span></span>  | <span data-ttu-id="a4aad-121">Se permite somente a seleção de pessoas, ou de pessoas e grupos.</span><span class="sxs-lookup"><span data-stu-id="a4aad-121">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="a4aad-122">Deve ser `peopleAndGroups` ou `peopleOnly`.</span><span class="sxs-lookup"><span data-stu-id="a4aad-122">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-values"></a><span data-ttu-id="a4aad-123">Valores de displayAs</span><span class="sxs-lookup"><span data-stu-id="a4aad-123">DisplayAs values</span></span>

| <span data-ttu-id="a4aad-124">Valor de displayAs</span><span class="sxs-lookup"><span data-stu-id="a4aad-124">DisplayAs value</span></span>               | <span data-ttu-id="a4aad-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4aad-125">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="a4aad-126">**account**</span><span class="sxs-lookup"><span data-stu-id="a4aad-126">**account**</span></span>                   | <span data-ttu-id="a4aad-127">A cadeia de caracteres de declaração codificada bruta do SharePoint para a pessoa ou grupo (por exemplo.</span><span class="sxs-lookup"><span data-stu-id="a4aad-127">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="a4aad-128">i:0#.f</span><span class="sxs-lookup"><span data-stu-id="a4aad-128">i:0#.f</span></span>|<span data-ttu-id="a4aad-129">membership</span><span class="sxs-lookup"><span data-stu-id="a4aad-129">membership</span></span>|<span data-ttu-id="a4aad-130">jane@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="a4aad-130">jane@contoso.com).</span></span>
| <span data-ttu-id="a4aad-131">**department**</span><span class="sxs-lookup"><span data-stu-id="a4aad-131">**department**</span></span>                | <span data-ttu-id="a4aad-132">O departamento da pessoa ou grupo.</span><span class="sxs-lookup"><span data-stu-id="a4aad-132">The person or group's department.</span></span>
| <span data-ttu-id="a4aad-133">**firstName**</span><span class="sxs-lookup"><span data-stu-id="a4aad-133">**firstName**</span></span>                 | <span data-ttu-id="a4aad-134">O primeiro nome da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4aad-134">The person's first name.</span></span>
| <span data-ttu-id="a4aad-135">**id**</span><span class="sxs-lookup"><span data-stu-id="a4aad-135">**id**</span></span>                        | <span data-ttu-id="a4aad-136">A id da pessoa ou grupo no diretório.</span><span class="sxs-lookup"><span data-stu-id="a4aad-136">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="a4aad-137">**lastName**</span><span class="sxs-lookup"><span data-stu-id="a4aad-137">**lastName**</span></span>                  | <span data-ttu-id="a4aad-138">O sobrenome da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4aad-138">The person's last name.</span></span>
| <span data-ttu-id="a4aad-139">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="a4aad-139">**mobilePhone**</span></span>               | <span data-ttu-id="a4aad-140">O número de celular da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4aad-140">The person's mobile phone number.</span></span>
| <span data-ttu-id="a4aad-141">**name**</span><span class="sxs-lookup"><span data-stu-id="a4aad-141">**name**</span></span>                      | <span data-ttu-id="a4aad-142">O nome da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4aad-142">The person's name.</span></span>
| <span data-ttu-id="a4aad-143">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="a4aad-143">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="a4aad-144">O nome da pessoa com sua imagem e detalhes adicionais.</span><span class="sxs-lookup"><span data-stu-id="a4aad-144">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="a4aad-145">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="a4aad-145">**nameWithPresence**</span></span>          | <span data-ttu-id="a4aad-146">Padrão.</span><span class="sxs-lookup"><span data-stu-id="a4aad-146">Default.</span></span> <span data-ttu-id="a4aad-147">O nome da pessoa com um ícone indicador de presença (disponível/ocupado/etc.)</span><span class="sxs-lookup"><span data-stu-id="a4aad-147">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="a4aad-148">**office**</span><span class="sxs-lookup"><span data-stu-id="a4aad-148">**office**</span></span>                    | <span data-ttu-id="a4aad-149">O número comercial da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4aad-149">The person's office number.</span></span>
| <span data-ttu-id="a4aad-150">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="a4aad-150">**pictureOnly36x36**</span></span>          | <span data-ttu-id="a4aad-151">Imagem da pessoa, delimitada por um quadrado de 36 x 36 pixels.</span><span class="sxs-lookup"><span data-stu-id="a4aad-151">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="a4aad-152">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="a4aad-152">**pictureOnly48x48**</span></span>          | <span data-ttu-id="a4aad-153">Imagem da pessoa, delimitada por um quadrado de 48 x 48 pixels.</span><span class="sxs-lookup"><span data-stu-id="a4aad-153">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="a4aad-154">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="a4aad-154">**pictureOnly72x72**</span></span>          | <span data-ttu-id="a4aad-155">Imagem da pessoa, delimitada por um quadrado de 72 x 72 pixels.</span><span class="sxs-lookup"><span data-stu-id="a4aad-155">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="a4aad-156">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="a4aad-156">**sipAddress**</span></span>                | <span data-ttu-id="a4aad-157">O endereço sip da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4aad-157">The person's sip address.</span></span>
| <span data-ttu-id="a4aad-158">**title**</span><span class="sxs-lookup"><span data-stu-id="a4aad-158">**title**</span></span>                     | <span data-ttu-id="a4aad-159">O cargo da pessoa na organização.</span><span class="sxs-lookup"><span data-stu-id="a4aad-159">The person's title in the organization.</span></span>
| <span data-ttu-id="a4aad-160">**userName**</span><span class="sxs-lookup"><span data-stu-id="a4aad-160">**userName**</span></span>                  | <span data-ttu-id="a4aad-161">O nome de usuário da pessoa ou grupo.</span><span class="sxs-lookup"><span data-stu-id="a4aad-161">The person or group's user name.</span></span>
| <span data-ttu-id="a4aad-162">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="a4aad-162">**workEmail**</span></span>                 | <span data-ttu-id="a4aad-163">O endereço de email da pessoa ou grupo.</span><span class="sxs-lookup"><span data-stu-id="a4aad-163">The person or group's email address.</span></span>
| <span data-ttu-id="a4aad-164">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="a4aad-164">**workPhone**</span></span>                 | <span data-ttu-id="a4aad-165">O número de telefone comercial da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4aad-165">The person's work phone number.</span></span>

<span data-ttu-id="a4aad-166">Observação: podem ser retornados tipos adicionais de DisplayAs.</span><span class="sxs-lookup"><span data-stu-id="a4aad-166">Note: Additional DisplayAs types may be returned.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/PersonOrGroupColumn"
} -->
