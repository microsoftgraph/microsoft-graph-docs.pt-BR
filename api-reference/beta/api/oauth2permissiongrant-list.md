---
title: Listar oAuth2PermissionGrants
description: Recupere uma lista de objetos oauth2PermissionGrant, representando as autorizações de permissão delegadas.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 2b6ecf8c40f4f9a41608ef7f6edf588c1032839c
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845495"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="02744-103">List oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="02744-103">List oauth2PermissionGrants</span></span>

<span data-ttu-id="02744-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02744-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02744-105">Recupere uma lista de objetos [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) , representando as permissões delegadas que foram concedidas para que os aplicativos clientes acessem APIs em nome de usuários conectados.</span><span class="sxs-lookup"><span data-stu-id="02744-105">Retrieve a list of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects, representing delegated permissions which have been granted for client applications to access APIs on behalf of signed-in users.</span></span>

## <a name="permissions"></a><span data-ttu-id="02744-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="02744-106">Permissions</span></span>

<span data-ttu-id="02744-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02744-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02744-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02744-109">Permission type</span></span>      | <span data-ttu-id="02744-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02744-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02744-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02744-111">Delegated (work or school account)</span></span> | <span data-ttu-id="02744-112">Directory. Read. All, DelegatedPermissionGrant. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="02744-112">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="02744-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02744-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02744-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02744-114">Not supported.</span></span>    |
|<span data-ttu-id="02744-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02744-115">Application</span></span> | <span data-ttu-id="02744-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02744-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="02744-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02744-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /oauth2PermissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="02744-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="02744-118">Optional query parameters</span></span>

<span data-ttu-id="02744-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="02744-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="02744-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02744-120">Request headers</span></span>

| <span data-ttu-id="02744-121">Nome</span><span class="sxs-lookup"><span data-stu-id="02744-121">Name</span></span> | <span data-ttu-id="02744-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="02744-122">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="02744-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="02744-123">Authorization</span></span>  | <span data-ttu-id="02744-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02744-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="02744-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02744-126">Request body</span></span>

<span data-ttu-id="02744-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="02744-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02744-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="02744-128">Response</span></span>

<span data-ttu-id="02744-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02744-129">If successful, this method returns a `200 OK` response code and collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02744-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02744-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="02744-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02744-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="02744-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="02744-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_oauth2permissiongrants"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/oauth2PermissionGrants
```
# <a name="c"></a>[<span data-ttu-id="02744-133">C#</span><span class="sxs-lookup"><span data-stu-id="02744-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-oauth2permissiongrants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02744-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02744-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-oauth2permissiongrants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02744-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02744-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-oauth2permissiongrants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="02744-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="02744-136">Response</span></span>

> <span data-ttu-id="02744-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02744-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "value": [
    {
      "id": "id-value",
      "clientId": "clientId-value",
      "consentType": "consentType-value",
      "principalId": "principalId-value",
      "resourceId": "resourceId-value",
      "scope": "scope-value",
      "startTime": "datetime-value",
      "expiryTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List oauth2PermissionGrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
