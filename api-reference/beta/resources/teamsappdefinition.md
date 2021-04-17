---
title: Tipo de recurso teamsAppDefinition
description: Os detalhes de uma versão de um teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4e8bfd4b7248d37ce8ec4d85e01a498a88fed1c3
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882317"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="34b49-103">Tipo de recurso teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="34b49-103">teamsAppDefinition resource type</span></span>

<span data-ttu-id="34b49-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34b49-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34b49-105">Os detalhes de uma versão de um [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="34b49-105">The details of a version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="34b49-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="34b49-106">Properties</span></span>

| <span data-ttu-id="34b49-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34b49-107">Property</span></span>            | <span data-ttu-id="34b49-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="34b49-108">Type</span></span>     | <span data-ttu-id="34b49-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="34b49-109">Description</span></span>                                            |
|:------------------- |:-------- |:------------------------------------------------------ |
| <span data-ttu-id="34b49-110">id</span><span class="sxs-lookup"><span data-stu-id="34b49-110">id</span></span>                  | <span data-ttu-id="34b49-111">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34b49-111">string</span></span>   | <span data-ttu-id="34b49-112">Uma ID exclusiva (não a ID do aplicativo do Teams).</span><span class="sxs-lookup"><span data-stu-id="34b49-112">A unique ID (not the Teams app ID).</span></span>                     |
| <span data-ttu-id="34b49-113">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="34b49-113">teamsAppId</span></span>          | <span data-ttu-id="34b49-114">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34b49-114">string</span></span>   | <span data-ttu-id="34b49-115">A ID do manifesto do aplicativo teams.</span><span class="sxs-lookup"><span data-stu-id="34b49-115">The ID from the Teams app manifest.</span></span>                    |
| <span data-ttu-id="34b49-116">publishingState</span><span class="sxs-lookup"><span data-stu-id="34b49-116">publishingState</span></span>     | <span data-ttu-id="34b49-117">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34b49-117">string</span></span>   | <span data-ttu-id="34b49-118">O status publicado de uma versão específica de um aplicativo do Teams.</span><span class="sxs-lookup"><span data-stu-id="34b49-118">The published status of a specific version of a Teams app.</span></span> <span data-ttu-id="34b49-119">Os valores possíveis são:</span><span class="sxs-lookup"><span data-stu-id="34b49-119">Possible values are:</span></span></br><span data-ttu-id="34b49-120">`submitted` — A versão específica do aplicativo teams foi enviada e está sob revisão.</span><span class="sxs-lookup"><span data-stu-id="34b49-120">`submitted` — The specific version of the Teams app has been submitted and is under review.</span></span> </br><span data-ttu-id="34b49-121">`published`  — A solicitação para publicar a versão específica do aplicativo teams foi aprovada pelo administrador e o aplicativo é publicado.</span><span class="sxs-lookup"><span data-stu-id="34b49-121">`published`  — The request to publish the specific version of the Teams app has been approved by the admin and the app is published.</span></span> </br> <span data-ttu-id="34b49-122">`rejected` — A solicitação para publicar a versão específica do aplicativo teams foi rejeitada pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="34b49-122">`rejected` — The request to publish the specific version of the Teams app was rejected by the admin.</span></span> |
| <span data-ttu-id="34b49-123">azureADAppId</span><span class="sxs-lookup"><span data-stu-id="34b49-123">azureADAppId</span></span>        | <span data-ttu-id="34b49-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34b49-124">string</span></span>   | <span data-ttu-id="34b49-125">O WebApplicationInfo.Id do manifesto do aplicativo teams.</span><span class="sxs-lookup"><span data-stu-id="34b49-125">The WebApplicationInfo.Id from the Teams app manifest.</span></span> |
| <span data-ttu-id="34b49-126">displayName</span><span class="sxs-lookup"><span data-stu-id="34b49-126">displayName</span></span>         | <span data-ttu-id="34b49-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34b49-127">string</span></span>   | <span data-ttu-id="34b49-128">O nome do aplicativo fornecido pelo desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="34b49-128">The name of the app provided by the app developer.</span></span>     |
| <span data-ttu-id="34b49-129">versão</span><span class="sxs-lookup"><span data-stu-id="34b49-129">version</span></span>             | <span data-ttu-id="34b49-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34b49-130">string</span></span>   | <span data-ttu-id="34b49-131">O número da versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="34b49-131">The version number of the application.</span></span>                 |
| <span data-ttu-id="34b49-132">allowedInstallationScopes</span><span class="sxs-lookup"><span data-stu-id="34b49-132">allowedInstallationScopes</span></span> | <span data-ttu-id="34b49-133">Coleção teamsAppInstallationScope</span><span class="sxs-lookup"><span data-stu-id="34b49-133">teamsAppInstallationScope collection</span></span> | <span data-ttu-id="34b49-134">Uma coleção de escopos onde o aplicativo teams pode ser instalado.</span><span class="sxs-lookup"><span data-stu-id="34b49-134">A collection of scopes where the Teams app can be installed.</span></span> <span data-ttu-id="34b49-135">Os valores possíveis são:</span><span class="sxs-lookup"><span data-stu-id="34b49-135">Possible values are:</span></span></br><span data-ttu-id="34b49-136">`team` — Indica que o aplicativo do Teams pode ser instalado em uma equipe e está autorizado a acessar os dados dessa equipe.</span><span class="sxs-lookup"><span data-stu-id="34b49-136">`team` — Indicates that the Teams app can be installed within a team and is authorized to access that team's data.</span></span> </br><span data-ttu-id="34b49-137">`groupChat`  — Indica que o aplicativo do Teams pode ser instalado em um chat de grupo e está autorizado a acessar os dados desse chat de grupo.</span><span class="sxs-lookup"><span data-stu-id="34b49-137">`groupChat`  — Indicates that the Teams app can be installed within a group chat and is authorized to access that group chat's data.</span></span> </br> <span data-ttu-id="34b49-138">`personal` — Indica que o aplicativo do Teams pode ser instalado no escopo pessoal de um usuário e está autorizado a acessar os dados desse usuário.</span><span class="sxs-lookup"><span data-stu-id="34b49-138">`personal` — Indicates that the Teams app can be installed in the personal scope of a user and is authorized to access that user's data.</span></span> | 

## <a name="relationships"></a><span data-ttu-id="34b49-139">Relações</span><span class="sxs-lookup"><span data-stu-id="34b49-139">Relationships</span></span>

| <span data-ttu-id="34b49-140">Relação</span><span class="sxs-lookup"><span data-stu-id="34b49-140">Relationship</span></span>   | <span data-ttu-id="34b49-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="34b49-141">Type</span></span>                           | <span data-ttu-id="34b49-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="34b49-142">Description</span></span>                                                 |
|:-------------- |:------------------------------ |:----------------------------------------------------------- |
| <span data-ttu-id="34b49-143">bot</span><span class="sxs-lookup"><span data-stu-id="34b49-143">bot</span></span>            |[<span data-ttu-id="34b49-144">teamworkBot</span><span class="sxs-lookup"><span data-stu-id="34b49-144">teamworkBot</span></span>](teamworkbot.md)   | <span data-ttu-id="34b49-145">Os detalhes do bot especificados no manifesto do aplicativo teams.</span><span class="sxs-lookup"><span data-stu-id="34b49-145">The details of the bot specified in the Teams app manifest.</span></span> |
| <span data-ttu-id="34b49-146">colorIcon</span><span class="sxs-lookup"><span data-stu-id="34b49-146">colorIcon</span></span>      |[<span data-ttu-id="34b49-147">teamsAppIcon</span><span class="sxs-lookup"><span data-stu-id="34b49-147">teamsAppIcon</span></span>](teamsappicon.md) | <span data-ttu-id="34b49-148">A versão colorida do ícone do aplicativo Teams.</span><span class="sxs-lookup"><span data-stu-id="34b49-148">The color version of the Teams app's icon.</span></span>                   |
| <span data-ttu-id="34b49-149">outlineIcon</span><span class="sxs-lookup"><span data-stu-id="34b49-149">outlineIcon</span></span>    |[<span data-ttu-id="34b49-150">teamsAppIcon</span><span class="sxs-lookup"><span data-stu-id="34b49-150">teamsAppIcon</span></span>](teamsappicon.md) | <span data-ttu-id="34b49-151">A versão de contorno do ícone do aplicativo Teams.</span><span class="sxs-lookup"><span data-stu-id="34b49-151">The outline version of the Teams app's icon.</span></span>                 |

## <a name="json-representation"></a><span data-ttu-id="34b49-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="34b49-152">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppDefinition",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "teamsAppId": "string",
  "publishingState": "#microsoft.graph.teamsAppPublishingState",
  "azureADAppId": "string",
  "displayName": "string",
  "version": "string"
}
```

## <a name="see-also"></a><span data-ttu-id="34b49-153">Confira também</span><span class="sxs-lookup"><span data-stu-id="34b49-153">See also</span></span>

- [<span data-ttu-id="34b49-154">teamsApp</span><span class="sxs-lookup"><span data-stu-id="34b49-154">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="34b49-155">teamsAppIcon</span><span class="sxs-lookup"><span data-stu-id="34b49-155">teamsAppIcon</span></span>](teamsappicon.md)
- [<span data-ttu-id="34b49-156">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="34b49-156">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="34b49-157">teamsTab</span><span class="sxs-lookup"><span data-stu-id="34b49-157">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


