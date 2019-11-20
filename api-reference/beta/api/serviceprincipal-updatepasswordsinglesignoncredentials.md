---
title: 'servicePrincipalName: updatePasswordSingleSignOnCredentials'
description: Atualize as credenciais de logon único usando uma senha de um usuário ou grupo.
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 30e629bddd7de3e55b83c43760d5f146c6849a27
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/20/2019
ms.locfileid: "38747801"
---
# <a name="serviceprincipal-updatepasswordsinglesignoncredentials"></a><span data-ttu-id="2f231-103">servicePrincipalName: updatePasswordSingleSignOnCredentials</span><span class="sxs-lookup"><span data-stu-id="2f231-103">servicePrincipal: updatePasswordSingleSignOnCredentials</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f231-104">Atualize as credenciais de logon único usando uma senha de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="2f231-104">Update single sign-on credentials using a password for a user or group.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f231-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2f231-105">Permissions</span></span>

<span data-ttu-id="2f231-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f231-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2f231-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f231-108">Permission type</span></span>                        | <span data-ttu-id="2f231-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2f231-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2f231-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f231-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2f231-111">Application. ReadWrite. All (também precisa Directory. Read. All), Directory. AccessAsUser. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="2f231-111">Application.ReadWrite.All (also needs Directory.Read.All), Directory.AccessAsUser.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="2f231-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f231-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f231-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f231-113">Not supported.</span></span> |
| <span data-ttu-id="2f231-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f231-114">Application</span></span>                            | <span data-ttu-id="2f231-115">Application. ReadWrite. All (também precisa Directory. Read. All), Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="2f231-115">Application.ReadWrite.All (also needs Directory.Read.All), Directory.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="2f231-116">Os usuários podem criar credenciais para si mesmos.</span><span class="sxs-lookup"><span data-stu-id="2f231-116">Users can create credentials for themselves.</span></span> <span data-ttu-id="2f231-117">Os proprietários e administradores da entidade de serviço com as seguintes funções podem criar credenciais para qualquer usuário ou grupo: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span><span class="sxs-lookup"><span data-stu-id="2f231-117">Service principal owners and admins with the following roles can create credentials for any user or group: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span></span> <span data-ttu-id="2f231-118">Para saber mais, confira [funções de diretório](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="2f231-118">To learn more, see [Directory roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="2f231-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f231-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/updatePasswordSingleSignOnCredentials
```

## <a name="request-headers"></a><span data-ttu-id="2f231-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f231-120">Request headers</span></span>

| <span data-ttu-id="2f231-121">Nome</span><span class="sxs-lookup"><span data-stu-id="2f231-121">Name</span></span>          | <span data-ttu-id="2f231-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f231-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2f231-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f231-123">Authorization</span></span> | <span data-ttu-id="2f231-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f231-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2f231-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2f231-126">Content-Type</span></span>  | <span data-ttu-id="2f231-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f231-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2f231-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f231-129">Request body</span></span>

<span data-ttu-id="2f231-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f231-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2f231-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2f231-131">Parameter</span></span>    | <span data-ttu-id="2f231-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f231-132">Type</span></span>        | <span data-ttu-id="2f231-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f231-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2f231-134">id</span><span class="sxs-lookup"><span data-stu-id="2f231-134">id</span></span>|<span data-ttu-id="2f231-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f231-135">String</span></span>|<span data-ttu-id="2f231-136">A ID do usuário ou grupo ao qual esse conjunto de credenciais pertence.</span><span class="sxs-lookup"><span data-stu-id="2f231-136">The ID of the user or group this credential set belongs to.</span></span>|
|<span data-ttu-id="2f231-137">las</span><span class="sxs-lookup"><span data-stu-id="2f231-137">credentials</span></span>|<span data-ttu-id="2f231-138">coleção [Credential](../resources/credential.md)</span><span class="sxs-lookup"><span data-stu-id="2f231-138">[credential](../resources/credential.md) collection</span></span>|<span data-ttu-id="2f231-139">Uma lista de objetos de credencial que definem o fluxo de entrada completo.</span><span class="sxs-lookup"><span data-stu-id="2f231-139">A list of credential objects that define the complete sign in flow.</span></span>|

## <a name="response"></a><span data-ttu-id="2f231-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f231-140">Response</span></span>

<span data-ttu-id="2f231-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f231-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2f231-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2f231-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2f231-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f231-144">Request</span></span>

<span data-ttu-id="2f231-145">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f231-145">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2f231-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f231-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_updatepasswordsinglesignoncredentials"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/updatePasswordSingleSignOnCredentials
Content-type: application/json

{
  "id": "5793aa3b-cca9-4794-679a240f8b58",
  "credentials": [
    {
      "fieldId": "param_username",
      "value": "myusername",
      "type": "username"
    },
    {
      "fieldId": "param_password",
      "value": "pa$$w0rd",
      "type": "password"
    }
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2f231-147">C#</span><span class="sxs-lookup"><span data-stu-id="2f231-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-updatepasswordsinglesignoncredentials-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2f231-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f231-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-updatepasswordsinglesignoncredentials-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2f231-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f231-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-updatepasswordsinglesignoncredentials-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2f231-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f231-150">Response</span></span>

<span data-ttu-id="2f231-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2f231-151">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: updatePasswordSingleSignOnCredentials",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
