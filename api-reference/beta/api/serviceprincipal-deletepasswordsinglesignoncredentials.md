---
title: 'servicePrincipalName: deletePasswordSingleSignOnCredentials'
description: Exclua as credenciais de logon único usando uma senha para um usuário ou grupo.
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9b39bf30f4a6a943a21db012d0201812681dd9ee
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2019
ms.locfileid: "38658818"
---
# <a name="serviceprincipal-deletepasswordsinglesignoncredentials"></a><span data-ttu-id="19fe2-103">servicePrincipalName: deletePasswordSingleSignOnCredentials</span><span class="sxs-lookup"><span data-stu-id="19fe2-103">servicePrincipal: deletePasswordSingleSignOnCredentials</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19fe2-104">Exclua as credenciais de logon único usando uma senha para um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="19fe2-104">Delete single sign-on credentials using a password for a user or group.</span></span>

## <a name="permissions"></a><span data-ttu-id="19fe2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="19fe2-105">Permissions</span></span>

<span data-ttu-id="19fe2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19fe2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="19fe2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19fe2-108">Permission type</span></span>                        | <span data-ttu-id="19fe2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="19fe2-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="19fe2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19fe2-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="19fe2-111">Application. ReadWrite. All (também precisa Directory. Read. All), Directory. AccessAsUser. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="19fe2-111">Application.ReadWrite.All (also needs Directory.Read.All), Directory.AccessAsUser.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="19fe2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19fe2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19fe2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19fe2-113">Not supported.</span></span> |
| <span data-ttu-id="19fe2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19fe2-114">Application</span></span>                            | <span data-ttu-id="19fe2-115">Application. ReadWrite. All (também precisa Directory. Read. All), Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="19fe2-115">Application.ReadWrite.All (also needs Directory.Read.All), Directory.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="19fe2-116">Os usuários podem criar credenciais para si mesmos.</span><span class="sxs-lookup"><span data-stu-id="19fe2-116">Users can create credentials for themselves.</span></span> <span data-ttu-id="19fe2-117">Os proprietários e administradores da entidade de serviço com as seguintes funções podem criar credenciais para qualquer usuário ou grupo: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span><span class="sxs-lookup"><span data-stu-id="19fe2-117">Service principal owners and admins with the following roles can create credentials for any user or group: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span></span> <span data-ttu-id="19fe2-118">Para saber mais, confira [funções de diretório](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="19fe2-118">To learn more, see [Directory roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="19fe2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19fe2-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/deletePasswordSingleSignOnCredentials
```

## <a name="request-headers"></a><span data-ttu-id="19fe2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19fe2-120">Request headers</span></span>

| <span data-ttu-id="19fe2-121">Nome</span><span class="sxs-lookup"><span data-stu-id="19fe2-121">Name</span></span>          | <span data-ttu-id="19fe2-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="19fe2-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="19fe2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="19fe2-123">Authorization</span></span> | <span data-ttu-id="19fe2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19fe2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="19fe2-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="19fe2-126">Content-Type</span></span>  | <span data-ttu-id="19fe2-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19fe2-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="19fe2-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19fe2-129">Request body</span></span>

<span data-ttu-id="19fe2-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="19fe2-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="19fe2-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="19fe2-131">Parameter</span></span>    | <span data-ttu-id="19fe2-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="19fe2-132">Type</span></span>        | <span data-ttu-id="19fe2-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="19fe2-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="19fe2-134">id</span><span class="sxs-lookup"><span data-stu-id="19fe2-134">id</span></span>|<span data-ttu-id="19fe2-135">String</span><span class="sxs-lookup"><span data-stu-id="19fe2-135">String</span></span>|<span data-ttu-id="19fe2-136">A ID do usuário ou grupo ao qual esse conjunto de credenciais pertence.</span><span class="sxs-lookup"><span data-stu-id="19fe2-136">The ID of the user or group this credential set belongs to.</span></span>|

## <a name="response"></a><span data-ttu-id="19fe2-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="19fe2-137">Response</span></span>

<span data-ttu-id="19fe2-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19fe2-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="19fe2-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="19fe2-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="19fe2-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19fe2-141">Request</span></span>

<span data-ttu-id="19fe2-142">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="19fe2-142">The following is an example of a request.</span></span>
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

### <a name="response"></a><span data-ttu-id="19fe2-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="19fe2-143">Response</span></span>

<span data-ttu-id="19fe2-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="19fe2-144">The following is an example of the response.</span></span>
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
