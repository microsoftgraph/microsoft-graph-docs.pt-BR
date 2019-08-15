---
title: Trabalhando com usuários no Microsoft Graph
description: Você pode usar o Microsoft Graph para criar experiências envolventes do aplicativo com base nos usuários, em suas relações com outros usuários e em grupos e seus emails, calendário e arquivos.
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 4d405dcc5e7881c7a404e5ca16f87c889cd5ccc7
ms.sourcegitcommit: 00959f992b9b77c98ec1fe2f185cc7fd098ab24b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36426409"
---
# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="0d291-103">Trabalhar com usuários no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0d291-103">Working with users in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d291-104">Você pode usar o Microsoft Graph para criar experiências envolventes do aplicativo com base nos usuários, em suas relações com outros usuários e em grupos e seus emails, calendário e arquivos.</span><span class="sxs-lookup"><span data-stu-id="0d291-104">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="0d291-105">Você pode acessar usuários pelo Microsoft Graph de duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="0d291-105">You can access users through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="0d291-106">Por sua ID, `/users/{id}`</span><span class="sxs-lookup"><span data-stu-id="0d291-106">By their ID, `/users/{id}`</span></span>
- <span data-ttu-id="0d291-107">Usando o alias `/me` para o usuário conectado, que é igual a `/users/{signed-in user's id}`</span><span class="sxs-lookup"><span data-stu-id="0d291-107">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="0d291-108">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d291-108">Authorization</span></span>

<span data-ttu-id="0d291-p101">Uma das seguintes [permissões](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) é necessária para acessar operações de usuário. As três primeiras permissões podem ser concedidas a um aplicativo por um usuário. O restante só pode ser concedido a um aplicativo pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="0d291-p101">One of the following [permissions](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="0d291-112">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="0d291-112">User.ReadBasic.All</span></span>
- <span data-ttu-id="0d291-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="0d291-113">User.Read</span></span>
- <span data-ttu-id="0d291-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d291-114">User.ReadWrite</span></span>
- <span data-ttu-id="0d291-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d291-115">User.Read.All</span></span>
- <span data-ttu-id="0d291-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d291-116">User.ReadWrite.All</span></span>
- <span data-ttu-id="0d291-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d291-117">Directory.Read.All</span></span>
- <span data-ttu-id="0d291-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d291-118">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="0d291-119">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0d291-119">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="0d291-120">Propriedades comuns</span><span class="sxs-lookup"><span data-stu-id="0d291-120">Common properties</span></span>

| <span data-ttu-id="0d291-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0d291-121">Property</span></span> | <span data-ttu-id="0d291-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d291-122">Description</span></span> |
|----------|-------------|
| <span data-ttu-id="0d291-123">displayName</span><span class="sxs-lookup"><span data-stu-id="0d291-123">displayName</span></span> | <span data-ttu-id="0d291-124">O nome exibido no catálogo de endereços do usuário.</span><span class="sxs-lookup"><span data-stu-id="0d291-124">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="0d291-125">givenName</span><span class="sxs-lookup"><span data-stu-id="0d291-125">givenName</span></span>| <span data-ttu-id="0d291-126">O nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="0d291-126">The first name of the user.</span></span> |
|<span data-ttu-id="0d291-127">surname</span><span class="sxs-lookup"><span data-stu-id="0d291-127">surname</span></span>| <span data-ttu-id="0d291-128">O sobrenome do usuário.</span><span class="sxs-lookup"><span data-stu-id="0d291-128">The last name of the user.</span></span> |
|<span data-ttu-id="0d291-129">email</span><span class="sxs-lookup"><span data-stu-id="0d291-129">mail</span></span>| <span data-ttu-id="0d291-130">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="0d291-130">The user's email address.</span></span> |
|<span data-ttu-id="0d291-131">photo</span><span class="sxs-lookup"><span data-stu-id="0d291-131">photo</span></span>| <span data-ttu-id="0d291-132">A foto de perfil do usuário.</span><span class="sxs-lookup"><span data-stu-id="0d291-132">The user's profile photo.</span></span> |

<span data-ttu-id="0d291-133">Para obter detalhes e uma lista de todas as propriedades, confira o objeto [user](user.md).</span><span class="sxs-lookup"><span data-stu-id="0d291-133">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="0d291-134">Operações comuns</span><span class="sxs-lookup"><span data-stu-id="0d291-134">Common operations</span></span>

><span data-ttu-id="0d291-135">**Observação:** Algumas destas operações exigem permissões adicionais.</span><span class="sxs-lookup"><span data-stu-id="0d291-135">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="0d291-136">Caminho</span><span class="sxs-lookup"><span data-stu-id="0d291-136">Path</span></span>    | <span data-ttu-id="0d291-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d291-137">Description</span></span> |
|---------|-------------|
|[`/users`](../api/user-list.md) | <span data-ttu-id="0d291-138">Lista os usuários na organização.</span><span class="sxs-lookup"><span data-stu-id="0d291-138">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user-get.md) | <span data-ttu-id="0d291-139">Obtém um usuário específico pela id.</span><span class="sxs-lookup"><span data-stu-id="0d291-139">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| <span data-ttu-id="0d291-140">Obtém a foto de perfil do usuário.</span><span class="sxs-lookup"><span data-stu-id="0d291-140">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user-list-manager.md) | <span data-ttu-id="0d291-141">Obtém o gerente do usuário.</span><span class="sxs-lookup"><span data-stu-id="0d291-141">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user-list-messages.md)| <span data-ttu-id="0d291-142">Lista as mensagens de email do usuário em sua caixa de entrada principal.</span><span class="sxs-lookup"><span data-stu-id="0d291-142">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user-list-events.md) | <span data-ttu-id="0d291-143">Lista os eventos futuros do usuário em seu calendário.</span><span class="sxs-lookup"><span data-stu-id="0d291-143">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive-get.md)| <span data-ttu-id="0d291-144">Obtém o repositório de arquivos do OneDrive do usuário.</span><span class="sxs-lookup"><span data-stu-id="0d291-144">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| <span data-ttu-id="0d291-145">Lista os grupos dos quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="0d291-145">Lists the groups that the user is a member of.</span></span> |
|[`/users/{id}/joinedTeams`](../api/user-list-joinedteams.md)| <span data-ttu-id="0d291-146">Lista as Microsoft Teams das quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="0d291-146">Lists the Microsoft Teams that the user is a member of.</span></span> |
