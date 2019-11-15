---
title: 'servicePrincipalName: getPasswordSingleSignOnCredentials'
description: Obter uma lista de credenciais de logon único usando uma senha para um usuário ou grupo.
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ca4c93c944912a0c40ed356a6e6f371e21bb4f0a
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2019
ms.locfileid: "38658741"
---
# <a name="serviceprincipal-getpasswordsinglesignoncredentials"></a><span data-ttu-id="846ec-103">servicePrincipalName: getPasswordSingleSignOnCredentials</span><span class="sxs-lookup"><span data-stu-id="846ec-103">servicePrincipal: getPasswordSingleSignOnCredentials</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="846ec-104">Obter uma lista de credenciais de logon único usando uma senha para um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="846ec-104">Get a list of single sign-on credentials using a password for a user or group.</span></span>

## <a name="permissions"></a><span data-ttu-id="846ec-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="846ec-105">Permissions</span></span>

<span data-ttu-id="846ec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="846ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="846ec-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="846ec-108">Permission type</span></span>                        | <span data-ttu-id="846ec-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="846ec-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="846ec-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="846ec-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="846ec-111">Application. ReadWrite. All (também precisa Directory. Read. All), Directory. AccessAsUser. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="846ec-111">Application.ReadWrite.All (also needs Directory.Read.All), Directory.AccessAsUser.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="846ec-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="846ec-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="846ec-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="846ec-113">Not supported.</span></span> |
| <span data-ttu-id="846ec-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="846ec-114">Application</span></span>                            | <span data-ttu-id="846ec-115">Application. ReadWrite. All (também precisa Directory. Read. All), Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="846ec-115">Application.ReadWrite.All (also needs Directory.Read.All), Directory.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="846ec-116">Os usuários podem criar credenciais para si mesmos.</span><span class="sxs-lookup"><span data-stu-id="846ec-116">Users can create credentials for themselves.</span></span> <span data-ttu-id="846ec-117">Os proprietários e administradores da entidade de serviço com as seguintes funções podem criar credenciais para qualquer usuário ou grupo: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span><span class="sxs-lookup"><span data-stu-id="846ec-117">Service principal owners and admins with the following roles can create credentials for any user or group: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span></span> <span data-ttu-id="846ec-118">Para saber mais, confira [funções de diretório](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="846ec-118">To learn more, see [Directory roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="846ec-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="846ec-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/getPasswordSingleSignOnCredentials
```

## <a name="request-headers"></a><span data-ttu-id="846ec-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="846ec-120">Request headers</span></span>

| <span data-ttu-id="846ec-121">Nome</span><span class="sxs-lookup"><span data-stu-id="846ec-121">Name</span></span>          | <span data-ttu-id="846ec-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="846ec-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="846ec-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="846ec-123">Authorization</span></span> | <span data-ttu-id="846ec-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="846ec-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="846ec-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="846ec-126">Content-Type</span></span>  | <span data-ttu-id="846ec-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="846ec-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="846ec-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="846ec-129">Request body</span></span>

<span data-ttu-id="846ec-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="846ec-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="846ec-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="846ec-131">Parameter</span></span>    | <span data-ttu-id="846ec-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="846ec-132">Type</span></span>        | <span data-ttu-id="846ec-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="846ec-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="846ec-134">id</span><span class="sxs-lookup"><span data-stu-id="846ec-134">id</span></span>|<span data-ttu-id="846ec-135">String</span><span class="sxs-lookup"><span data-stu-id="846ec-135">String</span></span>|<span data-ttu-id="846ec-136">A ID do usuário ou grupo ao qual esse conjunto de credenciais pertence.</span><span class="sxs-lookup"><span data-stu-id="846ec-136">The ID of the user or group this credential set belongs to.</span></span>|

## <a name="response"></a><span data-ttu-id="846ec-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="846ec-137">Response</span></span>

<span data-ttu-id="846ec-138">Se tiver êxito, este método retornará `200 OK` um código de resposta e um novo objeto [passwordSingleSignOnCredentialSet](../resources/passwordsinglesignoncredentialset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="846ec-138">If successful, this method returns a `200 OK` response code and a new [passwordSingleSignOnCredentialSet](../resources/passwordsinglesignoncredentialset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="846ec-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="846ec-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="846ec-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="846ec-140">Request</span></span>

<span data-ttu-id="846ec-141">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="846ec-141">The following is an example of a request.</span></span>
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

### <a name="response"></a><span data-ttu-id="846ec-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="846ec-142">Response</span></span>

<span data-ttu-id="846ec-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="846ec-143">The following is an example of the response.</span></span>

> <span data-ttu-id="846ec-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="846ec-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
