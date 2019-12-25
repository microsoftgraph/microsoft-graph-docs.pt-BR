---
title: Listar accessPackageResourceRequests
description: Recupere uma lista de objetos accessPackageResourceRequest.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c9cc83456021c3e10db5fbe1666d7696e8270507
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871707"
---
# <a name="list-accesspackageresourcerequests"></a><span data-ttu-id="5728c-103">Listar accessPackageResourceRequests</span><span class="sxs-lookup"><span data-stu-id="5728c-103">List accessPackageResourceRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5728c-104">Recupere uma lista de objetos [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="5728c-104">Retrieve a list of [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="5728c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5728c-105">Permissions</span></span>

<span data-ttu-id="5728c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5728c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5728c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5728c-108">Permission type</span></span>                        | <span data-ttu-id="5728c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5728c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5728c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5728c-110">Delegated (work or school account)</span></span>     |  <span data-ttu-id="5728c-111">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5728c-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="5728c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5728c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5728c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5728c-113">Not supported.</span></span> |
| <span data-ttu-id="5728c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5728c-114">Application</span></span>                            | <span data-ttu-id="5728c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5728c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5728c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5728c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageResourceRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5728c-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5728c-117">Optional query parameters</span></span>

<span data-ttu-id="5728c-118">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5728c-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5728c-119">Por exemplo, para recuperar quem solicitou a adição de um recurso a um catálogo, `$expand=requestor` inclua na consulta.</span><span class="sxs-lookup"><span data-stu-id="5728c-119">For example, to retrieve who requested the addition of a resource to a catalog, include `$expand=requestor` in the query.</span></span> <span data-ttu-id="5728c-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5728c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5728c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5728c-121">Request headers</span></span>

| <span data-ttu-id="5728c-122">Nome</span><span class="sxs-lookup"><span data-stu-id="5728c-122">Name</span></span>      |<span data-ttu-id="5728c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="5728c-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5728c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5728c-124">Authorization</span></span> | <span data-ttu-id="5728c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5728c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5728c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5728c-127">Request body</span></span>

<span data-ttu-id="5728c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5728c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5728c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5728c-129">Response</span></span>

<span data-ttu-id="5728c-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5728c-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5728c-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5728c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5728c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5728c-132">Request</span></span>

<span data-ttu-id="5728c-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5728c-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourcerequests"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
```

### <a name="response"></a><span data-ttu-id="5728c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5728c-134">Response</span></span>

<span data-ttu-id="5728c-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5728c-135">The following is an example of the response.</span></span>

> <span data-ttu-id="5728c-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5728c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRequest",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "catalogId": "26ac0c0a-08bc-4a7b-a313-839f58044ba5",
      "id": "1fe272f0-d463-42aa-a9a8-b07ab50a1c4d",
      "isValidationOnly": false,
      "justification": "String",
      "requestState": "Delivered",
      "requestStatus": "Fulfilled",
      "requestType": "AdminAdd"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResourceRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
