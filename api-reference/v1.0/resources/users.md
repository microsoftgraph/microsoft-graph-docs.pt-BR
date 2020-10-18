---
title: Trabalhar com usuários no Microsoft Graph
description: Crie experiências atraentes para aplicativos baseadas nos usuários, suas relações com outros usuários e grupos, seus emails, calendários e arquivos.
localization_priority: Priority
author: krbain
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 082efd396a1d26d8054339c82840dfb1fbea52a5
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/17/2020
ms.locfileid: "48582195"
---
# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="23a5b-103">Trabalhar com usuários no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="23a5b-103">Working with users in Microsoft Graph</span></span>

<span data-ttu-id="23a5b-104">Você pode usar o Microsoft Graph para criar experiências envolventes do aplicativo com base nos usuários, em suas relações com outros usuários e em grupos e seus emails, calendário e arquivos.</span><span class="sxs-lookup"><span data-stu-id="23a5b-104">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="23a5b-105">Você pode acessar [usuários](user.md) pelo Microsoft Graph de duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="23a5b-105">You can access [users](user.md) through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="23a5b-106">Por sua ID, `/users/{id | userPrincipalName}`</span><span class="sxs-lookup"><span data-stu-id="23a5b-106">By their ID, `/users/{id | userPrincipalName}`</span></span>
- <span data-ttu-id="23a5b-107">Usando o alias `/me` para o usuário conectado, que é igual a `/users/{signed-in user's id}`</span><span class="sxs-lookup"><span data-stu-id="23a5b-107">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="23a5b-108">Autorização</span><span class="sxs-lookup"><span data-stu-id="23a5b-108">Authorization</span></span>

<span data-ttu-id="23a5b-p101">Uma das seguintes [permissões](/graph/permissions-reference) é necessária para acessar operações de usuário. As três primeiras permissões podem ser concedidas a um aplicativo por um usuário. O restante só pode ser concedido a um aplicativo pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="23a5b-p101">One of the following [permissions](/graph/permissions-reference) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="23a5b-112">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="23a5b-112">User.ReadBasic.All</span></span>
- <span data-ttu-id="23a5b-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="23a5b-113">User.Read</span></span>
- <span data-ttu-id="23a5b-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23a5b-114">User.ReadWrite</span></span>
- <span data-ttu-id="23a5b-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="23a5b-115">User.Read.All</span></span>
- <span data-ttu-id="23a5b-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23a5b-116">User.ReadWrite.All</span></span>
- <span data-ttu-id="23a5b-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="23a5b-117">Directory.Read.All</span></span>
- <span data-ttu-id="23a5b-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23a5b-118">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="23a5b-119">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="23a5b-119">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="23a5b-120">Propriedades comuns</span><span class="sxs-lookup"><span data-stu-id="23a5b-120">Common properties</span></span>

<span data-ttu-id="23a5b-121">O item a seguir representa o conjunto padrão de propriedades que serão retornadas ao se obter um usuário ou listar usuários.</span><span class="sxs-lookup"><span data-stu-id="23a5b-121">The following represent the default set of properties that are returned when getting a user or listing users.</span></span> <span data-ttu-id="23a5b-122">Este é um subconjunto de todas as propriedades disponíveis.</span><span class="sxs-lookup"><span data-stu-id="23a5b-122">These are a subset of all available properties.</span></span> <span data-ttu-id="23a5b-123">Para obter mais propriedades do usuário, use o parâmetro de consulta `$select`.</span><span class="sxs-lookup"><span data-stu-id="23a5b-123">To get more user properties, use the `$select` query parameter.</span></span>

|<span data-ttu-id="23a5b-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23a5b-124">Property</span></span> |<span data-ttu-id="23a5b-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="23a5b-125">Description</span></span> |
|:----------|:-------------|
|<span data-ttu-id="23a5b-126">id</span><span class="sxs-lookup"><span data-stu-id="23a5b-126">id</span></span> | <span data-ttu-id="23a5b-127">O identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="23a5b-127">The unique identifier for the user.</span></span>|
|<span data-ttu-id="23a5b-128">businessPhones</span><span class="sxs-lookup"><span data-stu-id="23a5b-128">businessPhones</span></span> | <span data-ttu-id="23a5b-129">Os números de telefone do usuário.</span><span class="sxs-lookup"><span data-stu-id="23a5b-129">The user's phone numbers.</span></span>|
|<span data-ttu-id="23a5b-130">displayName</span><span class="sxs-lookup"><span data-stu-id="23a5b-130">displayName</span></span> | <span data-ttu-id="23a5b-131">O nome exibido no catálogo de endereços do usuário.</span><span class="sxs-lookup"><span data-stu-id="23a5b-131">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="23a5b-132">givenName</span><span class="sxs-lookup"><span data-stu-id="23a5b-132">givenName</span></span>| <span data-ttu-id="23a5b-133">O nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="23a5b-133">The first name of the user.</span></span> |
|<span data-ttu-id="23a5b-134">jobTitle</span><span class="sxs-lookup"><span data-stu-id="23a5b-134">jobTitle</span></span> | <span data-ttu-id="23a5b-135">O cargo do usuário.</span><span class="sxs-lookup"><span data-stu-id="23a5b-135">The user's job title.</span></span>|
|<span data-ttu-id="23a5b-136">email</span><span class="sxs-lookup"><span data-stu-id="23a5b-136">mail</span></span>| <span data-ttu-id="23a5b-137">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="23a5b-137">The user's email address.</span></span> |
|<span data-ttu-id="23a5b-138">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="23a5b-138">mobilePhone</span></span> | <span data-ttu-id="23a5b-139">O número de telefone celular do usuário.</span><span class="sxs-lookup"><span data-stu-id="23a5b-139">The user's cellphone number.</span></span>|
|<span data-ttu-id="23a5b-140">officeLocation</span><span class="sxs-lookup"><span data-stu-id="23a5b-140">officeLocation</span></span> | <span data-ttu-id="23a5b-141">O local do escritório físico do usuário.</span><span class="sxs-lookup"><span data-stu-id="23a5b-141">The user's physical office location.</span></span>|
|<span data-ttu-id="23a5b-142">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="23a5b-142">preferredLanguage</span></span> | <span data-ttu-id="23a5b-143">O idioma preferencial do usuário.</span><span class="sxs-lookup"><span data-stu-id="23a5b-143">The user's language of preference.</span></span>|
|<span data-ttu-id="23a5b-144">surname</span><span class="sxs-lookup"><span data-stu-id="23a5b-144">surname</span></span>| <span data-ttu-id="23a5b-145">O sobrenome do usuário.</span><span class="sxs-lookup"><span data-stu-id="23a5b-145">The last name of the user.</span></span> |
|<span data-ttu-id="23a5b-146">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="23a5b-146">userPrincipalName</span></span>| <span data-ttu-id="23a5b-147">O nome UPN do usuário.</span><span class="sxs-lookup"><span data-stu-id="23a5b-147">The user's principal name.</span></span> |

<span data-ttu-id="23a5b-148">Para obter detalhes e uma lista de todas as propriedades, confira o objeto [user](user.md).</span><span class="sxs-lookup"><span data-stu-id="23a5b-148">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="23a5b-149">Operações comuns</span><span class="sxs-lookup"><span data-stu-id="23a5b-149">Common operations</span></span>

> <span data-ttu-id="23a5b-150">**Observação:** Algumas destas operações exigem permissões adicionais.</span><span class="sxs-lookup"><span data-stu-id="23a5b-150">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="23a5b-151">Caminho</span><span class="sxs-lookup"><span data-stu-id="23a5b-151">Path</span></span>    | <span data-ttu-id="23a5b-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="23a5b-152">Description</span></span> |
|:---------|:-------------|
|[`/users`](../api/user-list.md) | <span data-ttu-id="23a5b-153">Lista os usuários na organização.</span><span class="sxs-lookup"><span data-stu-id="23a5b-153">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user-get.md) | <span data-ttu-id="23a5b-154">Obtém um usuário específico pela id.</span><span class="sxs-lookup"><span data-stu-id="23a5b-154">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| <span data-ttu-id="23a5b-155">Obtém a foto de perfil do usuário.</span><span class="sxs-lookup"><span data-stu-id="23a5b-155">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user-list-manager.md) | <span data-ttu-id="23a5b-156">Obtém o gerente do usuário.</span><span class="sxs-lookup"><span data-stu-id="23a5b-156">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user-list-messages.md)| <span data-ttu-id="23a5b-157">Lista as mensagens de email do usuário em sua caixa de entrada principal.</span><span class="sxs-lookup"><span data-stu-id="23a5b-157">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user-list-events.md) | <span data-ttu-id="23a5b-158">Lista os eventos futuros do usuário em seu calendário.</span><span class="sxs-lookup"><span data-stu-id="23a5b-158">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive-get.md)| <span data-ttu-id="23a5b-159">Obtém o repositório de arquivos do OneDrive do usuário.</span><span class="sxs-lookup"><span data-stu-id="23a5b-159">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| <span data-ttu-id="23a5b-160">Lista os grupos dos quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="23a5b-160">Lists the groups that the user is a member of.</span></span> |

## <a name="whats-new"></a><span data-ttu-id="23a5b-161">Novidades</span><span class="sxs-lookup"><span data-stu-id="23a5b-161">What's new</span></span>
<span data-ttu-id="23a5b-162">Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.</span><span class="sxs-lookup"><span data-stu-id="23a5b-162">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>