---
title: Obter workforceIntegration
description: Recupere as propriedades e os relacionamentos do objeto workforceIntegration.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2b19f368f14f26679247f310c34c6f263e45aec6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037931"
---
# <a name="get-workforceintegration"></a><span data-ttu-id="51370-103">Obter workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="51370-103">Get workforceIntegration</span></span>

<span data-ttu-id="51370-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51370-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="51370-105">Recupere as propriedades e os relacionamentos de um objeto [workforceIntegration](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="51370-105">Retrieve the properties and relationships of a [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="51370-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="51370-106">Permissions</span></span>

<span data-ttu-id="51370-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51370-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="51370-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51370-109">Permission type</span></span>                        | <span data-ttu-id="51370-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="51370-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="51370-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51370-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="51370-112">WorkforceIntegration. Read. All, WorkforceIntegration. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="51370-112">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="51370-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51370-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51370-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51370-114">Not supported.</span></span> |
| <span data-ttu-id="51370-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51370-115">Application</span></span>                            | <span data-ttu-id="51370-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51370-116">Not supported.</span></span> |

> <span data-ttu-id="51370-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="51370-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="51370-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="51370-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="51370-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51370-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teamwork/workforceIntegrations/{workforceIntegrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51370-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="51370-120">Optional query parameters</span></span>

<span data-ttu-id="51370-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="51370-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="51370-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="51370-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="51370-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51370-123">Request headers</span></span>

| <span data-ttu-id="51370-124">Nome</span><span class="sxs-lookup"><span data-stu-id="51370-124">Name</span></span>      |<span data-ttu-id="51370-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="51370-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="51370-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="51370-126">Authorization</span></span> | <span data-ttu-id="51370-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51370-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="51370-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51370-129">Request body</span></span>

<span data-ttu-id="51370-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="51370-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51370-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="51370-131">Response</span></span>

<span data-ttu-id="51370-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [workforceIntegration](../resources/workforceintegration.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51370-132">If successful, this method returns a `200 OK` response code and the requested [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="51370-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="51370-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="51370-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51370-134">Request</span></span>

<span data-ttu-id="51370-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="51370-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="51370-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="51370-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workforceintegration"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations/{workforceintegrationid}
```
# <a name="c"></a>[<span data-ttu-id="51370-137">C#</span><span class="sxs-lookup"><span data-stu-id="51370-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51370-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51370-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51370-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51370-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="51370-140">Java</span><span class="sxs-lookup"><span data-stu-id="51370-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workforceintegration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="51370-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="51370-141">Response</span></span>

<span data-ttu-id="51370-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="51370-142">The following is an example of the response.</span></span>

> <span data-ttu-id="51370-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51370-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "displayName": "KronosWorkforceIntegration",
  "apiVersion": 1,
  "isActive": true,
  "encryption": {
    "protocol": "sharedSecret",
    "secret": null
  },
  "url": "https://contosoWorkforceIntegration.com/Contoso/",
  "supportedEntities": "shift"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get workforceIntegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

