---
title: 'servicePrincipalName: createPasswordSingleSignOnCredentials'
description: Criar credenciais de logon único usando uma senha para um usuário ou grupo.
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5e8af42e62003b8aed9000efd2fa6de635c8bb67
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2019
ms.locfileid: "38658825"
---
# <a name="serviceprincipal-createpasswordsinglesignoncredentials"></a><span data-ttu-id="0ec2f-103">servicePrincipalName: createPasswordSingleSignOnCredentials</span><span class="sxs-lookup"><span data-stu-id="0ec2f-103">servicePrincipal: createPasswordSingleSignOnCredentials</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ec2f-104">Criar credenciais de logon único usando uma senha para um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="0ec2f-104">Create single sign-on credentials using a password for a user or group.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ec2f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0ec2f-105">Permissions</span></span>

<span data-ttu-id="0ec2f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ec2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0ec2f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ec2f-108">Permission type</span></span>                        | <span data-ttu-id="0ec2f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0ec2f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0ec2f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ec2f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0ec2f-111">Application. ReadWrite. All (também precisa Directory. Read. All), Directory. AccessAsUser. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0ec2f-111">Application.ReadWrite.All (also needs Directory.Read.All), Directory.AccessAsUser.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="0ec2f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ec2f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ec2f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ec2f-113">Not supported.</span></span> |
| <span data-ttu-id="0ec2f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ec2f-114">Application</span></span>                            | <span data-ttu-id="0ec2f-115">Application. ReadWrite. All (também precisa Directory. Read. All), Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0ec2f-115">Application.ReadWrite.All (also needs Directory.Read.All), Directory.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="0ec2f-116">Os usuários podem criar credenciais para si mesmos.</span><span class="sxs-lookup"><span data-stu-id="0ec2f-116">Users can create credentials for themselves.</span></span> <span data-ttu-id="0ec2f-117">Os proprietários e administradores da entidade de serviço com as seguintes funções podem criar credenciais para qualquer usuário ou grupo: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span><span class="sxs-lookup"><span data-stu-id="0ec2f-117">Service principal owners and admins with the following roles can create credentials for any user or group: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span></span> <span data-ttu-id="0ec2f-118">Para saber mais, confira [funções de diretório](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="0ec2f-118">To learn more, see [Directory roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="0ec2f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ec2f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/createPasswordSingleSignOnCredentials
```

## <a name="request-headers"></a><span data-ttu-id="0ec2f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ec2f-120">Request headers</span></span>

| <span data-ttu-id="0ec2f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0ec2f-121">Name</span></span>          | <span data-ttu-id="0ec2f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ec2f-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0ec2f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ec2f-123">Authorization</span></span> | <span data-ttu-id="0ec2f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ec2f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0ec2f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0ec2f-126">Content-Type</span></span>  | <span data-ttu-id="0ec2f-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ec2f-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0ec2f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ec2f-129">Request body</span></span>

<span data-ttu-id="0ec2f-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ec2f-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0ec2f-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0ec2f-131">Parameter</span></span>    | <span data-ttu-id="0ec2f-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ec2f-132">Type</span></span>        | <span data-ttu-id="0ec2f-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ec2f-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0ec2f-134">id</span><span class="sxs-lookup"><span data-stu-id="0ec2f-134">id</span></span>|<span data-ttu-id="0ec2f-135">String</span><span class="sxs-lookup"><span data-stu-id="0ec2f-135">String</span></span>|<span data-ttu-id="0ec2f-136">A ID do usuário ou grupo ao qual esse conjunto de credenciais pertence.</span><span class="sxs-lookup"><span data-stu-id="0ec2f-136">The ID of the user or group this credential set belongs to.</span></span>|
|<span data-ttu-id="0ec2f-137">las</span><span class="sxs-lookup"><span data-stu-id="0ec2f-137">credentials</span></span>|<span data-ttu-id="0ec2f-138">coleção [Credential](../resources/credential.md)</span><span class="sxs-lookup"><span data-stu-id="0ec2f-138">[credential](../resources/credential.md) collection</span></span>|<span data-ttu-id="0ec2f-139">Uma lista de objetos de credencial que definem o fluxo de entrada completo.</span><span class="sxs-lookup"><span data-stu-id="0ec2f-139">A list of credential objects that define the complete sign in flow.</span></span>|

## <a name="response"></a><span data-ttu-id="0ec2f-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ec2f-140">Response</span></span>

<span data-ttu-id="0ec2f-141">Se tiver êxito, este método retornará `200 OK` um código de resposta e um novo objeto [passwordSingleSignOnCredentialSet](../resources/passwordsinglesignoncredentialset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ec2f-141">If successful, this method returns a `200 OK` response code and a new [passwordSingleSignOnCredentialSet](../resources/passwordsinglesignoncredentialset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0ec2f-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0ec2f-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0ec2f-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ec2f-143">Request</span></span>

<span data-ttu-id="0ec2f-144">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ec2f-144">The following is an example of a request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0ec2f-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ec2f-145">Response</span></span>

<span data-ttu-id="0ec2f-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0ec2f-146">The following is an example of the response.</span></span>

> <span data-ttu-id="0ec2f-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0ec2f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
