---
title: 'servicePrincipalName: createPasswordSingleSignOnCredentials'
description: Criar credenciais de logon único usando uma senha para um usuário ou grupo.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 844aa04d39ada59fa06c92749331f0d71714bd9b
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313237"
---
# <a name="serviceprincipal-createpasswordsinglesignoncredentials"></a><span data-ttu-id="5f585-103">servicePrincipalName: createPasswordSingleSignOnCredentials</span><span class="sxs-lookup"><span data-stu-id="5f585-103">servicePrincipal: createPasswordSingleSignOnCredentials</span></span>

<span data-ttu-id="5f585-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f585-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f585-105">Criar credenciais de logon único usando uma senha para um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="5f585-105">Create single sign-on credentials using a password for a user or group.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f585-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5f585-106">Permissions</span></span>

<span data-ttu-id="5f585-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f585-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5f585-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f585-109">Permission type</span></span>                        | <span data-ttu-id="5f585-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5f585-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5f585-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f585-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5f585-112">Application. ReadWrite. All e Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="5f585-112">Application.ReadWrite.All and Directory.Read.All,  Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="5f585-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f585-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f585-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f585-114">Not supported.</span></span> |
| <span data-ttu-id="5f585-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5f585-115">Application</span></span>                            | <span data-ttu-id="5f585-116">Application. ReadWrite. All e Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="5f585-116">Application.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="5f585-117">Os usuários podem criar credenciais para si mesmos.</span><span class="sxs-lookup"><span data-stu-id="5f585-117">Users can create credentials for themselves.</span></span> <span data-ttu-id="5f585-118">Os proprietários e administradores da entidade de serviço com as seguintes funções podem criar credenciais para qualquer usuário ou grupo: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span><span class="sxs-lookup"><span data-stu-id="5f585-118">Service principal owners and admins with the following roles can create credentials for any user or group: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span></span> <span data-ttu-id="5f585-119">Para saber mais, confira [funções de diretório](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="5f585-119">To learn more, see [Directory roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="5f585-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f585-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/createPasswordSingleSignOnCredentials
```

## <a name="request-headers"></a><span data-ttu-id="5f585-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f585-121">Request headers</span></span>

| <span data-ttu-id="5f585-122">Nome</span><span class="sxs-lookup"><span data-stu-id="5f585-122">Name</span></span>          | <span data-ttu-id="5f585-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f585-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="5f585-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f585-124">Authorization</span></span> | <span data-ttu-id="5f585-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f585-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5f585-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5f585-127">Content-Type</span></span>  | <span data-ttu-id="5f585-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f585-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5f585-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5f585-130">Request body</span></span>

<span data-ttu-id="5f585-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f585-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5f585-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5f585-132">Parameter</span></span>    | <span data-ttu-id="5f585-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f585-133">Type</span></span>        | <span data-ttu-id="5f585-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f585-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5f585-135">id</span><span class="sxs-lookup"><span data-stu-id="5f585-135">id</span></span>|<span data-ttu-id="5f585-136">String</span><span class="sxs-lookup"><span data-stu-id="5f585-136">String</span></span>|<span data-ttu-id="5f585-137">A ID do usuário ou grupo ao qual esse conjunto de credenciais pertence.</span><span class="sxs-lookup"><span data-stu-id="5f585-137">The ID of the user or group this credential set belongs to.</span></span>|
|<span data-ttu-id="5f585-138">las</span><span class="sxs-lookup"><span data-stu-id="5f585-138">credentials</span></span>|<span data-ttu-id="5f585-139">coleção [Credential](../resources/credential.md)</span><span class="sxs-lookup"><span data-stu-id="5f585-139">[credential](../resources/credential.md) collection</span></span>|<span data-ttu-id="5f585-140">Uma lista de objetos de credencial que definem o fluxo de entrada completo.</span><span class="sxs-lookup"><span data-stu-id="5f585-140">A list of credential objects that define the complete sign in flow.</span></span>|

## <a name="response"></a><span data-ttu-id="5f585-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f585-141">Response</span></span>

<span data-ttu-id="5f585-142">Se tiver êxito, este método retornará um `200 OK` código de resposta e um novo objeto [passwordSingleSignOnCredentialSet](../resources/passwordsinglesignoncredentialset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5f585-142">If successful, this method returns a `200 OK` response code and a new [passwordSingleSignOnCredentialSet](../resources/passwordsinglesignoncredentialset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5f585-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5f585-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5f585-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f585-144">Request</span></span>

<span data-ttu-id="5f585-145">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f585-145">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5f585-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="5f585-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_createpasswordsinglesignoncredentials"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/createPasswordSingleSignOnCredentials
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
# <a name="c"></a>[<span data-ttu-id="5f585-147">C#</span><span class="sxs-lookup"><span data-stu-id="5f585-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-createpasswordsinglesignoncredentials-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5f585-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f585-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-createpasswordsinglesignoncredentials-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5f585-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5f585-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-createpasswordsinglesignoncredentials-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5f585-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f585-150">Response</span></span>

<span data-ttu-id="5f585-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5f585-151">The following is an example of the response.</span></span>

> <span data-ttu-id="5f585-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5f585-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "servicePrincipal: createPasswordSingleSignOnCredentials",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->