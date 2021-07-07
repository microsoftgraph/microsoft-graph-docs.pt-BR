---
title: 'cloudPcAuditEvent: getAuditActivityTypes'
description: Obter tipos de atividade de auditoria por id de locatário.
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 7ea6612160474c2fbbfde792f3565f1100dac146
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316962"
---
# <a name="cloudpcauditevent-getauditactivitytypes"></a><span data-ttu-id="9d396-103">cloudPcAuditEvent: getAuditActivityTypes</span><span class="sxs-lookup"><span data-stu-id="9d396-103">cloudPcAuditEvent: getAuditActivityTypes</span></span>

<span data-ttu-id="9d396-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d396-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d396-105">Obter tipos de atividade de auditoria por ID de locatário.</span><span class="sxs-lookup"><span data-stu-id="9d396-105">Get audit activity types by tenant ID.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="9d396-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9d396-106">Permissions</span></span>

<span data-ttu-id="9d396-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d396-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d396-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9d396-109">Permission type</span></span>| <span data-ttu-id="9d396-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9d396-110">Permissions (from least to most privileged)</span></span> |
|:---|:---|
|<span data-ttu-id="9d396-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9d396-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9d396-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d396-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="9d396-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9d396-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d396-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d396-114">Not supported.</span></span>|
|<span data-ttu-id="9d396-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9d396-115">Application</span></span>|<span data-ttu-id="9d396-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d396-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d396-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9d396-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="9d396-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9d396-118">Request headers</span></span>

| <span data-ttu-id="9d396-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9d396-119">Name</span></span>          | <span data-ttu-id="9d396-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d396-120">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="9d396-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9d396-121">Authorization</span></span> | <span data-ttu-id="9d396-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9d396-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d396-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9d396-124">Request body</span></span>

<span data-ttu-id="9d396-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9d396-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d396-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d396-126">Response</span></span>

<span data-ttu-id="9d396-127">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção String no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9d396-127">If successful, this method returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9d396-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9d396-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9d396-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9d396-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9d396-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d396-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cloudpcauditevent_getauditactivitytypes"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/auditEvents/getAuditActivityTypes
```
# <a name="c"></a>[<span data-ttu-id="9d396-131">C#</span><span class="sxs-lookup"><span data-stu-id="9d396-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cloudpcauditevent-getauditactivitytypes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9d396-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d396-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cloudpcauditevent-getauditactivitytypes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9d396-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d396-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cloudpcauditevent-getauditactivitytypes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9d396-134">Java</span><span class="sxs-lookup"><span data-stu-id="9d396-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cloudpcauditevent-getauditactivitytypes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9d396-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d396-135">Response</span></span>


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Edm.String)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    "Get Audit Activity Types value"
  ]
}
```
