---
title: 'servicePrincipalName: listar oAuth2Permissiongrants'
description: Recupere uma lista de objetos oAuth2Permissiongrant.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 089357ff1ba739815a03460bae4a0cdcd78c296d
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219057"
---
# <a name="serviceprincipal-list-oauth2permissiongrants"></a><span data-ttu-id="7e6a4-103">servicePrincipalName: listar oAuth2Permissiongrants</span><span class="sxs-lookup"><span data-stu-id="7e6a4-103">servicePrincipal: List oAuth2Permissiongrants</span></span>

<span data-ttu-id="7e6a4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e6a4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e6a4-105">Recupere uma lista de objetos oAuth2Permissiongrant.</span><span class="sxs-lookup"><span data-stu-id="7e6a4-105">Retrieve a list of oAuth2Permissiongrant objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e6a4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7e6a4-106">Permissions</span></span>
<span data-ttu-id="7e6a4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e6a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e6a4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e6a4-109">Permission type</span></span>      | <span data-ttu-id="7e6a4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7e6a4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e6a4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e6a4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7e6a4-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7e6a4-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7e6a4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e6a4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e6a4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e6a4-114">Not supported.</span></span>    |
|<span data-ttu-id="7e6a4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e6a4-115">Application</span></span> | <span data-ttu-id="7e6a4-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e6a4-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e6a4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e6a4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/oAuth2Permissiongrants
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7e6a4-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7e6a4-118">Optional query parameters</span></span>
<span data-ttu-id="7e6a4-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7e6a4-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7e6a4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7e6a4-120">Request headers</span></span>
| <span data-ttu-id="7e6a4-121">Nome</span><span class="sxs-lookup"><span data-stu-id="7e6a4-121">Name</span></span>       | <span data-ttu-id="7e6a4-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e6a4-122">Type</span></span> | <span data-ttu-id="7e6a4-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e6a4-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7e6a4-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e6a4-124">Authorization</span></span>  | <span data-ttu-id="7e6a4-125">string</span><span class="sxs-lookup"><span data-stu-id="7e6a4-125">string</span></span>  | <span data-ttu-id="7e6a4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e6a4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e6a4-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e6a4-128">Request body</span></span>
<span data-ttu-id="7e6a4-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7e6a4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e6a4-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e6a4-130">Response</span></span>

<span data-ttu-id="7e6a4-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e6a4-131">If successful, this method returns a `200 OK` response code and collection of [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7e6a4-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7e6a4-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7e6a4-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e6a4-133">Request</span></span>
<span data-ttu-id="7e6a4-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7e6a4-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7e6a4-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e6a4-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_oAuth2Permissiongrants"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/oAuth2Permissiongrants
```
# <a name="c"></a>[<span data-ttu-id="7e6a4-136">C#</span><span class="sxs-lookup"><span data-stu-id="7e6a4-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-oauth2permissiongrants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7e6a4-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e6a4-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-oauth2permissiongrants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7e6a4-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e6a4-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-oauth2permissiongrants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7e6a4-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e6a4-139">Response</span></span>
<span data-ttu-id="7e6a4-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7e6a4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 253

{
  "value": [
    {
      "clientId": "clientId-value",
      "consentType": "consentType-value",
      "expiryTime": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "principalId": "principalId-value",
      "resourceId": "resourceId-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List oAuth2Permissiongrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
