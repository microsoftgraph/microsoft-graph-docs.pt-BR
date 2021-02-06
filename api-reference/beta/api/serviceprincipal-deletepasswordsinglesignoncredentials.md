---
title: 'servicePrincipal: deletePasswordSingleSignOnCredentials'
description: Exclua as credenciais de login único usando uma senha para um usuário ou grupo.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 249f5022d3a7dd9170ab35e66c1ecf0e7c0dd99e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131947"
---
# <a name="serviceprincipal-deletepasswordsinglesignoncredentials"></a><span data-ttu-id="1cfa7-103">servicePrincipal: deletePasswordSingleSignOnCredentials</span><span class="sxs-lookup"><span data-stu-id="1cfa7-103">servicePrincipal: deletePasswordSingleSignOnCredentials</span></span>

<span data-ttu-id="1cfa7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1cfa7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1cfa7-105">Exclua as credenciais de login único usando uma senha para um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="1cfa7-105">Delete single sign-on credentials using a password for a user or group.</span></span>

## <a name="permissions"></a><span data-ttu-id="1cfa7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1cfa7-106">Permissions</span></span>

<span data-ttu-id="1cfa7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cfa7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1cfa7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1cfa7-109">Permission type</span></span>                        | <span data-ttu-id="1cfa7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1cfa7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1cfa7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1cfa7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1cfa7-112">Application.ReadWrite.All e Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1cfa7-112">Application.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="1cfa7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1cfa7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1cfa7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1cfa7-114">Not supported.</span></span> |
| <span data-ttu-id="1cfa7-115">Application</span><span class="sxs-lookup"><span data-stu-id="1cfa7-115">Application</span></span>                            | <span data-ttu-id="1cfa7-116">Application.ReadWrite.All e Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cfa7-116">Application.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="1cfa7-117">Os usuários podem criar credenciais para si próprios.</span><span class="sxs-lookup"><span data-stu-id="1cfa7-117">Users can create credentials for themselves.</span></span> <span data-ttu-id="1cfa7-118">Os proprietários e administradores da entidade de serviço com as seguintes funções podem criar credenciais para qualquer usuário ou grupo: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span><span class="sxs-lookup"><span data-stu-id="1cfa7-118">Service principal owners and admins with the following roles can create credentials for any user or group: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span></span> <span data-ttu-id="1cfa7-119">Para saber mais, consulte Funções [de diretório.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="1cfa7-119">To learn more, see [Directory roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="1cfa7-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1cfa7-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/deletePasswordSingleSignOnCredentials
```

## <a name="request-headers"></a><span data-ttu-id="1cfa7-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1cfa7-121">Request headers</span></span>

| <span data-ttu-id="1cfa7-122">Nome</span><span class="sxs-lookup"><span data-stu-id="1cfa7-122">Name</span></span>          | <span data-ttu-id="1cfa7-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cfa7-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1cfa7-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1cfa7-124">Authorization</span></span> | <span data-ttu-id="1cfa7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1cfa7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1cfa7-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1cfa7-127">Content-Type</span></span>  | <span data-ttu-id="1cfa7-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1cfa7-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1cfa7-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1cfa7-130">Request body</span></span>

<span data-ttu-id="1cfa7-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1cfa7-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1cfa7-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1cfa7-132">Parameter</span></span>    | <span data-ttu-id="1cfa7-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="1cfa7-133">Type</span></span>        | <span data-ttu-id="1cfa7-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cfa7-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1cfa7-135">id</span><span class="sxs-lookup"><span data-stu-id="1cfa7-135">id</span></span>|<span data-ttu-id="1cfa7-136">String</span><span class="sxs-lookup"><span data-stu-id="1cfa7-136">String</span></span>|<span data-ttu-id="1cfa7-137">A ID do usuário ou grupo ao que esse conjunto de credenciais pertence.</span><span class="sxs-lookup"><span data-stu-id="1cfa7-137">The ID of the user or group this credential set belongs to.</span></span>|

## <a name="response"></a><span data-ttu-id="1cfa7-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cfa7-138">Response</span></span>

<span data-ttu-id="1cfa7-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1cfa7-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1cfa7-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1cfa7-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1cfa7-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1cfa7-142">Request</span></span>

<span data-ttu-id="1cfa7-143">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="1cfa7-143">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1cfa7-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="1cfa7-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1cfa7-145">C#</span><span class="sxs-lookup"><span data-stu-id="1cfa7-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-deletepasswordsinglesignoncredentials-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1cfa7-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1cfa7-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-deletepasswordsinglesignoncredentials-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1cfa7-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1cfa7-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-deletepasswordsinglesignoncredentials-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1cfa7-148">Java</span><span class="sxs-lookup"><span data-stu-id="1cfa7-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-deletepasswordsinglesignoncredentials-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1cfa7-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cfa7-149">Response</span></span>

<span data-ttu-id="1cfa7-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1cfa7-150">The following is an example of the response.</span></span>
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
