---
title: tipo de recurso userScopeTeamsAppInstallation
description: Representa um teamsApp instalado no escopo pessoal de um usuário.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 30df2c14f8723dedd25fb7c4e5b2a00481338dc3
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49606857"
---
# <a name="userscopeteamsappinstallation-resource-type"></a><span data-ttu-id="4b05c-103">tipo de recurso userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="4b05c-103">userScopeTeamsAppInstallation resource type</span></span>

<span data-ttu-id="4b05c-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="4b05c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4b05c-105">Representa um [teamsApp](teamsapp.md) instalado no escopo pessoal de um [usuário](user.md).</span><span class="sxs-lookup"><span data-stu-id="4b05c-105">Represents a [teamsApp](teamsapp.md) installed in the personal scope of a [user](user.md).</span></span> <span data-ttu-id="4b05c-106">Qualquer bots que faça parte do aplicativo se tornará parte do escopo pessoal de um usuário ao qual o aplicativo é adicionado.</span><span class="sxs-lookup"><span data-stu-id="4b05c-106">Any bots that are part of the app will become part of a user's personal scope that the app is added to.</span></span>
<span data-ttu-id="4b05c-107">Este tipo herda de [teamsAppInstallation](teamsappinstallation.md).</span><span class="sxs-lookup"><span data-stu-id="4b05c-107">This type inherits from [teamsAppInstallation](teamsappinstallation.md).</span></span>

> [!NOTE]
> <span data-ttu-id="4b05c-108">O `id` de um recurso **teamsAppInstallation** não é o mesmo valor que o `id` do recurso **teamsApp** associado.</span><span class="sxs-lookup"><span data-stu-id="4b05c-108">The `id` of a **teamsAppInstallation** resource is not the same value as the `id` of the associated **teamsApp** resource.</span></span>

## <a name="methods"></a><span data-ttu-id="4b05c-109">Methods</span><span class="sxs-lookup"><span data-stu-id="4b05c-109">Methods</span></span>

| <span data-ttu-id="4b05c-110">Método</span><span class="sxs-lookup"><span data-stu-id="4b05c-110">Method</span></span>       | <span data-ttu-id="4b05c-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4b05c-111">Return Type</span></span>  |<span data-ttu-id="4b05c-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b05c-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4b05c-113">Listar aplicativos instalados para o usuário</span><span class="sxs-lookup"><span data-stu-id="4b05c-113">List apps installed for user</span></span>](../api/userteamwork-list-installedapps.md)| <span data-ttu-id="4b05c-114">coleção [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="4b05c-114">[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) collection</span></span> | <span data-ttu-id="4b05c-115">Listar aplicativos instalados no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="4b05c-115">List apps installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="4b05c-116">Obtém o aplicativo instalado para o usuário</span><span class="sxs-lookup"><span data-stu-id="4b05c-116">Gets the installed app for user</span></span>](../api/userteamwork-get-installedapps.md)| [<span data-ttu-id="4b05c-117">userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="4b05c-117">userScopeTeamsAppInstallation</span></span>](userscopeteamsappinstallation.md) | <span data-ttu-id="4b05c-118">Lista o aplicativo especificado instalado no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="4b05c-118">List the specified app installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="4b05c-119">Adicionar aplicativo para usuário</span><span class="sxs-lookup"><span data-stu-id="4b05c-119">Add app for user</span></span>](../api/userteamwork-post-installedapps.md) | <span data-ttu-id="4b05c-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4b05c-120">None</span></span> | <span data-ttu-id="4b05c-121">Adicionar (instalar) um aplicativo no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="4b05c-121">Add (install) an app in the personal scope of a user.</span></span> |
|[<span data-ttu-id="4b05c-122">Remover o aplicativo para o usuário</span><span class="sxs-lookup"><span data-stu-id="4b05c-122">Remove app for user</span></span>](../api/userteamwork-delete-installedapps.md) | <span data-ttu-id="4b05c-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4b05c-123">None</span></span> | <span data-ttu-id="4b05c-124">Remova (desinstale) um aplicativo no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="4b05c-124">Remove (uninstall) an app in the personal scope of a user.</span></span> |
|[<span data-ttu-id="4b05c-125">Atualizar o aplicativo instalado para o usuário</span><span class="sxs-lookup"><span data-stu-id="4b05c-125">Upgrade app installed for user</span></span>](../api/userteamwork-teamsappinstallation-upgrade.md) | <span data-ttu-id="4b05c-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4b05c-126">None</span></span> | <span data-ttu-id="4b05c-127">Atualize para a versão mais recente do aplicativo instalado no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="4b05c-127">Upgrade to the latest version of the app installed in the personal scope of a user.</span></span>|
|[<span data-ttu-id="4b05c-128">Obter chat entre o usuário e o aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b05c-128">Get chat between user and app</span></span>](../api/userscopeteamsappinstallation-get-chat.md) | [<span data-ttu-id="4b05c-129">chat</span><span class="sxs-lookup"><span data-stu-id="4b05c-129">chat</span></span>](chat.md) | <span data-ttu-id="4b05c-130">Listar chats de um-on-one entre um usuário e o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4b05c-130">List one-on-one chats between a user and the app.</span></span> |

## <a name="properties"></a><span data-ttu-id="4b05c-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4b05c-131">Properties</span></span>

| <span data-ttu-id="4b05c-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b05c-132">Property</span></span>            | <span data-ttu-id="4b05c-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b05c-133">Type</span></span>     | <span data-ttu-id="4b05c-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b05c-134">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="4b05c-135">id</span><span class="sxs-lookup"><span data-stu-id="4b05c-135">id</span></span>                  | <span data-ttu-id="4b05c-136">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b05c-136">string</span></span>   | <span data-ttu-id="4b05c-137">Uma ID exclusiva (não a ID do aplicativo Teams).</span><span class="sxs-lookup"><span data-stu-id="4b05c-137">A unique ID (not the Teams app ID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="4b05c-138">Relações</span><span class="sxs-lookup"><span data-stu-id="4b05c-138">Relationships</span></span>

| <span data-ttu-id="4b05c-139">Relação</span><span class="sxs-lookup"><span data-stu-id="4b05c-139">Relationship</span></span>   | <span data-ttu-id="4b05c-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b05c-140">Type</span></span>    | <span data-ttu-id="4b05c-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b05c-141">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="4b05c-142">teamsApp</span><span class="sxs-lookup"><span data-stu-id="4b05c-142">teamsApp</span></span>|[<span data-ttu-id="4b05c-143">teamsApp</span><span class="sxs-lookup"><span data-stu-id="4b05c-143">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="4b05c-144">O aplicativo que está instalado.</span><span class="sxs-lookup"><span data-stu-id="4b05c-144">The app that is installed.</span></span> |
|<span data-ttu-id="4b05c-145">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="4b05c-145">teamsAppDefinition</span></span>|[<span data-ttu-id="4b05c-146">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="4b05c-146">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="4b05c-147">Os detalhes desta versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4b05c-147">The details of this version of the app.</span></span> |
|<span data-ttu-id="4b05c-148">chat</span><span class="sxs-lookup"><span data-stu-id="4b05c-148">chat</span></span> |[<span data-ttu-id="4b05c-149">chat</span><span class="sxs-lookup"><span data-stu-id="4b05c-149">chat</span></span>](chat.md) | <span data-ttu-id="4b05c-150">O chat entre o usuário e o aplicativo do teams.</span><span class="sxs-lookup"><span data-stu-id="4b05c-150">The chat between the user and Teams app.</span></span> | 

## <a name="json-representation"></a><span data-ttu-id="4b05c-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4b05c-151">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="4b05c-152">Confira também</span><span class="sxs-lookup"><span data-stu-id="4b05c-152">See also</span></span>

- [<span data-ttu-id="4b05c-153">teamsApp</span><span class="sxs-lookup"><span data-stu-id="4b05c-153">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="4b05c-154">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="4b05c-154">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="4b05c-155">teamsTab</span><span class="sxs-lookup"><span data-stu-id="4b05c-155">teamsTab</span></span>](../resources/teamstab.md)

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

