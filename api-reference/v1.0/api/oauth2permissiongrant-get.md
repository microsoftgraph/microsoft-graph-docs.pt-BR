---
title: Obter um oAuth2PermissionGrant
description: Recupere as propriedades e os relacionamentos de um único oAuth2PermissionGrant, representando uma concessão de permissão delegada.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: a4e6626bef1969822954ddb889e33526cd09604f
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44288644"
---
# <a name="get-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="156a5-103">Obter uma concessão de permissão delegada (oAuth2PermissionGrant)</span><span class="sxs-lookup"><span data-stu-id="156a5-103">Get a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="156a5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="156a5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="156a5-105">Recupere as propriedades de um único [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).</span><span class="sxs-lookup"><span data-stu-id="156a5-105">Retrieve the properties of a single [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).</span></span>

<span data-ttu-id="156a5-106">Um **oAuth2PermissionGrant** representa permissões delegadas que foram concedidas para um aplicativo cliente acessar uma API em nome de um usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="156a5-106">An **oAuth2PermissionGrant** represents delegated permissions which have been granted for a client application to access an API on behalf of a signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="156a5-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="156a5-107">Permissions</span></span>

<span data-ttu-id="156a5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="156a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="156a5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="156a5-110">Permission type</span></span>      | <span data-ttu-id="156a5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="156a5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="156a5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="156a5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="156a5-113">Directory. Read. All, DelegatedPermissionGrant. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="156a5-113">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="156a5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="156a5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="156a5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="156a5-115">Not supported.</span></span>    |
|<span data-ttu-id="156a5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="156a5-116">Application</span></span> | <span data-ttu-id="156a5-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="156a5-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="156a5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="156a5-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /oauth2PermissionGrants/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="156a5-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="156a5-119">Optional query parameters</span></span>

<span data-ttu-id="156a5-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="156a5-120">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="156a5-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="156a5-121">Request headers</span></span>

| <span data-ttu-id="156a5-122">Nome</span><span class="sxs-lookup"><span data-stu-id="156a5-122">Name</span></span>       | <span data-ttu-id="156a5-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="156a5-123">Type</span></span> | <span data-ttu-id="156a5-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="156a5-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="156a5-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="156a5-125">Authorization</span></span>  | <span data-ttu-id="156a5-126">string</span><span class="sxs-lookup"><span data-stu-id="156a5-126">string</span></span>  | <span data-ttu-id="156a5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="156a5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="156a5-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="156a5-129">Request body</span></span>

<span data-ttu-id="156a5-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="156a5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="156a5-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="156a5-131">Response</span></span>

<span data-ttu-id="156a5-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="156a5-132">If successful, this method returns a `200 OK` response code and [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="156a5-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="156a5-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="156a5-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="156a5-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_oAuth2Permissiongrant"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/oauth2PermissionGrants/{id}
```

### <a name="response"></a><span data-ttu-id="156a5-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="156a5-135">Response</span></span>

> <span data-ttu-id="156a5-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="156a5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 200

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
  "description": "Get oAuth2PermissionGrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
