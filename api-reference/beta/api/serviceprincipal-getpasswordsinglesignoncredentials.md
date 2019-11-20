---
title: 'servicePrincipalName: getPasswordSingleSignOnCredentials'
description: Obter uma lista de credenciais de logon único usando uma senha para um usuário ou grupo.
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4ab87d51d39020336172e645d209307706140356
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/20/2019
ms.locfileid: "38747829"
---
# <a name="serviceprincipal-getpasswordsinglesignoncredentials"></a><span data-ttu-id="ddd1d-103">servicePrincipalName: getPasswordSingleSignOnCredentials</span><span class="sxs-lookup"><span data-stu-id="ddd1d-103">servicePrincipal: getPasswordSingleSignOnCredentials</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddd1d-104">Obter uma lista de credenciais de logon único usando uma senha para um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="ddd1d-104">Get a list of single sign-on credentials using a password for a user or group.</span></span>

## <a name="permissions"></a><span data-ttu-id="ddd1d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ddd1d-105">Permissions</span></span>

<span data-ttu-id="ddd1d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddd1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ddd1d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ddd1d-108">Permission type</span></span>                        | <span data-ttu-id="ddd1d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ddd1d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ddd1d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ddd1d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ddd1d-111">Application. ReadWrite. All (também precisa Directory. Read. All), Directory. AccessAsUser. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ddd1d-111">Application.ReadWrite.All (also needs Directory.Read.All), Directory.AccessAsUser.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="ddd1d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ddd1d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddd1d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ddd1d-113">Not supported.</span></span> |
| <span data-ttu-id="ddd1d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddd1d-114">Application</span></span>                            | <span data-ttu-id="ddd1d-115">Application. ReadWrite. All (também precisa Directory. Read. All), Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ddd1d-115">Application.ReadWrite.All (also needs Directory.Read.All), Directory.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="ddd1d-116">Os usuários podem criar credenciais para si mesmos.</span><span class="sxs-lookup"><span data-stu-id="ddd1d-116">Users can create credentials for themselves.</span></span> <span data-ttu-id="ddd1d-117">Os proprietários e administradores da entidade de serviço com as seguintes funções podem criar credenciais para qualquer usuário ou grupo: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span><span class="sxs-lookup"><span data-stu-id="ddd1d-117">Service principal owners and admins with the following roles can create credentials for any user or group: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span></span> <span data-ttu-id="ddd1d-118">Para saber mais, confira [funções de diretório](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="ddd1d-118">To learn more, see [Directory roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="ddd1d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ddd1d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/getPasswordSingleSignOnCredentials
```

## <a name="request-headers"></a><span data-ttu-id="ddd1d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ddd1d-120">Request headers</span></span>

| <span data-ttu-id="ddd1d-121">Nome</span><span class="sxs-lookup"><span data-stu-id="ddd1d-121">Name</span></span>          | <span data-ttu-id="ddd1d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddd1d-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ddd1d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ddd1d-123">Authorization</span></span> | <span data-ttu-id="ddd1d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ddd1d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ddd1d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ddd1d-126">Content-Type</span></span>  | <span data-ttu-id="ddd1d-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ddd1d-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ddd1d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ddd1d-129">Request body</span></span>

<span data-ttu-id="ddd1d-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddd1d-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ddd1d-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ddd1d-131">Parameter</span></span>    | <span data-ttu-id="ddd1d-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="ddd1d-132">Type</span></span>        | <span data-ttu-id="ddd1d-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddd1d-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ddd1d-134">id</span><span class="sxs-lookup"><span data-stu-id="ddd1d-134">id</span></span>|<span data-ttu-id="ddd1d-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ddd1d-135">String</span></span>|<span data-ttu-id="ddd1d-136">A ID do usuário ou grupo ao qual esse conjunto de credenciais pertence.</span><span class="sxs-lookup"><span data-stu-id="ddd1d-136">The ID of the user or group this credential set belongs to.</span></span>|

## <a name="response"></a><span data-ttu-id="ddd1d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddd1d-137">Response</span></span>

<span data-ttu-id="ddd1d-138">Se tiver êxito, este método retornará `200 OK` um código de resposta e um novo objeto [passwordSingleSignOnCredentialSet](../resources/passwordsinglesignoncredentialset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ddd1d-138">If successful, this method returns a `200 OK` response code and a new [passwordSingleSignOnCredentialSet](../resources/passwordsinglesignoncredentialset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ddd1d-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ddd1d-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ddd1d-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddd1d-140">Request</span></span>

<span data-ttu-id="ddd1d-141">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddd1d-141">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ddd1d-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="ddd1d-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_getpasswordsinglesignoncredentials"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/getPasswordSingleSignOnCredentials
Content-type: application/json

{
  "id": "5793aa3b-cca9-4794-679a240f8b58"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ddd1d-143">C#</span><span class="sxs-lookup"><span data-stu-id="ddd1d-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-getpasswordsinglesignoncredentials-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ddd1d-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddd1d-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-getpasswordsinglesignoncredentials-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ddd1d-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ddd1d-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-getpasswordsinglesignoncredentials-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ddd1d-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddd1d-146">Response</span></span>

<span data-ttu-id="ddd1d-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ddd1d-147">The following is an example of the response.</span></span>

> <span data-ttu-id="ddd1d-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ddd1d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordSingleSignOnCredentialSet"
} -->
```http
HTTP/1.1 200 OK
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
      "value": null,
      "type": "password"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: getPasswordSingleSignOnCredentials",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
