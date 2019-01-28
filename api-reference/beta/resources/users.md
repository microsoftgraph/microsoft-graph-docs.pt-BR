---
title: Trabalhando com usuários no Microsoft Graph
description: Você pode usar o Microsoft Graph para criar experiências envolventes do aplicativo com base nos usuários, em suas relações com outros usuários e em grupos e seus emails, calendário e arquivos.
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b98bdd3f84171823942b3a48dd49a8993597a5ee
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572175"
---
# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="6327b-103">Trabalhar com usuários no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6327b-103">Working with users in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6327b-104">Você pode usar o Microsoft Graph para criar experiências envolventes do aplicativo com base nos usuários, em suas relações com outros usuários e em grupos e seus emails, calendário e arquivos.</span><span class="sxs-lookup"><span data-stu-id="6327b-104">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="6327b-105">Você pode acessar usuários pelo Microsoft Graph de duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="6327b-105">You can access users through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="6327b-106">Por sua ID, `/users/{id}`</span><span class="sxs-lookup"><span data-stu-id="6327b-106">By their ID, `/users/{id}`</span></span> 
- <span data-ttu-id="6327b-107">Usando o alias `/me` para o usuário conectado, que é igual a `/users/{signed-in user's id}`</span><span class="sxs-lookup"><span data-stu-id="6327b-107">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="6327b-108">Autorização</span><span class="sxs-lookup"><span data-stu-id="6327b-108">Authorization</span></span>
<span data-ttu-id="6327b-p101">Uma das seguintes [permissões](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) é necessária para acessar operações de usuário. As três primeiras permissões podem ser concedidas a um aplicativo por um usuário. O restante só pode ser concedido a um aplicativo pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="6327b-p101">One of the following [permissions](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="6327b-112">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="6327b-112">User.ReadBasic.All</span></span>
- <span data-ttu-id="6327b-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="6327b-113">User.Read</span></span>
- <span data-ttu-id="6327b-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6327b-114">User.ReadWrite</span></span>
- <span data-ttu-id="6327b-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6327b-115">User.Read.All</span></span>
- <span data-ttu-id="6327b-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6327b-116">User.ReadWrite.All</span></span>
- <span data-ttu-id="6327b-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6327b-117">Directory.Read.All</span></span>
- <span data-ttu-id="6327b-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6327b-118">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="6327b-119">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6327b-119">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="6327b-120">Propriedades comuns</span><span class="sxs-lookup"><span data-stu-id="6327b-120">Common properties</span></span>

<span data-ttu-id="6327b-121">O item a seguir representa o conjunto padrão de propriedades que serão retornadas ao se obter um usuário ou listar usuários.</span><span class="sxs-lookup"><span data-stu-id="6327b-121">The following represent the default set of properties that are returned when getting a user or listing users.</span></span> <span data-ttu-id="6327b-122">Este é um subconjunto de todas as propriedades disponíveis.</span><span class="sxs-lookup"><span data-stu-id="6327b-122">These are a subset of all available properties.</span></span> <span data-ttu-id="6327b-123">Para obter mais propriedades do usuário, use o parâmetro de consulta `$select`.</span><span class="sxs-lookup"><span data-stu-id="6327b-123">To get more user properties, use the `$select` query parameter.</span></span> 

|<span data-ttu-id="6327b-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6327b-124">Property</span></span> |<span data-ttu-id="6327b-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="6327b-125">Description</span></span> |
|:----------|:-------------|
|<span data-ttu-id="6327b-126">id</span><span class="sxs-lookup"><span data-stu-id="6327b-126">id</span></span> | <span data-ttu-id="6327b-127">O identificador exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="6327b-127">The unique identifier for the user.</span></span>|
|<span data-ttu-id="6327b-128">businessPhones</span><span class="sxs-lookup"><span data-stu-id="6327b-128">businessPhones</span></span> | <span data-ttu-id="6327b-129">Os números de telefone do usuário.</span><span class="sxs-lookup"><span data-stu-id="6327b-129">The user's phone numbers.</span></span>|
|<span data-ttu-id="6327b-130">displayName</span><span class="sxs-lookup"><span data-stu-id="6327b-130">displayName</span></span> | <span data-ttu-id="6327b-131">O nome exibido no catálogo de endereços do usuário.</span><span class="sxs-lookup"><span data-stu-id="6327b-131">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="6327b-132">givenName</span><span class="sxs-lookup"><span data-stu-id="6327b-132">givenName</span></span>| <span data-ttu-id="6327b-133">O nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="6327b-133">The first name of the user.</span></span> |
|<span data-ttu-id="6327b-134">jobTitle</span><span class="sxs-lookup"><span data-stu-id="6327b-134">jobTitle</span></span> | <span data-ttu-id="6327b-135">O cargo do usuário.</span><span class="sxs-lookup"><span data-stu-id="6327b-135">The user's job title.</span></span>|
|<span data-ttu-id="6327b-136">email</span><span class="sxs-lookup"><span data-stu-id="6327b-136">mail</span></span>| <span data-ttu-id="6327b-137">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="6327b-137">The user's email address.</span></span> |
|<span data-ttu-id="6327b-138">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="6327b-138">mobilePhone</span></span> | <span data-ttu-id="6327b-139">O número de telefone celular do usuário.</span><span class="sxs-lookup"><span data-stu-id="6327b-139">The user's cellphone number.</span></span>|
|<span data-ttu-id="6327b-140">officeLocation</span><span class="sxs-lookup"><span data-stu-id="6327b-140">officeLocation</span></span> | <span data-ttu-id="6327b-141">O local do escritório físico do usuário.</span><span class="sxs-lookup"><span data-stu-id="6327b-141">The user's physical office location.</span></span>|
|<span data-ttu-id="6327b-142">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="6327b-142">preferredLanguage</span></span> | <span data-ttu-id="6327b-143">O idioma preferencial do usuário.</span><span class="sxs-lookup"><span data-stu-id="6327b-143">The user's language of preference.</span></span>|
|<span data-ttu-id="6327b-144">surname</span><span class="sxs-lookup"><span data-stu-id="6327b-144">surname</span></span>| <span data-ttu-id="6327b-145">O sobrenome do usuário.</span><span class="sxs-lookup"><span data-stu-id="6327b-145">The last name of the user.</span></span> |
|<span data-ttu-id="6327b-146">email</span><span class="sxs-lookup"><span data-stu-id="6327b-146">mail</span></span>| <span data-ttu-id="6327b-147">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="6327b-147">The user's email address.</span></span> |
|<span data-ttu-id="6327b-148">photo</span><span class="sxs-lookup"><span data-stu-id="6327b-148">photo</span></span>| <span data-ttu-id="6327b-149">A foto de perfil do usuário.</span><span class="sxs-lookup"><span data-stu-id="6327b-149">The user's profile photo. Read-only.</span></span> |
|<span data-ttu-id="6327b-150">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6327b-150">userPrincipalName</span></span>| <span data-ttu-id="6327b-151">O nome UPN do usuário.</span><span class="sxs-lookup"><span data-stu-id="6327b-151">The user's principal name.</span></span> |

<span data-ttu-id="6327b-152">Para obter detalhes e uma lista de todas as propriedades, confira o objeto [user](user.md).</span><span class="sxs-lookup"><span data-stu-id="6327b-152">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="6327b-153">Operações comuns</span><span class="sxs-lookup"><span data-stu-id="6327b-153">Common operations</span></span>
><span data-ttu-id="6327b-154">**Observação:** Algumas destas operações exigem permissões adicionais.</span><span class="sxs-lookup"><span data-stu-id="6327b-154">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="6327b-155">Caminho</span><span class="sxs-lookup"><span data-stu-id="6327b-155">Path</span></span>    | <span data-ttu-id="6327b-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="6327b-156">Description</span></span> |
|:---------|:-------------|
|[`/users`](../api/user-list.md) | <span data-ttu-id="6327b-157">Lista os usuários na organização.</span><span class="sxs-lookup"><span data-stu-id="6327b-157">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user-get.md) | <span data-ttu-id="6327b-158">Obtém um usuário específico pela id.</span><span class="sxs-lookup"><span data-stu-id="6327b-158">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| <span data-ttu-id="6327b-159">Obtém a foto de perfil do usuário.</span><span class="sxs-lookup"><span data-stu-id="6327b-159">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user-list-manager.md) | <span data-ttu-id="6327b-160">Obtém o gerente do usuário.</span><span class="sxs-lookup"><span data-stu-id="6327b-160">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user-list-messages.md)| <span data-ttu-id="6327b-161">Lista as mensagens de email do usuário em sua caixa de entrada principal.</span><span class="sxs-lookup"><span data-stu-id="6327b-161">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user-list-events.md) | <span data-ttu-id="6327b-162">Lista os eventos futuros do usuário em seu calendário.</span><span class="sxs-lookup"><span data-stu-id="6327b-162">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive-get.md)| <span data-ttu-id="6327b-163">Obtém o repositório de arquivos do OneDrive do usuário.</span><span class="sxs-lookup"><span data-stu-id="6327b-163">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| <span data-ttu-id="6327b-164">Lista os grupos dos quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="6327b-164">Lists the groups that the user is a member of.</span></span> |
|[`/users/{id}/joinedTeams`](../api/user-list-joinedteams.md)| <span data-ttu-id="6327b-165">Lista as Microsoft Teams das quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="6327b-165">Get the Microsoft Teams that the user is a direct member of.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/users.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
