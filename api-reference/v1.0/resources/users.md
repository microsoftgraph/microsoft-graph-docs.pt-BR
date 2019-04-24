---
title: Trabalhando com usuários no Microsoft Graph
description: Você pode usar o Microsoft Graph para criar experiências envolventes do aplicativo com base nos usuários, em suas relações com outros usuários e em grupos e seus emails, calendário e arquivos.
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bfd7778d3fdc9675880b98a356dd690c4b1eaec8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456882"
---
# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="6be46-103">Trabalhar com usuários no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6be46-103">Working with users in Microsoft Graph</span></span>

<span data-ttu-id="6be46-104">Você pode usar o Microsoft Graph para criar experiências envolventes do aplicativo com base nos usuários, em suas relações com outros usuários e em grupos e seus emails, calendário e arquivos.</span><span class="sxs-lookup"><span data-stu-id="6be46-104">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="6be46-105">Você pode acessar [usuários](user.md) pelo Microsoft Graph de duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="6be46-105">You can access [users](user.md) through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="6be46-106">Por sua ID, `/users/{id | userPrincipalName}`</span><span class="sxs-lookup"><span data-stu-id="6be46-106">By their ID, `/users/{id | userPrincipalName}`</span></span> 
- <span data-ttu-id="6be46-107">Usando o alias `/me` para o usuário conectado, que é igual a `/users/{signed-in user's id}`</span><span class="sxs-lookup"><span data-stu-id="6be46-107">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="6be46-108">Autorização</span><span class="sxs-lookup"><span data-stu-id="6be46-108">Authorization</span></span>

<span data-ttu-id="6be46-p101">Uma das seguintes [permissões](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) é necessária para acessar operações de usuário. As três primeiras permissões podem ser concedidas a um aplicativo por um usuário. O restante só pode ser concedido a um aplicativo pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="6be46-p101">One of the following [permissions](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="6be46-112">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="6be46-112">User.ReadBasic.All</span></span>
- <span data-ttu-id="6be46-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="6be46-113">User.Read</span></span>
- <span data-ttu-id="6be46-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6be46-114">User.ReadWrite</span></span>
- <span data-ttu-id="6be46-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6be46-115">User.Read.All</span></span>
- <span data-ttu-id="6be46-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6be46-116">User.ReadWrite.All</span></span>
- <span data-ttu-id="6be46-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6be46-117">Directory.Read.All</span></span>
- <span data-ttu-id="6be46-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6be46-118">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="6be46-119">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6be46-119">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="6be46-120">Propriedades comuns</span><span class="sxs-lookup"><span data-stu-id="6be46-120">Common properties</span></span>

<span data-ttu-id="6be46-121">O item a seguir representa o conjunto padrão de propriedades que serão retornadas ao se obter um usuário ou listar usuários.</span><span class="sxs-lookup"><span data-stu-id="6be46-121">The following represent the default set of properties that are returned when getting a user or listing users.</span></span> <span data-ttu-id="6be46-122">Este é um subconjunto de todas as propriedades disponíveis.</span><span class="sxs-lookup"><span data-stu-id="6be46-122">These are a subset of all available properties.</span></span> <span data-ttu-id="6be46-123">Para obter mais propriedades do usuário, use o parâmetro de consulta `$select`.</span><span class="sxs-lookup"><span data-stu-id="6be46-123">To get more user properties, use the `$select` query parameter.</span></span> 

|<span data-ttu-id="6be46-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6be46-124">Property</span></span> |<span data-ttu-id="6be46-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="6be46-125">Description</span></span> |
|:----------|:-------------|
|<span data-ttu-id="6be46-126">id</span><span class="sxs-lookup"><span data-stu-id="6be46-126">id</span></span> | <span data-ttu-id="6be46-127">O identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="6be46-127">The unique identifier for the user.</span></span>|
|<span data-ttu-id="6be46-128">businessPhones</span><span class="sxs-lookup"><span data-stu-id="6be46-128">businessPhones</span></span> | <span data-ttu-id="6be46-129">Os números de telefone do usuário.</span><span class="sxs-lookup"><span data-stu-id="6be46-129">The user's phone numbers.</span></span>|
|<span data-ttu-id="6be46-130">displayName</span><span class="sxs-lookup"><span data-stu-id="6be46-130">displayName</span></span> | <span data-ttu-id="6be46-131">O nome exibido no catálogo de endereços do usuário.</span><span class="sxs-lookup"><span data-stu-id="6be46-131">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="6be46-132">givenName</span><span class="sxs-lookup"><span data-stu-id="6be46-132">givenName</span></span>| <span data-ttu-id="6be46-133">O nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="6be46-133">The first name of the user.</span></span> |
|<span data-ttu-id="6be46-134">jobTitle</span><span class="sxs-lookup"><span data-stu-id="6be46-134">jobTitle</span></span> | <span data-ttu-id="6be46-135">O cargo do usuário.</span><span class="sxs-lookup"><span data-stu-id="6be46-135">The user's job title.</span></span>|
|<span data-ttu-id="6be46-136">email</span><span class="sxs-lookup"><span data-stu-id="6be46-136">mail</span></span>| <span data-ttu-id="6be46-137">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="6be46-137">The user's email address.</span></span> |
|<span data-ttu-id="6be46-138">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="6be46-138">mobilePhone</span></span> | <span data-ttu-id="6be46-139">O número de telefone celular do usuário.</span><span class="sxs-lookup"><span data-stu-id="6be46-139">The user's cellphone number.</span></span>|
|<span data-ttu-id="6be46-140">officeLocation</span><span class="sxs-lookup"><span data-stu-id="6be46-140">officeLocation</span></span> | <span data-ttu-id="6be46-141">O local do escritório físico do usuário.</span><span class="sxs-lookup"><span data-stu-id="6be46-141">The user's physical office location.</span></span>|
|<span data-ttu-id="6be46-142">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="6be46-142">preferredLanguage</span></span> | <span data-ttu-id="6be46-143">O idioma preferencial do usuário.</span><span class="sxs-lookup"><span data-stu-id="6be46-143">The user's language of preference.</span></span>|
|<span data-ttu-id="6be46-144">surname</span><span class="sxs-lookup"><span data-stu-id="6be46-144">surname</span></span>| <span data-ttu-id="6be46-145">O sobrenome do usuário.</span><span class="sxs-lookup"><span data-stu-id="6be46-145">The last name of the user.</span></span> |
|<span data-ttu-id="6be46-146">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6be46-146">userPrincipalName</span></span>| <span data-ttu-id="6be46-147">O nome UPN do usuário.</span><span class="sxs-lookup"><span data-stu-id="6be46-147">The user's principal name.</span></span> |

<br/>

<span data-ttu-id="6be46-148">Para obter detalhes e uma lista de todas as propriedades, confira o objeto [user](user.md).</span><span class="sxs-lookup"><span data-stu-id="6be46-148">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="6be46-149">Operações comuns</span><span class="sxs-lookup"><span data-stu-id="6be46-149">Common operations</span></span>

> <span data-ttu-id="6be46-150">**Observação:** Algumas destas operações exigem permissões adicionais.</span><span class="sxs-lookup"><span data-stu-id="6be46-150">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="6be46-151">Caminho</span><span class="sxs-lookup"><span data-stu-id="6be46-151">Path</span></span>    | <span data-ttu-id="6be46-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="6be46-152">Description</span></span> |
|:---------|:-------------|
|[`/users`](../api/user-list.md) | <span data-ttu-id="6be46-153">Lista os usuários na organização.</span><span class="sxs-lookup"><span data-stu-id="6be46-153">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user-get.md) | <span data-ttu-id="6be46-154">Obtém um usuário específico pela id.</span><span class="sxs-lookup"><span data-stu-id="6be46-154">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| <span data-ttu-id="6be46-155">Obtém a foto de perfil do usuário.</span><span class="sxs-lookup"><span data-stu-id="6be46-155">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user-list-manager.md) | <span data-ttu-id="6be46-156">Obtém o gerente do usuário.</span><span class="sxs-lookup"><span data-stu-id="6be46-156">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user-list-messages.md)| <span data-ttu-id="6be46-157">Lista as mensagens de email do usuário em sua caixa de entrada principal.</span><span class="sxs-lookup"><span data-stu-id="6be46-157">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user-list-events.md) | <span data-ttu-id="6be46-158">Lista os eventos futuros do usuário em seu calendário.</span><span class="sxs-lookup"><span data-stu-id="6be46-158">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive-get.md)| <span data-ttu-id="6be46-159">Obtém o repositório de arquivos do OneDrive do usuário.</span><span class="sxs-lookup"><span data-stu-id="6be46-159">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| <span data-ttu-id="6be46-160">Lista os grupos dos quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="6be46-160">Lists the groups that the user is a member of.</span></span> |
