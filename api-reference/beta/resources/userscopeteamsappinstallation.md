---
title: tipo de recurso userScopeTeamsAppInstallation
description: Representa um teamsApp instalado no escopo pessoal de um usuário.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 19ca16e4d6a3171cc622440ee79dce3d93e8dd84
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49564163"
---
# <a name="userscopeteamsappinstallation-resource-type"></a><span data-ttu-id="7ee66-103">tipo de recurso userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="7ee66-103">userScopeTeamsAppInstallation resource type</span></span>

<span data-ttu-id="7ee66-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ee66-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ee66-105">Representa um [teamsApp](teamsapp.md) instalado no escopo pessoal de um [usuário](user.md).</span><span class="sxs-lookup"><span data-stu-id="7ee66-105">Represents a [teamsApp](teamsapp.md) installed in the personal scope of a [user](user.md).</span></span> <span data-ttu-id="7ee66-106">Qualquer bots que faça parte do aplicativo se tornará parte do escopo pessoal de um usuário ao qual o aplicativo é adicionado.</span><span class="sxs-lookup"><span data-stu-id="7ee66-106">Any bots that are part of the app will become part of a user's personal scope that the app is added to.</span></span>
<span data-ttu-id="7ee66-107">Este tipo herda de [teamsAppInstallation](teamsappinstallation.md).</span><span class="sxs-lookup"><span data-stu-id="7ee66-107">This type inherits from [teamsAppInstallation](teamsappinstallation.md).</span></span>

## <a name="methods"></a><span data-ttu-id="7ee66-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="7ee66-108">Methods</span></span>

| <span data-ttu-id="7ee66-109">Método</span><span class="sxs-lookup"><span data-stu-id="7ee66-109">Method</span></span>       | <span data-ttu-id="7ee66-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7ee66-110">Return Type</span></span>  |<span data-ttu-id="7ee66-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ee66-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7ee66-112">Listar aplicativos instalados para o usuário</span><span class="sxs-lookup"><span data-stu-id="7ee66-112">List apps installed for user</span></span>](../api/userteamwork-list-installedapps.md)| <span data-ttu-id="7ee66-113">coleção [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="7ee66-113">[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) collection</span></span> | <span data-ttu-id="7ee66-114">Listar aplicativos instalados no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="7ee66-114">List apps installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="7ee66-115">Obter o aplicativo instalado para o usuário</span><span class="sxs-lookup"><span data-stu-id="7ee66-115">Get the installed app for user</span></span>](../api/userteamwork-get-installedapps.md)| [<span data-ttu-id="7ee66-116">userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="7ee66-116">userScopeTeamsAppInstallation</span></span>](userscopeteamsappinstallation.md) | <span data-ttu-id="7ee66-117">Lista o aplicativo especificado instalado no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="7ee66-117">List the specified app installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="7ee66-118">Adicionar aplicativo para usuário</span><span class="sxs-lookup"><span data-stu-id="7ee66-118">Add app for user</span></span>](../api/userteamwork-add-installedapps.md) | <span data-ttu-id="7ee66-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7ee66-119">None</span></span> | <span data-ttu-id="7ee66-120">Adiciona (instala) um aplicativo no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="7ee66-120">Adds (installs) an app in the personal scope of a user.</span></span> |
|[<span data-ttu-id="7ee66-121">Remover o aplicativo para o usuário</span><span class="sxs-lookup"><span data-stu-id="7ee66-121">Remove app for user</span></span>](../api/userteamwork-delete-installedapps.md) | <span data-ttu-id="7ee66-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7ee66-122">None</span></span> | <span data-ttu-id="7ee66-123">Remove (desinstala) um aplicativo no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="7ee66-123">Removes (uninstalls) an app in the personal scope of a user.</span></span> |
|[<span data-ttu-id="7ee66-124">Atualizar o aplicativo instalado para o usuário</span><span class="sxs-lookup"><span data-stu-id="7ee66-124">Upgrade app installed for user</span></span>](../api/userteamwork-upgrade-installedapps.md) | <span data-ttu-id="7ee66-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7ee66-125">None</span></span> | <span data-ttu-id="7ee66-126">Atualiza para a versão mais recente do aplicativo instalado no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="7ee66-126">Upgrades to the latest version of the app installed in the personal scope of a user.</span></span>|
|[<span data-ttu-id="7ee66-127">Obter chat entre o usuário e o aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ee66-127">Get chat between user and app</span></span>](../api/userscopeteamsappinstallation-get-chat.md) | [<span data-ttu-id="7ee66-128">chat</span><span class="sxs-lookup"><span data-stu-id="7ee66-128">chat</span></span>](chat.md) | <span data-ttu-id="7ee66-129">Lista o chat de um em um entre o usuário e o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ee66-129">Lists one-on-one chat between the user and the app.</span></span> |

## <a name="properties"></a><span data-ttu-id="7ee66-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7ee66-130">Properties</span></span>

| <span data-ttu-id="7ee66-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ee66-131">Property</span></span>            | <span data-ttu-id="7ee66-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ee66-132">Type</span></span>     | <span data-ttu-id="7ee66-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ee66-133">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="7ee66-134">id</span><span class="sxs-lookup"><span data-stu-id="7ee66-134">id</span></span>                  | <span data-ttu-id="7ee66-135">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ee66-135">string</span></span>   | <span data-ttu-id="7ee66-136">Uma ID exclusiva (não a ID do aplicativo Teams).</span><span class="sxs-lookup"><span data-stu-id="7ee66-136">A unique ID (not the Teams app ID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="7ee66-137">Relações</span><span class="sxs-lookup"><span data-stu-id="7ee66-137">Relationships</span></span>

| <span data-ttu-id="7ee66-138">Relação</span><span class="sxs-lookup"><span data-stu-id="7ee66-138">Relationship</span></span>   | <span data-ttu-id="7ee66-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ee66-139">Type</span></span>    | <span data-ttu-id="7ee66-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ee66-140">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="7ee66-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="7ee66-141">teamsApp</span></span>|[<span data-ttu-id="7ee66-142">teamsApp</span><span class="sxs-lookup"><span data-stu-id="7ee66-142">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="7ee66-143">O aplicativo que está instalado.</span><span class="sxs-lookup"><span data-stu-id="7ee66-143">The app that is installed.</span></span> |
|<span data-ttu-id="7ee66-144">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="7ee66-144">teamsAppDefinition</span></span>|[<span data-ttu-id="7ee66-145">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="7ee66-145">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="7ee66-146">Os detalhes desta versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ee66-146">The details of this version of the app.</span></span> |
|<span data-ttu-id="7ee66-147">chat</span><span class="sxs-lookup"><span data-stu-id="7ee66-147">chat</span></span> |[<span data-ttu-id="7ee66-148">chat</span><span class="sxs-lookup"><span data-stu-id="7ee66-148">chat</span></span>](chat.md) | <span data-ttu-id="7ee66-149">O chat entre o usuário e o aplicativo do teams.</span><span class="sxs-lookup"><span data-stu-id="7ee66-149">The chat between the user and Teams app.</span></span> | 

## <a name="json-representation"></a><span data-ttu-id="7ee66-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7ee66-150">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userScopeTeamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}
```

## <a name="see-also"></a><span data-ttu-id="7ee66-151">Confira também</span><span class="sxs-lookup"><span data-stu-id="7ee66-151">See also</span></span>

- [<span data-ttu-id="7ee66-152">teamsApp</span><span class="sxs-lookup"><span data-stu-id="7ee66-152">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="7ee66-153">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="7ee66-153">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="7ee66-154">teamsTab</span><span class="sxs-lookup"><span data-stu-id="7ee66-154">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userScopeTeamsAppInstallation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
  "suppressions": []
}-->

