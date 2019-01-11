---
title: Obter dataPolicyOperation
description: Recupere as propriedades do objeto dataPolicyOperation.
localization_priority: Normal
ms.openlocfilehash: a06b2b119683a75516b0d51f955565276249be41
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860358"
---
# <a name="get-datapolicyoperation"></a><span data-ttu-id="d96d1-103">Obter dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="d96d1-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="d96d1-104">Recupere as propriedades de um objeto **dataPolicyOperation** .</span><span class="sxs-lookup"><span data-stu-id="d96d1-104">Retrieve the properties of a **dataPolicyOperation** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d96d1-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="d96d1-105">Permissions</span></span>
<span data-ttu-id="d96d1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d96d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d96d1-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d96d1-108">Permission type</span></span>      | <span data-ttu-id="d96d1-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d96d1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d96d1-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d96d1-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="d96d1-111">User.Export.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d96d1-111">User.Export.All, User.Read.All</span></span>  |
|<span data-ttu-id="d96d1-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d96d1-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d96d1-113">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="d96d1-113">Not applicable</span></span>  |
|<span data-ttu-id="d96d1-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d96d1-114">Application</span></span> | <span data-ttu-id="d96d1-115">User.Export.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d96d1-115">User.Export.All, User.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d96d1-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d96d1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d96d1-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d96d1-117">Request headers</span></span>
| <span data-ttu-id="d96d1-118">Nome</span><span class="sxs-lookup"><span data-stu-id="d96d1-118">Name</span></span>      |<span data-ttu-id="d96d1-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="d96d1-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d96d1-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="d96d1-120">Authorization</span></span>  | <span data-ttu-id="d96d1-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="d96d1-121">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d96d1-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d96d1-122">Request body</span></span>
<span data-ttu-id="d96d1-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d96d1-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d96d1-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="d96d1-124">Response</span></span>
<span data-ttu-id="d96d1-125">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [dataPolicyOperation](../resources/datapolicyoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d96d1-125">If successful, this method returns a `200 OK` response code and a [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d96d1-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d96d1-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d96d1-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d96d1-127">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```http
GET https://graph.microsoft.com/v1.0/dataPolicyOperations/{id}
```
##### <a name="response"></a><span data-ttu-id="d96d1-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d96d1-128">Response</span></span>
><span data-ttu-id="d96d1-p102">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d96d1-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.dataPolicyOperation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 212

{
  "completedDateTime": "datetime-value",
  "id": "id-value",
  "status": "status-value",
  "storageLocation": "storageLocation-value",
  "userId": "userId-value",
  "submittedDateTime": "datetime-value", 
  "progress": "double-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get dataPolicyOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
