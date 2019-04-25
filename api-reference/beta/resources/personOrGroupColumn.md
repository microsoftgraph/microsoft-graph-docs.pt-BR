---
author: simonhult
ms.date: 09/11/2017
title: PersonOrGroupColumn
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: a3136d7c5b9563999eb9b21a9235317afdaeb63e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573939"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="282a5-102">Tipo de recurso PersonOrGroupColumn</span><span class="sxs-lookup"><span data-stu-id="282a5-102">PersonOrGroupColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="282a5-103">O recurso **personOrGroupColumn** em uma [columnDefinition](columndefinition.md) indica que os valores da coluna representam uma pessoa ou grupo escolhido no diretório.</span><span class="sxs-lookup"><span data-stu-id="282a5-103">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="282a5-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="282a5-104">JSON representation</span></span>

<span data-ttu-id="282a5-105">Aqui está uma representação JSON de um recurso **personOrGroupColumn**.</span><span class="sxs-lookup"><span data-stu-id="282a5-105">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="282a5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="282a5-106">Properties</span></span>

| <span data-ttu-id="282a5-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="282a5-107">Property name</span></span>              | <span data-ttu-id="282a5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="282a5-108">Type</span></span>    | <span data-ttu-id="282a5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="282a5-109">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="282a5-110">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="282a5-110">**allowMultipleSelection**</span></span> | <span data-ttu-id="282a5-111">booliano</span><span class="sxs-lookup"><span data-stu-id="282a5-111">boolean</span></span> | <span data-ttu-id="282a5-112">Indica se vários valores podem ser selecionados da origem.</span><span class="sxs-lookup"><span data-stu-id="282a5-112">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="282a5-113">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="282a5-113">**displayAs**</span></span>              | <span data-ttu-id="282a5-114">string</span><span class="sxs-lookup"><span data-stu-id="282a5-114">string</span></span>  | <span data-ttu-id="282a5-115">Como exibir as informações sobre a pessoa ou grupo escolhido.</span><span class="sxs-lookup"><span data-stu-id="282a5-115">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="282a5-116">Veja a seguir.</span><span class="sxs-lookup"><span data-stu-id="282a5-116">See below.</span></span>
| <span data-ttu-id="282a5-117">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="282a5-117">**chooseFromType**</span></span>         | <span data-ttu-id="282a5-118">string</span><span class="sxs-lookup"><span data-stu-id="282a5-118">string</span></span>  | <span data-ttu-id="282a5-119">Se permite somente a seleção de pessoas, ou de pessoas e grupos.</span><span class="sxs-lookup"><span data-stu-id="282a5-119">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="282a5-120">Deve ser `peopleAndGroups` ou `peopleOnly`.</span><span class="sxs-lookup"><span data-stu-id="282a5-120">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-values"></a><span data-ttu-id="282a5-121">Valores de displayAs</span><span class="sxs-lookup"><span data-stu-id="282a5-121">DisplayAs values</span></span>

| <span data-ttu-id="282a5-122">Valor de displayAs</span><span class="sxs-lookup"><span data-stu-id="282a5-122">DisplayAs value</span></span>               | <span data-ttu-id="282a5-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="282a5-123">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="282a5-124">**account**</span><span class="sxs-lookup"><span data-stu-id="282a5-124">**account**</span></span>                   | <span data-ttu-id="282a5-125">A cadeia de caracteres de declaração codificada bruta do SharePoint para a pessoa ou grupo (por exemplo.</span><span class="sxs-lookup"><span data-stu-id="282a5-125">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="282a5-126">i:0#.f</span><span class="sxs-lookup"><span data-stu-id="282a5-126">i:0#.f</span></span>|<span data-ttu-id="282a5-127">membership</span><span class="sxs-lookup"><span data-stu-id="282a5-127">membership</span></span>|<span data-ttu-id="282a5-128">jane@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="282a5-128">jane@contoso.com).</span></span>
| <span data-ttu-id="282a5-129">**department**</span><span class="sxs-lookup"><span data-stu-id="282a5-129">**department**</span></span>                | <span data-ttu-id="282a5-130">O departamento da pessoa ou grupo.</span><span class="sxs-lookup"><span data-stu-id="282a5-130">The person or group's department.</span></span>
| <span data-ttu-id="282a5-131">**firstName**</span><span class="sxs-lookup"><span data-stu-id="282a5-131">**firstName**</span></span>                 | <span data-ttu-id="282a5-132">O primeiro nome da pessoa.</span><span class="sxs-lookup"><span data-stu-id="282a5-132">The person's first name.</span></span>
| <span data-ttu-id="282a5-133">**id**</span><span class="sxs-lookup"><span data-stu-id="282a5-133">**id**</span></span>                        | <span data-ttu-id="282a5-134">A id da pessoa ou grupo no diretório.</span><span class="sxs-lookup"><span data-stu-id="282a5-134">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="282a5-135">**lastName**</span><span class="sxs-lookup"><span data-stu-id="282a5-135">**lastName**</span></span>                  | <span data-ttu-id="282a5-136">O sobrenome da pessoa.</span><span class="sxs-lookup"><span data-stu-id="282a5-136">The person's last name.</span></span>
| <span data-ttu-id="282a5-137">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="282a5-137">**mobilePhone**</span></span>               | <span data-ttu-id="282a5-138">O número de celular da pessoa.</span><span class="sxs-lookup"><span data-stu-id="282a5-138">The person's mobile phone number.</span></span>
| <span data-ttu-id="282a5-139">**name**</span><span class="sxs-lookup"><span data-stu-id="282a5-139">**name**</span></span>                      | <span data-ttu-id="282a5-140">O nome da pessoa.</span><span class="sxs-lookup"><span data-stu-id="282a5-140">The person's name.</span></span>
| <span data-ttu-id="282a5-141">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="282a5-141">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="282a5-142">O nome da pessoa com sua imagem e detalhes adicionais.</span><span class="sxs-lookup"><span data-stu-id="282a5-142">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="282a5-143">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="282a5-143">**nameWithPresence**</span></span>          | <span data-ttu-id="282a5-144">Padrão.</span><span class="sxs-lookup"><span data-stu-id="282a5-144">Default.</span></span> <span data-ttu-id="282a5-145">O nome da pessoa com um ícone indicador de presença (disponível/ocupado/etc.)</span><span class="sxs-lookup"><span data-stu-id="282a5-145">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="282a5-146">**office**</span><span class="sxs-lookup"><span data-stu-id="282a5-146">**office**</span></span>                    | <span data-ttu-id="282a5-147">O número comercial da pessoa.</span><span class="sxs-lookup"><span data-stu-id="282a5-147">The person's office number.</span></span>
| <span data-ttu-id="282a5-148">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="282a5-148">**pictureOnly36x36**</span></span>          | <span data-ttu-id="282a5-149">Imagem da pessoa, delimitada por um quadrado de 36 x 36 pixels.</span><span class="sxs-lookup"><span data-stu-id="282a5-149">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="282a5-150">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="282a5-150">**pictureOnly48x48**</span></span>          | <span data-ttu-id="282a5-151">Imagem da pessoa, delimitada por um quadrado de 48 x 48 pixels.</span><span class="sxs-lookup"><span data-stu-id="282a5-151">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="282a5-152">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="282a5-152">**pictureOnly72x72**</span></span>          | <span data-ttu-id="282a5-153">Imagem da pessoa, delimitada por um quadrado de 72 x 72 pixels.</span><span class="sxs-lookup"><span data-stu-id="282a5-153">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="282a5-154">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="282a5-154">**sipAddress**</span></span>                | <span data-ttu-id="282a5-155">O endereço sip da pessoa.</span><span class="sxs-lookup"><span data-stu-id="282a5-155">The person's sip address.</span></span>
| <span data-ttu-id="282a5-156">**title**</span><span class="sxs-lookup"><span data-stu-id="282a5-156">**title**</span></span>                     | <span data-ttu-id="282a5-157">O cargo da pessoa na organização.</span><span class="sxs-lookup"><span data-stu-id="282a5-157">The person's title in the organization.</span></span>
| <span data-ttu-id="282a5-158">**userName**</span><span class="sxs-lookup"><span data-stu-id="282a5-158">**userName**</span></span>                  | <span data-ttu-id="282a5-159">O nome de usuário da pessoa ou grupo.</span><span class="sxs-lookup"><span data-stu-id="282a5-159">The person or group's user name.</span></span>
| <span data-ttu-id="282a5-160">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="282a5-160">**workEmail**</span></span>                 | <span data-ttu-id="282a5-161">O endereço de email da pessoa ou grupo.</span><span class="sxs-lookup"><span data-stu-id="282a5-161">The person or group's email address.</span></span>
| <span data-ttu-id="282a5-162">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="282a5-162">**workPhone**</span></span>                 | <span data-ttu-id="282a5-163">O número de telefone comercial da pessoa.</span><span class="sxs-lookup"><span data-stu-id="282a5-163">The person's work phone number.</span></span>

<span data-ttu-id="282a5-164">Observação: podem ser retornados tipos adicionais de DisplayAs.</span><span class="sxs-lookup"><span data-stu-id="282a5-164">Note: Additional DisplayAs types may be returned.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/PersonOrGroupColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/personOrGroupColumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
