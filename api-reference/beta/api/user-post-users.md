---
title: Criar usuário
description: Use essa API para criar um novo usuário.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9d1e98ffa4be67141d1e5ae679f9f51a71ef92fd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529331"
---
# <a name="create-user"></a><span data-ttu-id="9c1e3-103">Criar usuário</span><span class="sxs-lookup"><span data-stu-id="9c1e3-103">Create user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c1e3-p101">Use essa API para criar um novo Usuário. O corpo da solicitação contém o usuário a ser criado. No mínimo, você deve especificar as propriedades necessárias para o usuário. Opcionalmente, você pode especificar outras propriedades graváveis.</span><span class="sxs-lookup"><span data-stu-id="9c1e3-p101">Use this API to create a new user. The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>
## <a name="permissions"></a><span data-ttu-id="9c1e3-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="9c1e3-108">Permissions</span></span>
<span data-ttu-id="9c1e3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c1e3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c1e3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c1e3-111">Permission type</span></span>      | <span data-ttu-id="9c1e3-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9c1e3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c1e3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c1e3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9c1e3-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9c1e3-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9c1e3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c1e3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c1e3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c1e3-116">Not supported.</span></span>    |
|<span data-ttu-id="9c1e3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c1e3-117">Application</span></span> | <span data-ttu-id="9c1e3-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c1e3-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c1e3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c1e3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="9c1e3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c1e3-120">Request headers</span></span>
| <span data-ttu-id="9c1e3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9c1e3-121">Header</span></span>       | <span data-ttu-id="9c1e3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9c1e3-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9c1e3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c1e3-123">Authorization</span></span>  | <span data-ttu-id="9c1e3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c1e3-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9c1e3-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9c1e3-126">Content-Type</span></span>  | <span data-ttu-id="9c1e3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9c1e3-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9c1e3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c1e3-128">Request body</span></span>
<span data-ttu-id="9c1e3-129">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="9c1e3-129">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="9c1e3-130">A tabela a seguir mostra as propriedades que são necessárias ao criar um usuário.</span><span class="sxs-lookup"><span data-stu-id="9c1e3-130">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="9c1e3-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9c1e3-131">Parameter</span></span> | <span data-ttu-id="9c1e3-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c1e3-132">Type</span></span> | <span data-ttu-id="9c1e3-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c1e3-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c1e3-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="9c1e3-134">accountEnabled</span></span> |<span data-ttu-id="9c1e3-135">booliano</span><span class="sxs-lookup"><span data-stu-id="9c1e3-135">boolean</span></span> |<span data-ttu-id="9c1e3-136">true se a conta estiver habilitada; caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="9c1e3-136">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="9c1e3-137">displayName</span><span class="sxs-lookup"><span data-stu-id="9c1e3-137">displayName</span></span> |<span data-ttu-id="9c1e3-138">string</span><span class="sxs-lookup"><span data-stu-id="9c1e3-138">string</span></span> |<span data-ttu-id="9c1e3-139">Nome de exibição no catálogo de endereços do usuário.</span><span class="sxs-lookup"><span data-stu-id="9c1e3-139">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="9c1e3-140">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="9c1e3-140">onPremisesImmutableId</span></span> |<span data-ttu-id="9c1e3-141">string</span><span class="sxs-lookup"><span data-stu-id="9c1e3-141">string</span></span> |<span data-ttu-id="9c1e3-142">Só precisa ser especificado ao criar uma nova conta de usuário se você está usando um domínio federado para propriedade userPrincipalName (UPN) do usuário.</span><span class="sxs-lookup"><span data-stu-id="9c1e3-142">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="9c1e3-143">mailNickname</span><span class="sxs-lookup"><span data-stu-id="9c1e3-143">mailNickname</span></span> |<span data-ttu-id="9c1e3-144">string</span><span class="sxs-lookup"><span data-stu-id="9c1e3-144">string</span></span> |<span data-ttu-id="9c1e3-145">O alias de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="9c1e3-145">The mail alias for the user.</span></span>|
|<span data-ttu-id="9c1e3-146">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="9c1e3-146">passwordProfile</span></span>|[<span data-ttu-id="9c1e3-147">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="9c1e3-147">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="9c1e3-148">O perfil de senha do usuário.</span><span class="sxs-lookup"><span data-stu-id="9c1e3-148">The password profile for the user.</span></span>|
|<span data-ttu-id="9c1e3-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9c1e3-149">userPrincipalName</span></span> |<span data-ttu-id="9c1e3-150">string</span><span class="sxs-lookup"><span data-stu-id="9c1e3-150">string</span></span> |<span data-ttu-id="9c1e3-151">Nome UPN (usuario@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="9c1e3-151">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="9c1e3-152">Desde que o recurso de **usuário** oferece suporte às [extensões](/graph/extensibility-overview), você pode usar o `POST` operação e adicionar propriedades personalizadas com seus próprios dados à instância do usuário ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="9c1e3-152">Since the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="9c1e3-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c1e3-153">Response</span></span>

<span data-ttu-id="9c1e3-154">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c1e3-154">If successful, this method returns `201 Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c1e3-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9c1e3-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9c1e3-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c1e3-156">Request</span></span>
<span data-ttu-id="9c1e3-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c1e3-157">Here is an example of the request.</span></span>
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
<span data-ttu-id="9c1e3-158">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="9c1e3-158">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="9c1e3-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c1e3-159">Response</span></span>
<span data-ttu-id="9c1e3-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9c1e3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
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

## <a name="see-also"></a><span data-ttu-id="9c1e3-163">Confira também</span><span class="sxs-lookup"><span data-stu-id="9c1e3-163">See also</span></span>

- [<span data-ttu-id="9c1e3-164">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="9c1e3-164">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="9c1e3-165">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="9c1e3-165">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="9c1e3-166">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="9c1e3-166">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
    "Error: /api-reference/beta/api/user-post-users.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
