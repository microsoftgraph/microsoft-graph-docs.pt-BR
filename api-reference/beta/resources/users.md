---
title: Trabalhando com usuários no Microsoft Graph
description: Você pode usar o Microsoft Graph para criar experiências envolventes do aplicativo com base nos usuários, em suas relações com outros usuários e em grupos e seus emails, calendário e arquivos.
ms.openlocfilehash: 0bc1e0b045703c73a22568912db978d50c5a0c15
ms.sourcegitcommit: f3d479edf03935d0edbbc7668a65f7cde2a56c92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2018
ms.locfileid: "27283644"
---
# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="7b8fc-103">Trabalhando com usuários no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7b8fc-103">Working with users in Microsoft Graph</span></span>

> <span data-ttu-id="7b8fc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7b8fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b8fc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7b8fc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7b8fc-106">Você pode usar o Microsoft Graph para criar experiências envolventes do aplicativo com base nos usuários, em suas relações com outros usuários e em grupos e seus emails, calendário e arquivos.</span><span class="sxs-lookup"><span data-stu-id="7b8fc-106">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="7b8fc-107">Você pode acessar usuários pelo Microsoft Graph de duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="7b8fc-107">You can access users through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="7b8fc-108">Por sua ID, `/users/{id}`</span><span class="sxs-lookup"><span data-stu-id="7b8fc-108">By their ID, `/users/{id}`</span></span> 
- <span data-ttu-id="7b8fc-109">Usando o alias `/me` para o usuário conectado, que é igual a `/users/{signed-in user's id}`</span><span class="sxs-lookup"><span data-stu-id="7b8fc-109">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="7b8fc-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="7b8fc-110">Authorization</span></span>
<span data-ttu-id="7b8fc-p102">Uma das seguintes [permissões](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) é necessária para acessar operações de usuário. As três primeiras permissões podem ser concedidas a um aplicativo por um usuário. O restante só pode ser concedido a um aplicativo pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="7b8fc-p102">One of the following [permissions](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="7b8fc-114">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="7b8fc-114">User.ReadBasic.All</span></span>
- <span data-ttu-id="7b8fc-115">User.Read</span><span class="sxs-lookup"><span data-stu-id="7b8fc-115">User.Read</span></span>
- <span data-ttu-id="7b8fc-116">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7b8fc-116">User.ReadWrite</span></span>
- <span data-ttu-id="7b8fc-117">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b8fc-117">User.Read.All</span></span>
- <span data-ttu-id="7b8fc-118">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b8fc-118">User.ReadWrite.All</span></span>
- <span data-ttu-id="7b8fc-119">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b8fc-119">Directory.Read.All</span></span>
- <span data-ttu-id="7b8fc-120">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b8fc-120">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="7b8fc-121">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7b8fc-121">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="7b8fc-122">Propriedades comuns</span><span class="sxs-lookup"><span data-stu-id="7b8fc-122">Common properties</span></span>

| <span data-ttu-id="7b8fc-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b8fc-123">Property</span></span> | <span data-ttu-id="7b8fc-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b8fc-124">Description</span></span> |
|----------|-------------|
| <span data-ttu-id="7b8fc-125">displayName</span><span class="sxs-lookup"><span data-stu-id="7b8fc-125">displayName</span></span> | <span data-ttu-id="7b8fc-126">O nome exibido no catálogo de endereços do usuário.</span><span class="sxs-lookup"><span data-stu-id="7b8fc-126">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="7b8fc-127">givenName</span><span class="sxs-lookup"><span data-stu-id="7b8fc-127">givenName</span></span>| <span data-ttu-id="7b8fc-128">O nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="7b8fc-128">The first name of the user.</span></span> |
|<span data-ttu-id="7b8fc-129">surname</span><span class="sxs-lookup"><span data-stu-id="7b8fc-129">surname</span></span>| <span data-ttu-id="7b8fc-130">O sobrenome do usuário.</span><span class="sxs-lookup"><span data-stu-id="7b8fc-130">The last name of the user.</span></span> |
|<span data-ttu-id="7b8fc-131">email</span><span class="sxs-lookup"><span data-stu-id="7b8fc-131">mail</span></span>| <span data-ttu-id="7b8fc-132">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="7b8fc-132">The user's email address.</span></span> |
|<span data-ttu-id="7b8fc-133">Foto</span><span class="sxs-lookup"><span data-stu-id="7b8fc-133">photo</span></span>| <span data-ttu-id="7b8fc-134">Foto de perfil do usuário.</span><span class="sxs-lookup"><span data-stu-id="7b8fc-134">The user's profile photo.</span></span> |

<span data-ttu-id="7b8fc-135">Para obter detalhes e uma lista de todas as propriedades, confira o objeto [user](user.md).</span><span class="sxs-lookup"><span data-stu-id="7b8fc-135">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="7b8fc-136">Operações comuns</span><span class="sxs-lookup"><span data-stu-id="7b8fc-136">Common operations</span></span>
><span data-ttu-id="7b8fc-137">**Observação:** Algumas destas operações exigem permissões adicionais.</span><span class="sxs-lookup"><span data-stu-id="7b8fc-137">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="7b8fc-138">Path</span><span class="sxs-lookup"><span data-stu-id="7b8fc-138">Path</span></span>    | <span data-ttu-id="7b8fc-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b8fc-139">Description</span></span> |
|---------|-------------|
|[`/users`](../api/user-list.md) | <span data-ttu-id="7b8fc-140">Lista os usuários na organização.</span><span class="sxs-lookup"><span data-stu-id="7b8fc-140">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user-get.md) | <span data-ttu-id="7b8fc-141">Obtém um usuário específico pela id.</span><span class="sxs-lookup"><span data-stu-id="7b8fc-141">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| <span data-ttu-id="7b8fc-142">Obtém a foto de perfil do usuário.</span><span class="sxs-lookup"><span data-stu-id="7b8fc-142">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user-list-manager.md) | <span data-ttu-id="7b8fc-143">Obtém o gerente do usuário.</span><span class="sxs-lookup"><span data-stu-id="7b8fc-143">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user-list-messages.md)| <span data-ttu-id="7b8fc-144">Lista as mensagens de email do usuário em sua caixa de entrada principal.</span><span class="sxs-lookup"><span data-stu-id="7b8fc-144">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user-list-events.md) | <span data-ttu-id="7b8fc-145">Lista os eventos futuros do usuário em seu calendário.</span><span class="sxs-lookup"><span data-stu-id="7b8fc-145">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive-get.md)| <span data-ttu-id="7b8fc-146">Obtém o repositório de arquivos do OneDrive do usuário.</span><span class="sxs-lookup"><span data-stu-id="7b8fc-146">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| <span data-ttu-id="7b8fc-147">Lista os grupos dos quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="7b8fc-147">Lists the groups that the user is a member of.</span></span> |
|[`/users/{id}/joinedTeams`](../api/user-list-joinedteams.md)| <span data-ttu-id="7b8fc-148">Lista Teams Microsoft que o usuário é membro de.</span><span class="sxs-lookup"><span data-stu-id="7b8fc-148">Lists the Microsoft Teams that the user is a member of.</span></span> |