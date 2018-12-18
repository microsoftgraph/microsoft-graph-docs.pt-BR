---
title: tipo de recurso de teamsAppInstallation
description: 'Um teamsApp instalado em uma equipe. '
author: nkramer
ms.openlocfilehash: cab42c3bc2bde2e20dff3478d432d70e1563d248
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341794"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="3be8e-103">tipo de recurso de teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="3be8e-103">teamsAppInstallation resource type</span></span>

> <span data-ttu-id="3be8e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3be8e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3be8e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3be8e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3be8e-106">Um [teamsApp](teamsapp.md) instalado em uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="3be8e-106">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="3be8e-107">Qualquer bots que fazem parte do aplicativo se tornará parte de qualquer aplicativo é adicionado de equipe.</span><span class="sxs-lookup"><span data-stu-id="3be8e-107">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="3be8e-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="3be8e-108">Methods</span></span>

| <span data-ttu-id="3be8e-109">Método</span><span class="sxs-lookup"><span data-stu-id="3be8e-109">Method</span></span>       | <span data-ttu-id="3be8e-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3be8e-110">Return Type</span></span>  |<span data-ttu-id="3be8e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3be8e-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3be8e-112">Lista de aplicativos</span><span class="sxs-lookup"><span data-stu-id="3be8e-112">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="3be8e-113">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="3be8e-113">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="3be8e-114">Lista os aplicativos instalados em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="3be8e-114">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="3be8e-115">Adicionar aplicativo</span><span class="sxs-lookup"><span data-stu-id="3be8e-115">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="3be8e-116">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="3be8e-116">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="3be8e-117">Adiciona (instala) um aplicativo para uma equipe.</span><span class="sxs-lookup"><span data-stu-id="3be8e-117">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="3be8e-118">Remover aplicativo</span><span class="sxs-lookup"><span data-stu-id="3be8e-118">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="3be8e-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3be8e-119">None</span></span> | <span data-ttu-id="3be8e-120">Remove (desinstala) um aplicativo da equipe.</span><span class="sxs-lookup"><span data-stu-id="3be8e-120">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="3be8e-121">Atualizar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="3be8e-121">Upgrade app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="3be8e-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3be8e-122">None</span></span> | <span data-ttu-id="3be8e-123">Atualizações para a versão mais recente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3be8e-123">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="3be8e-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3be8e-124">Properties</span></span>

| <span data-ttu-id="3be8e-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3be8e-125">Property</span></span>            | <span data-ttu-id="3be8e-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="3be8e-126">Type</span></span>     | <span data-ttu-id="3be8e-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="3be8e-127">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="3be8e-128">id</span><span class="sxs-lookup"><span data-stu-id="3be8e-128">id</span></span>                  | <span data-ttu-id="3be8e-129">string</span><span class="sxs-lookup"><span data-stu-id="3be8e-129">string</span></span>   | <span data-ttu-id="3be8e-130">Uma identificação exclusiva (não o appid equipes).</span><span class="sxs-lookup"><span data-stu-id="3be8e-130">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="3be8e-131">Relações</span><span class="sxs-lookup"><span data-stu-id="3be8e-131">Relationships</span></span>

| <span data-ttu-id="3be8e-132">Relação</span><span class="sxs-lookup"><span data-stu-id="3be8e-132">Relationship</span></span>   | <span data-ttu-id="3be8e-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="3be8e-133">Type</span></span>    | <span data-ttu-id="3be8e-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="3be8e-134">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="3be8e-135">teamsApp</span><span class="sxs-lookup"><span data-stu-id="3be8e-135">teamsApp</span></span>|[<span data-ttu-id="3be8e-136">teamsApp</span><span class="sxs-lookup"><span data-stu-id="3be8e-136">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="3be8e-137">O aplicativo que está instalado.</span><span class="sxs-lookup"><span data-stu-id="3be8e-137">The app that is installed.</span></span> |
|<span data-ttu-id="3be8e-138">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="3be8e-138">teamsAppDefinition</span></span>|[<span data-ttu-id="3be8e-139">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="3be8e-139">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="3be8e-140">Os detalhes desta versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3be8e-140">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3be8e-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3be8e-141">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
}
```

# <a name="see-also"></a><span data-ttu-id="3be8e-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="3be8e-142">See also</span></span>

- [<span data-ttu-id="3be8e-143">teamsApp</span><span class="sxs-lookup"><span data-stu-id="3be8e-143">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="3be8e-144">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="3be8e-144">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="3be8e-145">teamsTab</span><span class="sxs-lookup"><span data-stu-id="3be8e-145">teamsTab</span></span>](../resources/teamstab.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

