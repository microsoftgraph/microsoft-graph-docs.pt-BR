---
title: Trabalhando com usuários no Microsoft Graph
description: Você pode usar o Microsoft Graph para criar experiências envolventes do aplicativo com base nos usuários, em suas relações com outros usuários e em grupos e seus emails, calendário e arquivos.
ms.openlocfilehash: ee084bb52042b0c42f0308584ec6b3989b5b6114
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036684"
---
# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="48bf8-103">Trabalhando com usuários no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="48bf8-103">Working with users in Microsoft Graph</span></span>

> <span data-ttu-id="48bf8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="48bf8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="48bf8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="48bf8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="48bf8-106">Você pode usar o Microsoft Graph para criar experiências envolventes do aplicativo com base nos usuários, em suas relações com outros usuários e em grupos e seus emails, calendário e arquivos.</span><span class="sxs-lookup"><span data-stu-id="48bf8-106">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="48bf8-107">Você pode acessar usuários pelo Microsoft Graph de duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="48bf8-107">You can access users through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="48bf8-108">Por sua ID, `/users/{id}`</span><span class="sxs-lookup"><span data-stu-id="48bf8-108">By their ID, `/users/{id}`</span></span> 
- <span data-ttu-id="48bf8-109">Usando o alias `/me` para o usuário conectado, que é igual a `/users/{signed-in user's id}`</span><span class="sxs-lookup"><span data-stu-id="48bf8-109">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="48bf8-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="48bf8-110">Authorization</span></span>
<span data-ttu-id="48bf8-p102">Uma das seguintes [permissões](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) é necessária para acessar operações de usuário. As três primeiras permissões podem ser concedidas a um aplicativo por um usuário. O restante só pode ser concedido a um aplicativo pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="48bf8-p102">One of the following [permissions](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="48bf8-114">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="48bf8-114">User.ReadBasic.All</span></span>
- <span data-ttu-id="48bf8-115">User.Read</span><span class="sxs-lookup"><span data-stu-id="48bf8-115">User.Read</span></span>
- <span data-ttu-id="48bf8-116">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48bf8-116">User.ReadWrite</span></span>
- <span data-ttu-id="48bf8-117">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="48bf8-117">User.Read.All</span></span>
- <span data-ttu-id="48bf8-118">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48bf8-118">User.ReadWrite.All</span></span>
- <span data-ttu-id="48bf8-119">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="48bf8-119">Directory.Read.All</span></span>
- <span data-ttu-id="48bf8-120">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48bf8-120">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="48bf8-121">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="48bf8-121">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="48bf8-122">Propriedades comuns</span><span class="sxs-lookup"><span data-stu-id="48bf8-122">Common properties</span></span>

| <span data-ttu-id="48bf8-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48bf8-123">Property</span></span> | <span data-ttu-id="48bf8-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="48bf8-124">Description</span></span> |
|----------|-------------|
| <span data-ttu-id="48bf8-125">displayName</span><span class="sxs-lookup"><span data-stu-id="48bf8-125">displayName</span></span> | <span data-ttu-id="48bf8-126">O nome exibido no catálogo de endereços do usuário.</span><span class="sxs-lookup"><span data-stu-id="48bf8-126">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="48bf8-127">givenName</span><span class="sxs-lookup"><span data-stu-id="48bf8-127">givenName</span></span>| <span data-ttu-id="48bf8-128">O nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="48bf8-128">The first name of the user.</span></span> |
|<span data-ttu-id="48bf8-129">surname</span><span class="sxs-lookup"><span data-stu-id="48bf8-129">surname</span></span>| <span data-ttu-id="48bf8-130">O sobrenome do usuário.</span><span class="sxs-lookup"><span data-stu-id="48bf8-130">The last name of the user.</span></span> |
|<span data-ttu-id="48bf8-131">email</span><span class="sxs-lookup"><span data-stu-id="48bf8-131">mail</span></span>| <span data-ttu-id="48bf8-132">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="48bf8-132">The user's email address.</span></span> |
|<span data-ttu-id="48bf8-133">Foto</span><span class="sxs-lookup"><span data-stu-id="48bf8-133">photo</span></span>| <span data-ttu-id="48bf8-134">Foto de perfil do usuário.</span><span class="sxs-lookup"><span data-stu-id="48bf8-134">The user's profile photo.</span></span> |

<span data-ttu-id="48bf8-135">Para obter detalhes e uma lista de todas as propriedades, confira o objeto [user](user.md).</span><span class="sxs-lookup"><span data-stu-id="48bf8-135">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="48bf8-136">Operações comuns</span><span class="sxs-lookup"><span data-stu-id="48bf8-136">Common operations</span></span>
><span data-ttu-id="48bf8-137">**Observação:** Algumas destas operações exigem permissões adicionais.</span><span class="sxs-lookup"><span data-stu-id="48bf8-137">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="48bf8-138">Path</span><span class="sxs-lookup"><span data-stu-id="48bf8-138">Path</span></span>    | <span data-ttu-id="48bf8-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="48bf8-139">Description</span></span> |
|---------|-------------|
|[`/users`](../api/user-list.md) | <span data-ttu-id="48bf8-140">Lista os usuários na organização.</span><span class="sxs-lookup"><span data-stu-id="48bf8-140">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user-get.md) | <span data-ttu-id="48bf8-141">Obtém um usuário específico pela id.</span><span class="sxs-lookup"><span data-stu-id="48bf8-141">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| <span data-ttu-id="48bf8-142">Obtém a foto de perfil do usuário.</span><span class="sxs-lookup"><span data-stu-id="48bf8-142">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user-list-manager.md) | <span data-ttu-id="48bf8-143">Obtém o gerente do usuário.</span><span class="sxs-lookup"><span data-stu-id="48bf8-143">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user-list-messages.md)| <span data-ttu-id="48bf8-144">Lista as mensagens de email do usuário em sua caixa de entrada principal.</span><span class="sxs-lookup"><span data-stu-id="48bf8-144">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user-list-events.md) | <span data-ttu-id="48bf8-145">Lista os eventos futuros do usuário em seu calendário.</span><span class="sxs-lookup"><span data-stu-id="48bf8-145">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive-get.md)| <span data-ttu-id="48bf8-146">Obtém o repositório de arquivos do OneDrive do usuário.</span><span class="sxs-lookup"><span data-stu-id="48bf8-146">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| <span data-ttu-id="48bf8-147">Lista os grupos dos quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="48bf8-147">Lists the groups that the user is a member of.</span></span> |
|[`/users/{id}/joinedTeams`](../api/user-list-joinedteams.md)| <span data-ttu-id="48bf8-148">Lista Teams Microsoft que o usuário é membro de.</span><span class="sxs-lookup"><span data-stu-id="48bf8-148">Lists the Microsoft Teams that the user is a member of.</span></span> |
