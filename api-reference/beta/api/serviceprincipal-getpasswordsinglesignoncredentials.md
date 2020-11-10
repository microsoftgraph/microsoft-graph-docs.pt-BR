---
title: 'servicePrincipalName: getPasswordSingleSignOnCredentials'
description: Obter uma lista de credenciais de logon único usando uma senha para um usuário ou grupo.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7f54c77df6ab0b833d0ca5cc8d157a5167bdd2fc
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980640"
---
# <a name="serviceprincipal-getpasswordsinglesignoncredentials"></a><span data-ttu-id="8f551-103">servicePrincipalName: getPasswordSingleSignOnCredentials</span><span class="sxs-lookup"><span data-stu-id="8f551-103">servicePrincipal: getPasswordSingleSignOnCredentials</span></span>

<span data-ttu-id="8f551-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f551-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f551-105">Obter uma lista de credenciais de logon único usando uma senha para um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="8f551-105">Get a list of single sign-on credentials using a password for a user or group.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f551-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8f551-106">Permissions</span></span>

<span data-ttu-id="8f551-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f551-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8f551-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f551-109">Permission type</span></span>                        | <span data-ttu-id="8f551-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8f551-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8f551-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f551-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8f551-112">Application. ReadWrite. All e Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="8f551-112">Application.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="8f551-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f551-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f551-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f551-114">Not supported.</span></span> |
| <span data-ttu-id="8f551-115">Application</span><span class="sxs-lookup"><span data-stu-id="8f551-115">Application</span></span>                            | <span data-ttu-id="8f551-116">Application. ReadWrite. OwnedBy e Directory. Read. All, Application. ReadWrite. All e Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8f551-116">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="8f551-117">Os usuários podem criar credenciais para si mesmos.</span><span class="sxs-lookup"><span data-stu-id="8f551-117">Users can create credentials for themselves.</span></span> <span data-ttu-id="8f551-118">Os proprietários e administradores da entidade de serviço com as seguintes funções podem criar credenciais para qualquer usuário ou grupo: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span><span class="sxs-lookup"><span data-stu-id="8f551-118">Service principal owners and admins with the following roles can create credentials for any user or group: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span></span> <span data-ttu-id="8f551-119">Para saber mais, confira [funções de diretório](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="8f551-119">To learn more, see [Directory roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="8f551-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f551-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/getPasswordSingleSignOnCredentials
```

## <a name="request-headers"></a><span data-ttu-id="8f551-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f551-121">Request headers</span></span>

| <span data-ttu-id="8f551-122">Nome</span><span class="sxs-lookup"><span data-stu-id="8f551-122">Name</span></span>          | <span data-ttu-id="8f551-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f551-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8f551-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f551-124">Authorization</span></span> | <span data-ttu-id="8f551-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f551-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8f551-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8f551-127">Content-Type</span></span>  | <span data-ttu-id="8f551-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f551-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8f551-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f551-130">Request body</span></span>

<span data-ttu-id="8f551-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f551-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8f551-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8f551-132">Parameter</span></span>    | <span data-ttu-id="8f551-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f551-133">Type</span></span>        | <span data-ttu-id="8f551-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f551-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8f551-135">id</span><span class="sxs-lookup"><span data-stu-id="8f551-135">id</span></span>|<span data-ttu-id="8f551-136">String</span><span class="sxs-lookup"><span data-stu-id="8f551-136">String</span></span>|<span data-ttu-id="8f551-137">A ID do usuário ou grupo ao qual esse conjunto de credenciais pertence.</span><span class="sxs-lookup"><span data-stu-id="8f551-137">The ID of the user or group this credential set belongs to.</span></span>|

## <a name="response"></a><span data-ttu-id="8f551-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f551-138">Response</span></span>

<span data-ttu-id="8f551-139">Se tiver êxito, este método retornará um `200 OK` código de resposta e um novo objeto [passwordSingleSignOnCredentialSet](../resources/passwordsinglesignoncredentialset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8f551-139">If successful, this method returns a `200 OK` response code and a new [passwordSingleSignOnCredentialSet](../resources/passwordsinglesignoncredentialset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8f551-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8f551-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8f551-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f551-141">Request</span></span>

<span data-ttu-id="8f551-142">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f551-142">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8f551-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f551-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8f551-144">C#</span><span class="sxs-lookup"><span data-stu-id="8f551-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-getpasswordsinglesignoncredentials-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8f551-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f551-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-getpasswordsinglesignoncredentials-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8f551-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8f551-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-getpasswordsinglesignoncredentials-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8f551-147">Java</span><span class="sxs-lookup"><span data-stu-id="8f551-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-getpasswordsinglesignoncredentials-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8f551-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f551-148">Response</span></span>

<span data-ttu-id="8f551-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8f551-149">The following is an example of the response.</span></span>

> <span data-ttu-id="8f551-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8f551-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
