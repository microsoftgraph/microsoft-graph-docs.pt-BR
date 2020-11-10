---
title: 'servicePrincipalName: deletePasswordSingleSignOnCredentials'
description: Exclua as credenciais de logon único usando uma senha para um usuário ou grupo.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 75f33809759e6325c3767ee2c7dec1f6212d8883
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969608"
---
# <a name="serviceprincipal-deletepasswordsinglesignoncredentials"></a><span data-ttu-id="05f2a-103">servicePrincipalName: deletePasswordSingleSignOnCredentials</span><span class="sxs-lookup"><span data-stu-id="05f2a-103">servicePrincipal: deletePasswordSingleSignOnCredentials</span></span>

<span data-ttu-id="05f2a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05f2a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05f2a-105">Exclua as credenciais de logon único usando uma senha para um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="05f2a-105">Delete single sign-on credentials using a password for a user or group.</span></span>

## <a name="permissions"></a><span data-ttu-id="05f2a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="05f2a-106">Permissions</span></span>

<span data-ttu-id="05f2a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05f2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="05f2a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05f2a-109">Permission type</span></span>                        | <span data-ttu-id="05f2a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="05f2a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="05f2a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05f2a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="05f2a-112">Application. ReadWrite. All e Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="05f2a-112">Application.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="05f2a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05f2a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05f2a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05f2a-114">Not supported.</span></span> |
| <span data-ttu-id="05f2a-115">Application</span><span class="sxs-lookup"><span data-stu-id="05f2a-115">Application</span></span>                            | <span data-ttu-id="05f2a-116">Application. ReadWrite. All e Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="05f2a-116">Application.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="05f2a-117">Os usuários podem criar credenciais para si mesmos.</span><span class="sxs-lookup"><span data-stu-id="05f2a-117">Users can create credentials for themselves.</span></span> <span data-ttu-id="05f2a-118">Os proprietários e administradores da entidade de serviço com as seguintes funções podem criar credenciais para qualquer usuário ou grupo: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span><span class="sxs-lookup"><span data-stu-id="05f2a-118">Service principal owners and admins with the following roles can create credentials for any user or group: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span></span> <span data-ttu-id="05f2a-119">Para saber mais, confira [funções de diretório](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="05f2a-119">To learn more, see [Directory roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="05f2a-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05f2a-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/deletePasswordSingleSignOnCredentials
```

## <a name="request-headers"></a><span data-ttu-id="05f2a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05f2a-121">Request headers</span></span>

| <span data-ttu-id="05f2a-122">Nome</span><span class="sxs-lookup"><span data-stu-id="05f2a-122">Name</span></span>          | <span data-ttu-id="05f2a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="05f2a-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="05f2a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="05f2a-124">Authorization</span></span> | <span data-ttu-id="05f2a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05f2a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="05f2a-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="05f2a-127">Content-Type</span></span>  | <span data-ttu-id="05f2a-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05f2a-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="05f2a-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05f2a-130">Request body</span></span>

<span data-ttu-id="05f2a-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="05f2a-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="05f2a-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="05f2a-132">Parameter</span></span>    | <span data-ttu-id="05f2a-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="05f2a-133">Type</span></span>        | <span data-ttu-id="05f2a-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="05f2a-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="05f2a-135">id</span><span class="sxs-lookup"><span data-stu-id="05f2a-135">id</span></span>|<span data-ttu-id="05f2a-136">String</span><span class="sxs-lookup"><span data-stu-id="05f2a-136">String</span></span>|<span data-ttu-id="05f2a-137">A ID do usuário ou grupo ao qual esse conjunto de credenciais pertence.</span><span class="sxs-lookup"><span data-stu-id="05f2a-137">The ID of the user or group this credential set belongs to.</span></span>|

## <a name="response"></a><span data-ttu-id="05f2a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="05f2a-138">Response</span></span>

<span data-ttu-id="05f2a-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05f2a-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="05f2a-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="05f2a-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="05f2a-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05f2a-142">Request</span></span>

<span data-ttu-id="05f2a-143">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="05f2a-143">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="05f2a-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="05f2a-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_deletepasswordsinglesignoncredentials"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/deletePasswordSingleSignOnCredentials
Content-type: application/json

{
  "id": "5793aa3b-cca9-4794-679a240f8b58"
}
```
# <a name="c"></a>[<span data-ttu-id="05f2a-145">C#</span><span class="sxs-lookup"><span data-stu-id="05f2a-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-deletepasswordsinglesignoncredentials-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="05f2a-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="05f2a-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-deletepasswordsinglesignoncredentials-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="05f2a-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="05f2a-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-deletepasswordsinglesignoncredentials-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="05f2a-148">Java</span><span class="sxs-lookup"><span data-stu-id="05f2a-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-deletepasswordsinglesignoncredentials-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="05f2a-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="05f2a-149">Response</span></span>

<span data-ttu-id="05f2a-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="05f2a-150">The following is an example of the response.</span></span>
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
  "description": "servicePrincipal: deletePasswordSingleSignOnCredentials",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
