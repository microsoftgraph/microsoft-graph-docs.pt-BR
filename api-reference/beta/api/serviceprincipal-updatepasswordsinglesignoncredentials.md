---
title: 'servicePrincipal: updatePasswordSingleSignOnCredentials'
description: Atualize as credenciais de login único usando uma senha para um usuário ou grupo.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 154e74f3cdf7ed8b0fd690bd4b5b6c476a787d30
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132108"
---
# <a name="serviceprincipal-updatepasswordsinglesignoncredentials"></a><span data-ttu-id="09d59-103">servicePrincipal: updatePasswordSingleSignOnCredentials</span><span class="sxs-lookup"><span data-stu-id="09d59-103">servicePrincipal: updatePasswordSingleSignOnCredentials</span></span>

<span data-ttu-id="09d59-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09d59-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09d59-105">Atualize as credenciais de login único usando uma senha para um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="09d59-105">Update single sign-on credentials using a password for a user or group.</span></span>

## <a name="permissions"></a><span data-ttu-id="09d59-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="09d59-106">Permissions</span></span>

<span data-ttu-id="09d59-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09d59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="09d59-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="09d59-109">Permission type</span></span>                        | <span data-ttu-id="09d59-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="09d59-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="09d59-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="09d59-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="09d59-112">Application.ReadWrite.All e Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="09d59-112">Application.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="09d59-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="09d59-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09d59-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09d59-114">Not supported.</span></span> |
| <span data-ttu-id="09d59-115">Application</span><span class="sxs-lookup"><span data-stu-id="09d59-115">Application</span></span>                            | <span data-ttu-id="09d59-116">Application.ReadWrite.All e Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09d59-116">Application.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="09d59-117">Os usuários podem criar credenciais para si próprios.</span><span class="sxs-lookup"><span data-stu-id="09d59-117">Users can create credentials for themselves.</span></span> <span data-ttu-id="09d59-118">Os proprietários e administradores da entidade de serviço com as seguintes funções podem criar credenciais para qualquer usuário ou grupo: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span><span class="sxs-lookup"><span data-stu-id="09d59-118">Service principal owners and admins with the following roles can create credentials for any user or group: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span></span> <span data-ttu-id="09d59-119">Para saber mais, consulte Funções [de diretório.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="09d59-119">To learn more, see [Directory roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="09d59-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="09d59-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/updatePasswordSingleSignOnCredentials
```

## <a name="request-headers"></a><span data-ttu-id="09d59-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="09d59-121">Request headers</span></span>

| <span data-ttu-id="09d59-122">Nome</span><span class="sxs-lookup"><span data-stu-id="09d59-122">Name</span></span>          | <span data-ttu-id="09d59-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="09d59-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="09d59-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="09d59-124">Authorization</span></span> | <span data-ttu-id="09d59-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09d59-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="09d59-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="09d59-127">Content-Type</span></span>  | <span data-ttu-id="09d59-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09d59-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="09d59-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="09d59-130">Request body</span></span>

<span data-ttu-id="09d59-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="09d59-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="09d59-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="09d59-132">Parameter</span></span>    | <span data-ttu-id="09d59-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="09d59-133">Type</span></span>        | <span data-ttu-id="09d59-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="09d59-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="09d59-135">id</span><span class="sxs-lookup"><span data-stu-id="09d59-135">id</span></span>|<span data-ttu-id="09d59-136">String</span><span class="sxs-lookup"><span data-stu-id="09d59-136">String</span></span>|<span data-ttu-id="09d59-137">A ID do usuário ou grupo ao que esse conjunto de credenciais pertence.</span><span class="sxs-lookup"><span data-stu-id="09d59-137">The ID of the user or group this credential set belongs to.</span></span>|
|<span data-ttu-id="09d59-138">credenciais</span><span class="sxs-lookup"><span data-stu-id="09d59-138">credentials</span></span>|<span data-ttu-id="09d59-139">[coleção de](../resources/credential.md) credenciais</span><span class="sxs-lookup"><span data-stu-id="09d59-139">[credential](../resources/credential.md) collection</span></span>|<span data-ttu-id="09d59-140">Uma lista de objetos de credencial que definem o fluxo de login completo.</span><span class="sxs-lookup"><span data-stu-id="09d59-140">A list of credential objects that define the complete sign in flow.</span></span>|

## <a name="response"></a><span data-ttu-id="09d59-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="09d59-141">Response</span></span>

<span data-ttu-id="09d59-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="09d59-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="09d59-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="09d59-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="09d59-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09d59-145">Request</span></span>

<span data-ttu-id="09d59-146">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="09d59-146">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="09d59-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="09d59-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="09d59-148">C#</span><span class="sxs-lookup"><span data-stu-id="09d59-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-updatepasswordsinglesignoncredentials-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="09d59-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="09d59-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-updatepasswordsinglesignoncredentials-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="09d59-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="09d59-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-updatepasswordsinglesignoncredentials-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="09d59-151">Java</span><span class="sxs-lookup"><span data-stu-id="09d59-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-updatepasswordsinglesignoncredentials-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="09d59-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="09d59-152">Response</span></span>

<span data-ttu-id="09d59-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="09d59-153">The following is an example of the response.</span></span>
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
