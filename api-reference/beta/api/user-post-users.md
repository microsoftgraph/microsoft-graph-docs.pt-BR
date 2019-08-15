---
title: Criar usuário
description: Crie um novo usuário.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7c9042fef0de54465f1876486f9d2bd8a7e67e0a
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421873"
---
# <a name="create-user"></a><span data-ttu-id="f1ed8-103">Criar usuário</span><span class="sxs-lookup"><span data-stu-id="f1ed8-103">Create user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1ed8-104">Criar um novo [usuário](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="f1ed8-104">Create a new [user](../resources/user.md).</span></span>
<span data-ttu-id="f1ed8-105">O corpo da solicitação contém o usuário a ser criado.</span><span class="sxs-lookup"><span data-stu-id="f1ed8-105">The request body contains the user to create.</span></span> <span data-ttu-id="f1ed8-106">No mínimo, você deve especificar as propriedades necessárias para o usuário.</span><span class="sxs-lookup"><span data-stu-id="f1ed8-106">At a minimum, you must specify the required properties for the user.</span></span> <span data-ttu-id="f1ed8-107">Opcionalmente, você pode especificar outras propriedades graváveis.</span><span class="sxs-lookup"><span data-stu-id="f1ed8-107">You can optionally specify any other writable properties.</span></span>

>[!NOTE]
><span data-ttu-id="f1ed8-108">Para criar usuários externos, use a [API de convite](invitation-post.md).</span><span class="sxs-lookup"><span data-stu-id="f1ed8-108">To create external users, use the [invitation API](invitation-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f1ed8-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="f1ed8-109">Permissions</span></span>

<span data-ttu-id="f1ed8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1ed8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1ed8-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1ed8-112">Permission type</span></span>      | <span data-ttu-id="f1ed8-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1ed8-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1ed8-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1ed8-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f1ed8-115">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f1ed8-115">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f1ed8-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1ed8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1ed8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1ed8-117">Not supported.</span></span>    |
|<span data-ttu-id="f1ed8-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1ed8-118">Application</span></span> | <span data-ttu-id="f1ed8-119">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1ed8-119">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1ed8-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1ed8-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="f1ed8-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1ed8-121">Request headers</span></span>
| <span data-ttu-id="f1ed8-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f1ed8-122">Header</span></span>       | <span data-ttu-id="f1ed8-123">Valor</span><span class="sxs-lookup"><span data-stu-id="f1ed8-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f1ed8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1ed8-124">Authorization</span></span>  | <span data-ttu-id="f1ed8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1ed8-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f1ed8-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f1ed8-127">Content-Type</span></span>  | <span data-ttu-id="f1ed8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f1ed8-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f1ed8-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1ed8-129">Request body</span></span>

<span data-ttu-id="f1ed8-130">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="f1ed8-130">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="f1ed8-131">A tabela a seguir mostra as propriedades que são necessárias ao criar um usuário.</span><span class="sxs-lookup"><span data-stu-id="f1ed8-131">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="f1ed8-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f1ed8-132">Parameter</span></span> | <span data-ttu-id="f1ed8-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1ed8-133">Type</span></span> | <span data-ttu-id="f1ed8-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1ed8-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1ed8-135">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="f1ed8-135">accountEnabled</span></span> |<span data-ttu-id="f1ed8-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="f1ed8-136">Boolean</span></span> |<span data-ttu-id="f1ed8-137">true se a conta estiver habilitada; caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="f1ed8-137">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="f1ed8-138">displayName</span><span class="sxs-lookup"><span data-stu-id="f1ed8-138">displayName</span></span> |<span data-ttu-id="f1ed8-139">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1ed8-139">string</span></span> |<span data-ttu-id="f1ed8-140">Nome de exibição no catálogo de endereços do usuário.</span><span class="sxs-lookup"><span data-stu-id="f1ed8-140">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="f1ed8-141">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="f1ed8-141">onPremisesImmutableId</span></span> |<span data-ttu-id="f1ed8-142">string</span><span class="sxs-lookup"><span data-stu-id="f1ed8-142">string</span></span> |<span data-ttu-id="f1ed8-143">Só precisa ser especificado ao criar uma nova conta de usuário se você está usando um domínio federado para propriedade userPrincipalName (UPN) do usuário.</span><span class="sxs-lookup"><span data-stu-id="f1ed8-143">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="f1ed8-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="f1ed8-144">mailNickname</span></span> |<span data-ttu-id="f1ed8-145">string</span><span class="sxs-lookup"><span data-stu-id="f1ed8-145">string</span></span> |<span data-ttu-id="f1ed8-146">O alias de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="f1ed8-146">The mail alias for the user.</span></span>|
|<span data-ttu-id="f1ed8-147">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="f1ed8-147">passwordProfile</span></span>|[<span data-ttu-id="f1ed8-148">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="f1ed8-148">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="f1ed8-149">O perfil de senha do usuário.</span><span class="sxs-lookup"><span data-stu-id="f1ed8-149">The password profile for the user.</span></span>|
|<span data-ttu-id="f1ed8-150">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f1ed8-150">userPrincipalName</span></span> |<span data-ttu-id="f1ed8-151">string</span><span class="sxs-lookup"><span data-stu-id="f1ed8-151">string</span></span> |<span data-ttu-id="f1ed8-152">Nome UPN (usuario@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="f1ed8-152">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="f1ed8-153">Como o recurso de **usuário** oferece suporte a [extensões](/graph/extensibility-overview), você `POST` pode usar a operação e adicionar propriedades personalizadas com seus próprios dados à instância de usuário ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="f1ed8-153">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

>[!NOTE]
><span data-ttu-id="f1ed8-154">Os usuários federados criados usando essa API serão forçados a entrar a cada 12 horas por padrão.</span><span class="sxs-lookup"><span data-stu-id="f1ed8-154">Federated users created using this API will be forced to sign in every 12 hours by default.</span></span> <span data-ttu-id="f1ed8-155">Para obter mais informações sobre como alterar isso, confira [exceções para tempos de vida do token](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span><span class="sxs-lookup"><span data-stu-id="f1ed8-155">For more information about how to change this, see [Exceptions for token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

## <a name="response"></a><span data-ttu-id="f1ed8-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1ed8-156">Response</span></span>

<span data-ttu-id="f1ed8-157">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1ed8-157">If successful, this method returns a `201 Created` response code and a [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1ed8-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1ed8-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1ed8-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1ed8-159">Request</span></span>
<span data-ttu-id="f1ed8-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1ed8-160">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f1ed8-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1ed8-161">HTTP</span></span>](#tab/http)
<!-- {  
  "blockType": "request",   
  "name": "create_user_from_users_2"    
}-->

```http
POST https://graph.microsoft.com/beta/users
Content-type: application/json

{
  "accountEnabled": true,
  "displayName": "displayName-value",
  "mailNickname": "mailNickname-value",
  "userPrincipalName": "upn-value@tenant-value.onmicrosoft.com",
  "passwordProfile" : {
    "forceChangePasswordNextSignIn": true,
    "password": "password-value"
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f1ed8-162">C#</span><span class="sxs-lookup"><span data-stu-id="f1ed8-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f1ed8-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1ed8-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f1ed8-164">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f1ed8-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="f1ed8-165">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="f1ed8-165">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f1ed8-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1ed8-166">Response</span></span>
<span data-ttu-id="f1ed8-167">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1ed8-167">Here is an example of the response.</span></span> 

[!NOTE]
<span data-ttu-id="f1ed8-168">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f1ed8-168">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f1ed8-169">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1ed8-169">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/$entity",
    "id": "id-value",
    "businessPhones": [],
    "displayName": "displayName-value",
    "givenName": null,
    "jobTitle": null,
    "mail": null,
    "mobilePhone": null,
    "officeLocation": null,
    "preferredLanguage": null,
    "surname": null,
    "userPrincipalName": "upn-value@tenant-value.onmicrosoft.com"
}
```

## <a name="see-also"></a><span data-ttu-id="f1ed8-170">Confira também</span><span class="sxs-lookup"><span data-stu-id="f1ed8-170">See also</span></span>

- [<span data-ttu-id="f1ed8-171">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="f1ed8-171">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="f1ed8-172">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="f1ed8-172">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="f1ed8-173">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="f1ed8-173">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
