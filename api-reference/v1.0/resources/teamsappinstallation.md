---
title: tipo de recurso de teamsAppInstallation
description: 'Um teamsApp instalado em uma equipe. '
ms.openlocfilehash: 194a0525f46f57b9caca13f6308a31d56a84a299
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004649"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="d5020-103">tipo de recurso de teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="d5020-103">teamsAppInstallation resource type</span></span>



<span data-ttu-id="d5020-104">Um [teamsApp](teamsapp.md) instalado em uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="d5020-104">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="d5020-105">Qualquer bots que fazem parte do aplicativo se tornará parte de qualquer aplicativo é adicionado de equipe.</span><span class="sxs-lookup"><span data-stu-id="d5020-105">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="d5020-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="d5020-106">Methods</span></span>

| <span data-ttu-id="d5020-107">Método</span><span class="sxs-lookup"><span data-stu-id="d5020-107">Method</span></span>       | <span data-ttu-id="d5020-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d5020-108">Return Type</span></span>  |<span data-ttu-id="d5020-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5020-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d5020-110">Lista de aplicativos</span><span class="sxs-lookup"><span data-stu-id="d5020-110">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="d5020-111">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="d5020-111">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="d5020-112">Lista os aplicativos instalados em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="d5020-112">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="d5020-113">Adicionar aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5020-113">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="d5020-114">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="d5020-114">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="d5020-115">Adiciona (instala) um aplicativo para uma equipe.</span><span class="sxs-lookup"><span data-stu-id="d5020-115">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="d5020-116">Remover aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5020-116">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="d5020-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d5020-117">None</span></span> | <span data-ttu-id="d5020-118">Remove (desinstala) um aplicativo da equipe.</span><span class="sxs-lookup"><span data-stu-id="d5020-118">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="d5020-119">Atualizar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5020-119">Upgrade app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="d5020-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d5020-120">None</span></span> | <span data-ttu-id="d5020-121">Atualizações para a versão mais recente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d5020-121">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="d5020-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d5020-122">Properties</span></span>

| <span data-ttu-id="d5020-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5020-123">Property</span></span>            | <span data-ttu-id="d5020-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5020-124">Type</span></span>     | <span data-ttu-id="d5020-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5020-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="d5020-126">id</span><span class="sxs-lookup"><span data-stu-id="d5020-126">id</span></span>                  | <span data-ttu-id="d5020-127">string</span><span class="sxs-lookup"><span data-stu-id="d5020-127">string</span></span>   | <span data-ttu-id="d5020-128">Uma identificação exclusiva (não o appid equipes).</span><span class="sxs-lookup"><span data-stu-id="d5020-128">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="d5020-129">Relações</span><span class="sxs-lookup"><span data-stu-id="d5020-129">Relationships</span></span>

| <span data-ttu-id="d5020-130">Relação</span><span class="sxs-lookup"><span data-stu-id="d5020-130">Relationship</span></span>   | <span data-ttu-id="d5020-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5020-131">Type</span></span>    | <span data-ttu-id="d5020-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5020-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d5020-133">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d5020-133">teamsApp</span></span>|[<span data-ttu-id="d5020-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d5020-134">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="d5020-135">O aplicativo que está instalado.</span><span class="sxs-lookup"><span data-stu-id="d5020-135">The app that is installed.</span></span> |
|<span data-ttu-id="d5020-136">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="d5020-136">teamsAppDefinition</span></span>|[<span data-ttu-id="d5020-137">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="d5020-137">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="d5020-138">Os detalhes desta versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d5020-138">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d5020-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d5020-139">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="d5020-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="d5020-140">See also</span></span>

- [<span data-ttu-id="d5020-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d5020-141">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="d5020-142">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="d5020-142">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="d5020-143">teamsTab</span><span class="sxs-lookup"><span data-stu-id="d5020-143">teamsTab</span></span>](../resources/teamstab.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

