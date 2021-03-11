---
title: Trabalhar com usuários no Microsoft Graph
description: Crie experiências atraentes para aplicativos baseadas nos usuários, suas relações com outros usuários e grupos, seus emails, calendários e arquivos.
localization_priority: Priority
author: jpettere
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: c18731042d9d86479c5658f0a0f38a38d23bdb0d
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719819"
---
# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="3f117-103">Trabalhar com usuários no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3f117-103">Working with users in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f117-104">Você pode usar o Microsoft Graph para criar experiências envolventes do aplicativo com base nos usuários, em suas relações com outros usuários e em grupos e seus emails, calendário e arquivos.</span><span class="sxs-lookup"><span data-stu-id="3f117-104">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="3f117-105">Você pode acessar usuários pelo Microsoft Graph de duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="3f117-105">You can access users through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="3f117-106">Por sua ID, `/users/{id}`</span><span class="sxs-lookup"><span data-stu-id="3f117-106">By their ID, `/users/{id}`</span></span>
- <span data-ttu-id="3f117-107">Usando o alias `/me` para o usuário conectado, que é igual a `/users/{signed-in user's id}`</span><span class="sxs-lookup"><span data-stu-id="3f117-107">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="3f117-108">Autorização</span><span class="sxs-lookup"><span data-stu-id="3f117-108">Authorization</span></span>

<span data-ttu-id="3f117-p101">Uma das seguintes [permissões](/graph/permissions-reference) é necessária para acessar operações de usuário. As três primeiras permissões podem ser concedidas a um aplicativo por um usuário. O restante só pode ser concedido a um aplicativo pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="3f117-p101">One of the following [permissions](/graph/permissions-reference) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="3f117-112">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="3f117-112">User.ReadBasic.All</span></span>
- <span data-ttu-id="3f117-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="3f117-113">User.Read</span></span>
- <span data-ttu-id="3f117-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f117-114">User.ReadWrite</span></span>
- <span data-ttu-id="3f117-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f117-115">User.Read.All</span></span>
- <span data-ttu-id="3f117-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f117-116">User.ReadWrite.All</span></span>
- <span data-ttu-id="3f117-117">User.ManageIdentities.All</span><span class="sxs-lookup"><span data-stu-id="3f117-117">User.ManageIdentities.All</span></span>
- <span data-ttu-id="3f117-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f117-118">Directory.Read.All</span></span>
- <span data-ttu-id="3f117-119">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f117-119">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="3f117-120">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3f117-120">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="3f117-121">Propriedades comuns</span><span class="sxs-lookup"><span data-stu-id="3f117-121">Common properties</span></span>

| <span data-ttu-id="3f117-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3f117-122">Property</span></span> | <span data-ttu-id="3f117-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f117-123">Description</span></span> |
|----------|-------------|
| <span data-ttu-id="3f117-124">displayName</span><span class="sxs-lookup"><span data-stu-id="3f117-124">displayName</span></span> | <span data-ttu-id="3f117-125">O nome exibido no catálogo de endereços do usuário.</span><span class="sxs-lookup"><span data-stu-id="3f117-125">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="3f117-126">givenName</span><span class="sxs-lookup"><span data-stu-id="3f117-126">givenName</span></span>| <span data-ttu-id="3f117-127">O nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="3f117-127">The first name of the user.</span></span> |
|<span data-ttu-id="3f117-128">surname</span><span class="sxs-lookup"><span data-stu-id="3f117-128">surname</span></span>| <span data-ttu-id="3f117-129">O sobrenome do usuário.</span><span class="sxs-lookup"><span data-stu-id="3f117-129">The last name of the user.</span></span> |
|<span data-ttu-id="3f117-130">email</span><span class="sxs-lookup"><span data-stu-id="3f117-130">mail</span></span>| <span data-ttu-id="3f117-131">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="3f117-131">The user's email address.</span></span> |
|<span data-ttu-id="3f117-132">photo</span><span class="sxs-lookup"><span data-stu-id="3f117-132">photo</span></span>| <span data-ttu-id="3f117-133">A foto de perfil do usuário.</span><span class="sxs-lookup"><span data-stu-id="3f117-133">The user's profile photo.</span></span> |

<span data-ttu-id="3f117-134">Para obter detalhes e uma lista de todas as propriedades, confira o objeto [user](user.md).</span><span class="sxs-lookup"><span data-stu-id="3f117-134">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="3f117-135">Operações comuns</span><span class="sxs-lookup"><span data-stu-id="3f117-135">Common operations</span></span>

><span data-ttu-id="3f117-136">**Observação:** Algumas destas operações exigem permissões adicionais.</span><span class="sxs-lookup"><span data-stu-id="3f117-136">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="3f117-137">Caminho</span><span class="sxs-lookup"><span data-stu-id="3f117-137">Path</span></span>    | <span data-ttu-id="3f117-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f117-138">Description</span></span> |
|---------|-------------|
|[`/users`](../api/user-list.md) | <span data-ttu-id="3f117-139">Lista os usuários na organização.</span><span class="sxs-lookup"><span data-stu-id="3f117-139">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user-get.md) | <span data-ttu-id="3f117-140">Obtém um usuário específico pela id.</span><span class="sxs-lookup"><span data-stu-id="3f117-140">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| <span data-ttu-id="3f117-141">Obtém a foto de perfil do usuário.</span><span class="sxs-lookup"><span data-stu-id="3f117-141">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user-list-manager.md) | <span data-ttu-id="3f117-142">Obtém o gerente do usuário.</span><span class="sxs-lookup"><span data-stu-id="3f117-142">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user-list-messages.md)| <span data-ttu-id="3f117-143">Lista as mensagens de email do usuário em sua caixa de entrada principal.</span><span class="sxs-lookup"><span data-stu-id="3f117-143">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user-list-events.md) | <span data-ttu-id="3f117-144">Lista os eventos futuros do usuário em seu calendário.</span><span class="sxs-lookup"><span data-stu-id="3f117-144">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive-get.md)| <span data-ttu-id="3f117-145">Obtém o repositório de arquivos do OneDrive do usuário.</span><span class="sxs-lookup"><span data-stu-id="3f117-145">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| <span data-ttu-id="3f117-146">Lista os grupos dos quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="3f117-146">Lists the groups that the user is a member of.</span></span> |
|[`/users/{id}/joinedTeams`](../api/user-list-joinedteams.md)| <span data-ttu-id="3f117-147">Lista as Microsoft Teams das quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="3f117-147">Lists the Microsoft Teams that the user is a member of.</span></span> |

## <a name="whats-new"></a><span data-ttu-id="3f117-148">Novidades</span><span class="sxs-lookup"><span data-stu-id="3f117-148">What's new</span></span>
<span data-ttu-id="3f117-149">Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.</span><span class="sxs-lookup"><span data-stu-id="3f117-149">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>