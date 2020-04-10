---
title: 'servicePrincipalName: updatePasswordSingleSignOnCredentials'
description: Atualize as credenciais de logon único usando uma senha de um usuário ou grupo.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ab8a6d256c3f90dbaaa7197f87dec4fd230c73d0
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218588"
---
# <a name="serviceprincipal-updatepasswordsinglesignoncredentials"></a><span data-ttu-id="03f81-103">servicePrincipalName: updatePasswordSingleSignOnCredentials</span><span class="sxs-lookup"><span data-stu-id="03f81-103">servicePrincipal: updatePasswordSingleSignOnCredentials</span></span>

<span data-ttu-id="03f81-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03f81-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03f81-105">Atualize as credenciais de logon único usando uma senha de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="03f81-105">Update single sign-on credentials using a password for a user or group.</span></span>

## <a name="permissions"></a><span data-ttu-id="03f81-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="03f81-106">Permissions</span></span>

<span data-ttu-id="03f81-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03f81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="03f81-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03f81-109">Permission type</span></span>                        | <span data-ttu-id="03f81-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="03f81-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="03f81-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03f81-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="03f81-112">Application. ReadWrite. All (também precisa Directory. Read. All), Directory. AccessAsUser. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="03f81-112">Application.ReadWrite.All (also needs Directory.Read.All), Directory.AccessAsUser.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="03f81-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03f81-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03f81-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03f81-114">Not supported.</span></span> |
| <span data-ttu-id="03f81-115">Application</span><span class="sxs-lookup"><span data-stu-id="03f81-115">Application</span></span>                            | <span data-ttu-id="03f81-116">Application. ReadWrite. All (também precisa Directory. Read. All), Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="03f81-116">Application.ReadWrite.All (also needs Directory.Read.All), Directory.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="03f81-117">Os usuários podem criar credenciais para si mesmos.</span><span class="sxs-lookup"><span data-stu-id="03f81-117">Users can create credentials for themselves.</span></span> <span data-ttu-id="03f81-118">Os proprietários e administradores da entidade de serviço com as seguintes funções podem criar credenciais para qualquer usuário ou grupo: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span><span class="sxs-lookup"><span data-stu-id="03f81-118">Service principal owners and admins with the following roles can create credentials for any user or group: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span></span> <span data-ttu-id="03f81-119">Para saber mais, confira [funções de diretório](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="03f81-119">To learn more, see [Directory roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="03f81-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03f81-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/updatePasswordSingleSignOnCredentials
```

## <a name="request-headers"></a><span data-ttu-id="03f81-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03f81-121">Request headers</span></span>

| <span data-ttu-id="03f81-122">Nome</span><span class="sxs-lookup"><span data-stu-id="03f81-122">Name</span></span>          | <span data-ttu-id="03f81-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="03f81-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="03f81-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="03f81-124">Authorization</span></span> | <span data-ttu-id="03f81-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03f81-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="03f81-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="03f81-127">Content-Type</span></span>  | <span data-ttu-id="03f81-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03f81-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="03f81-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03f81-130">Request body</span></span>

<span data-ttu-id="03f81-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="03f81-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="03f81-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="03f81-132">Parameter</span></span>    | <span data-ttu-id="03f81-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="03f81-133">Type</span></span>        | <span data-ttu-id="03f81-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="03f81-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="03f81-135">id</span><span class="sxs-lookup"><span data-stu-id="03f81-135">id</span></span>|<span data-ttu-id="03f81-136">String</span><span class="sxs-lookup"><span data-stu-id="03f81-136">String</span></span>|<span data-ttu-id="03f81-137">A ID do usuário ou grupo ao qual esse conjunto de credenciais pertence.</span><span class="sxs-lookup"><span data-stu-id="03f81-137">The ID of the user or group this credential set belongs to.</span></span>|
|<span data-ttu-id="03f81-138">las</span><span class="sxs-lookup"><span data-stu-id="03f81-138">credentials</span></span>|<span data-ttu-id="03f81-139">coleção [Credential](../resources/credential.md)</span><span class="sxs-lookup"><span data-stu-id="03f81-139">[credential](../resources/credential.md) collection</span></span>|<span data-ttu-id="03f81-140">Uma lista de objetos de credencial que definem o fluxo de entrada completo.</span><span class="sxs-lookup"><span data-stu-id="03f81-140">A list of credential objects that define the complete sign in flow.</span></span>|

## <a name="response"></a><span data-ttu-id="03f81-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="03f81-141">Response</span></span>

<span data-ttu-id="03f81-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03f81-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="03f81-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="03f81-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="03f81-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03f81-145">Request</span></span>

<span data-ttu-id="03f81-146">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="03f81-146">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="03f81-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="03f81-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="03f81-148">C#</span><span class="sxs-lookup"><span data-stu-id="03f81-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-updatepasswordsinglesignoncredentials-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03f81-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03f81-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-updatepasswordsinglesignoncredentials-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03f81-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03f81-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-updatepasswordsinglesignoncredentials-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="03f81-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="03f81-151">Response</span></span>

<span data-ttu-id="03f81-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="03f81-152">The following is an example of the response.</span></span>
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
