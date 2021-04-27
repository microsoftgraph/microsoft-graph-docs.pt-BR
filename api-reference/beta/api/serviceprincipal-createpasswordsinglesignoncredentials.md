---
title: 'servicePrincipal: createPasswordSingleSignOnCredentials'
description: Crie credenciais de login único usando uma senha para um usuário ou grupo.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: a83e5c1eeb09cab08f3b086e50f864172e5061b5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051960"
---
# <a name="serviceprincipal-createpasswordsinglesignoncredentials"></a><span data-ttu-id="446d1-103">servicePrincipal: createPasswordSingleSignOnCredentials</span><span class="sxs-lookup"><span data-stu-id="446d1-103">servicePrincipal: createPasswordSingleSignOnCredentials</span></span>

<span data-ttu-id="446d1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="446d1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="446d1-105">Crie credenciais de login único usando uma senha para um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="446d1-105">Create single sign-on credentials using a password for a user or group.</span></span>

## <a name="permissions"></a><span data-ttu-id="446d1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="446d1-106">Permissions</span></span>

<span data-ttu-id="446d1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="446d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="446d1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="446d1-109">Permission type</span></span>                        | <span data-ttu-id="446d1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="446d1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="446d1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="446d1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="446d1-112">Application.ReadWrite.All e Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="446d1-112">Application.ReadWrite.All and Directory.Read.All,  Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="446d1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="446d1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="446d1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="446d1-114">Not supported.</span></span> |
| <span data-ttu-id="446d1-115">Application</span><span class="sxs-lookup"><span data-stu-id="446d1-115">Application</span></span>                            | <span data-ttu-id="446d1-116">Application.ReadWrite.All e Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="446d1-116">Application.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="446d1-117">Os usuários podem criar credenciais para si mesmos.</span><span class="sxs-lookup"><span data-stu-id="446d1-117">Users can create credentials for themselves.</span></span> <span data-ttu-id="446d1-118">Os proprietários e administradores de entidades de serviço com as seguintes funções podem criar credenciais para qualquer usuário ou grupo: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span><span class="sxs-lookup"><span data-stu-id="446d1-118">Service principal owners and admins with the following roles can create credentials for any user or group: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span></span> <span data-ttu-id="446d1-119">Para saber mais, confira [Funções de diretório](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="446d1-119">To learn more, see [Directory roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="446d1-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="446d1-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/createPasswordSingleSignOnCredentials
```

## <a name="request-headers"></a><span data-ttu-id="446d1-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="446d1-121">Request headers</span></span>

| <span data-ttu-id="446d1-122">Nome</span><span class="sxs-lookup"><span data-stu-id="446d1-122">Name</span></span>          | <span data-ttu-id="446d1-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="446d1-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="446d1-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="446d1-124">Authorization</span></span> | <span data-ttu-id="446d1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="446d1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="446d1-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="446d1-127">Content-Type</span></span>  | <span data-ttu-id="446d1-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="446d1-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="446d1-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="446d1-130">Request body</span></span>

<span data-ttu-id="446d1-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="446d1-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="446d1-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="446d1-132">Parameter</span></span>    | <span data-ttu-id="446d1-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="446d1-133">Type</span></span>        | <span data-ttu-id="446d1-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="446d1-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="446d1-135">id</span><span class="sxs-lookup"><span data-stu-id="446d1-135">id</span></span>|<span data-ttu-id="446d1-136">String</span><span class="sxs-lookup"><span data-stu-id="446d1-136">String</span></span>|<span data-ttu-id="446d1-137">A ID do usuário ou grupo a que esse conjunto de credenciais pertence.</span><span class="sxs-lookup"><span data-stu-id="446d1-137">The ID of the user or group this credential set belongs to.</span></span>|
|<span data-ttu-id="446d1-138">credenciais</span><span class="sxs-lookup"><span data-stu-id="446d1-138">credentials</span></span>|<span data-ttu-id="446d1-139">[coleção credential](../resources/credential.md)</span><span class="sxs-lookup"><span data-stu-id="446d1-139">[credential](../resources/credential.md) collection</span></span>|<span data-ttu-id="446d1-140">Uma lista de objetos de credencial que definem o fluxo de login completo.</span><span class="sxs-lookup"><span data-stu-id="446d1-140">A list of credential objects that define the complete sign in flow.</span></span>|

## <a name="response"></a><span data-ttu-id="446d1-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="446d1-141">Response</span></span>

<span data-ttu-id="446d1-142">Se tiver êxito, este método retornará um código de resposta e um `200 OK` novo [objeto passwordSingleSignOnCredentialSet](../resources/passwordsinglesignoncredentialset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="446d1-142">If successful, this method returns a `200 OK` response code and a new [passwordSingleSignOnCredentialSet](../resources/passwordsinglesignoncredentialset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="446d1-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="446d1-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="446d1-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="446d1-144">Request</span></span>

<span data-ttu-id="446d1-145">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="446d1-145">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="446d1-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="446d1-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="446d1-147">C#</span><span class="sxs-lookup"><span data-stu-id="446d1-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-createpasswordsinglesignoncredentials-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="446d1-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="446d1-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-createpasswordsinglesignoncredentials-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="446d1-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="446d1-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-createpasswordsinglesignoncredentials-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="446d1-150">Java</span><span class="sxs-lookup"><span data-stu-id="446d1-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-createpasswordsinglesignoncredentials-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="446d1-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="446d1-151">Response</span></span>

<span data-ttu-id="446d1-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="446d1-152">The following is an example of the response.</span></span>

> <span data-ttu-id="446d1-153">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="446d1-153">**Note:** The response object shown here might be shortened for readability.</span></span>

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
