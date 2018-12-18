---
title: Criar usuário
description: Use essa API para criar um novo usuário.
author: dkershaw10
ms.openlocfilehash: ace74039d3740b51487252447ba3d56a018f745e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314851"
---
# <a name="create-user"></a><span data-ttu-id="aee04-103">Criar usuário</span><span class="sxs-lookup"><span data-stu-id="aee04-103">Create user</span></span>

> <span data-ttu-id="aee04-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="aee04-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aee04-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="aee04-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aee04-106">Use essa API para criar um novo usuário.</span><span class="sxs-lookup"><span data-stu-id="aee04-106">Use this API to create a new user.</span></span>
<span data-ttu-id="aee04-107">O corpo da solicitação contém o usuário crie.</span><span class="sxs-lookup"><span data-stu-id="aee04-107">The request body contains the user to create.</span></span> <span data-ttu-id="aee04-108">No mínimo, você deve especificar as propriedades necessárias para o usuário.</span><span class="sxs-lookup"><span data-stu-id="aee04-108">At a minimum, you must specify the required properties for the user.</span></span> <span data-ttu-id="aee04-109">Opcionalmente, você pode especificar todas as outras propriedades graváveis.</span><span class="sxs-lookup"><span data-stu-id="aee04-109">You can optionally specify any other writable properties.</span></span>
## <a name="permissions"></a><span data-ttu-id="aee04-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="aee04-110">Permissions</span></span>
<span data-ttu-id="aee04-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aee04-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aee04-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aee04-113">Permission type</span></span>      | <span data-ttu-id="aee04-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aee04-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aee04-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aee04-115">Delegated (work or school account)</span></span> | <span data-ttu-id="aee04-116">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aee04-116">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="aee04-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aee04-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aee04-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aee04-118">Not supported.</span></span>    |
|<span data-ttu-id="aee04-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aee04-119">Application</span></span> | <span data-ttu-id="aee04-120">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aee04-120">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aee04-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aee04-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="aee04-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aee04-122">Request headers</span></span>
| <span data-ttu-id="aee04-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aee04-123">Header</span></span>       | <span data-ttu-id="aee04-124">Valor</span><span class="sxs-lookup"><span data-stu-id="aee04-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="aee04-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="aee04-125">Authorization</span></span>  | <span data-ttu-id="aee04-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aee04-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="aee04-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aee04-128">Content-Type</span></span>  | <span data-ttu-id="aee04-129">application/json</span><span class="sxs-lookup"><span data-stu-id="aee04-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aee04-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aee04-130">Request body</span></span>
<span data-ttu-id="aee04-131">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="aee04-131">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="aee04-132">A tabela a seguir mostra as propriedades que são necessárias ao criar um usuário.</span><span class="sxs-lookup"><span data-stu-id="aee04-132">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="aee04-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="aee04-133">Parameter</span></span> | <span data-ttu-id="aee04-134">Type</span><span class="sxs-lookup"><span data-stu-id="aee04-134">Type</span></span> | <span data-ttu-id="aee04-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="aee04-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aee04-136">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="aee04-136">accountEnabled</span></span> |<span data-ttu-id="aee04-137">booliano</span><span class="sxs-lookup"><span data-stu-id="aee04-137">boolean</span></span> |<span data-ttu-id="aee04-138">true se a conta estiver habilitada; caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="aee04-138">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="aee04-139">displayName</span><span class="sxs-lookup"><span data-stu-id="aee04-139">displayName</span></span> |<span data-ttu-id="aee04-140">string</span><span class="sxs-lookup"><span data-stu-id="aee04-140">string</span></span> |<span data-ttu-id="aee04-141">Nome de exibição no catálogo de endereços do usuário.</span><span class="sxs-lookup"><span data-stu-id="aee04-141">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="aee04-142">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="aee04-142">onPremisesImmutableId</span></span> |<span data-ttu-id="aee04-143">string</span><span class="sxs-lookup"><span data-stu-id="aee04-143">string</span></span> |<span data-ttu-id="aee04-144">Só precisa ser especificado ao criar uma nova conta de usuário se você está usando um domínio federado para propriedade userPrincipalName (UPN) do usuário.</span><span class="sxs-lookup"><span data-stu-id="aee04-144">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="aee04-145">mailNickname</span><span class="sxs-lookup"><span data-stu-id="aee04-145">mailNickname</span></span> |<span data-ttu-id="aee04-146">string</span><span class="sxs-lookup"><span data-stu-id="aee04-146">string</span></span> |<span data-ttu-id="aee04-147">O alias de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="aee04-147">The mail alias for the user.</span></span>|
|<span data-ttu-id="aee04-148">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="aee04-148">passwordProfile</span></span>|[<span data-ttu-id="aee04-149">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="aee04-149">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="aee04-150">O perfil de senha do usuário.</span><span class="sxs-lookup"><span data-stu-id="aee04-150">The password profile for the user.</span></span>|
|<span data-ttu-id="aee04-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="aee04-151">userPrincipalName</span></span> |<span data-ttu-id="aee04-152">string</span><span class="sxs-lookup"><span data-stu-id="aee04-152">string</span></span> |<span data-ttu-id="aee04-153">Nome UPN (usuario@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="aee04-153">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="aee04-154">Desde que o recurso de **usuário** oferece suporte às [extensões](/graph/extensibility-overview), você pode usar o `POST` operação e adicionar propriedades personalizadas com seus próprios dados à instância do usuário ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="aee04-154">Since the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="aee04-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="aee04-155">Response</span></span>

<span data-ttu-id="aee04-156">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aee04-156">If successful, this method returns `201 Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aee04-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aee04-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aee04-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aee04-158">Request</span></span>
<span data-ttu-id="aee04-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aee04-159">Here is an example of the request.</span></span>
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
  "userPrincipalName": "upn-value@tenant-value@onmicrosoft.com",
  "passwordProfile" : {
    "forceChangePasswordNextSignIn": true,
    "password": "password-value"
  }
}
```
<span data-ttu-id="aee04-160">No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="aee04-160">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="aee04-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="aee04-161">Response</span></span>
<span data-ttu-id="aee04-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aee04-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="aee04-165">Confira também</span><span class="sxs-lookup"><span data-stu-id="aee04-165">See also</span></span>

- [<span data-ttu-id="aee04-166">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="aee04-166">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="aee04-167">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="aee04-167">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="aee04-168">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="aee04-168">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
