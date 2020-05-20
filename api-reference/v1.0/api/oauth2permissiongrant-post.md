---
title: Criar um oAuth2PermissionGrant
description: Crie um objeto oAuth2PermissionGrant, representando uma concessão de permissão delegada.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: d4d2e7c4b4bc114dac07515586f13f4cbaac738c
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44288640"
---
# <a name="create-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="2f33a-103">Criar uma concessão de permissão delegada (oAuth2PermissionGrant)</span><span class="sxs-lookup"><span data-stu-id="2f33a-103">Create a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="2f33a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f33a-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="2f33a-105">Criar uma concessão de permissão delegada.</span><span class="sxs-lookup"><span data-stu-id="2f33a-105">Create a delegated permission grant.</span></span> <span data-ttu-id="2f33a-106">Uma concessão de permissão delegada é representada por um objeto [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) .</span><span class="sxs-lookup"><span data-stu-id="2f33a-106">A delegated permission grant is represented by an [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object.</span></span>

<span data-ttu-id="2f33a-107">Uma concessão de permissão delegada autoriza uma entidade de serviço de cliente (representando um aplicativo cliente) para acessar uma entidade de serviço de recurso (representando uma API), em nome de um usuário conectado, para o nível de acesso limitado pelas permissões delegadas que foram concedidas.</span><span class="sxs-lookup"><span data-stu-id="2f33a-107">A delegated permission grant authorizes a client service principal (representing a client application) to access a resource service principal (representing an API), on behalf of a signed-in user, for the level of access limited by the delegated permissions which were granted.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f33a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="2f33a-108">Permissions</span></span>

<span data-ttu-id="2f33a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f33a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f33a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f33a-111">Permission type</span></span>      | <span data-ttu-id="2f33a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2f33a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f33a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f33a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2f33a-114">DelegatedPermissionGrant. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="2f33a-114">DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2f33a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f33a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f33a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f33a-116">Not supported.</span></span>    |
|<span data-ttu-id="2f33a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f33a-117">Application</span></span> | <span data-ttu-id="2f33a-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f33a-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f33a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f33a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /oauth2PermissionGrants
```

## <a name="request-headers"></a><span data-ttu-id="2f33a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f33a-120">Request headers</span></span>

| <span data-ttu-id="2f33a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="2f33a-121">Name</span></span>       | <span data-ttu-id="2f33a-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f33a-122">Type</span></span> | <span data-ttu-id="2f33a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f33a-123">Description</span></span> |
|:-----------|:------|:----------|
| <span data-ttu-id="2f33a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f33a-124">Authorization</span></span>  | <span data-ttu-id="2f33a-125">string</span><span class="sxs-lookup"><span data-stu-id="2f33a-125">string</span></span>  | <span data-ttu-id="2f33a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f33a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f33a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f33a-128">Request body</span></span>

<span data-ttu-id="2f33a-129">No corpo da solicitação, forneça uma representação JSON de um objeto [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) .</span><span class="sxs-lookup"><span data-stu-id="2f33a-129">In the request body, supply a JSON representation of an [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2f33a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f33a-130">Response</span></span>

<span data-ttu-id="2f33a-131">Se tiver êxito, este método retornará um código de resposta de série 200 e um novo objeto [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f33a-131">If successful, this method returns a 200-series response code and a new [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f33a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f33a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f33a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f33a-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "post_oAuth2PermissionGrant"
}-->

```http
POST https://graph.microsoft.com/v1.0/oauth2PermissionGrants
Content-Type: application/json
Content-Length: 30

{
  "clientId": "clientId-value",
  "consentType": "consentType-value",
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "scope": "scope-value"
}
```

### <a name="response"></a><span data-ttu-id="2f33a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f33a-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "id-value",
  "clientId": "clientId-value",
  "consentType": "consentType-value",
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "scope": "scope-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update oAuth2PermissionGrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
