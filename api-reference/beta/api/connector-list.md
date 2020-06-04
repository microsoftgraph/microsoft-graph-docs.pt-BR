---
title: Conectores de lista
description: Recupere uma lista de objetos Connector.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 75b0d48c9b900f9d947e23cc68649e92f3c7f438
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556078"
---
# <a name="list-connectors"></a><span data-ttu-id="4ebe2-103">Conectores de lista</span><span class="sxs-lookup"><span data-stu-id="4ebe2-103">List connectors</span></span>

<span data-ttu-id="4ebe2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ebe2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ebe2-105">Recupere uma lista de objetos [Connector](../resources/connector.md) .</span><span class="sxs-lookup"><span data-stu-id="4ebe2-105">Retrieve a list of [connector](../resources/connector.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ebe2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4ebe2-106">Permissions</span></span>
<span data-ttu-id="4ebe2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ebe2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ebe2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ebe2-109">Permission type</span></span>      | <span data-ttu-id="4ebe2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4ebe2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ebe2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ebe2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4ebe2-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4ebe2-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4ebe2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ebe2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ebe2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ebe2-114">Not supported.</span></span>    |
|<span data-ttu-id="4ebe2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ebe2-115">Application</span></span> | <span data-ttu-id="4ebe2-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ebe2-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ebe2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ebe2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectors
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4ebe2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4ebe2-118">Optional query parameters</span></span>
<span data-ttu-id="4ebe2-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4ebe2-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ebe2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ebe2-120">Request headers</span></span>
| <span data-ttu-id="4ebe2-121">Nome</span><span class="sxs-lookup"><span data-stu-id="4ebe2-121">Name</span></span>      |<span data-ttu-id="4ebe2-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ebe2-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4ebe2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ebe2-123">Authorization</span></span>  | <span data-ttu-id="4ebe2-124">Portador.</span><span class="sxs-lookup"><span data-stu-id="4ebe2-124">Bearer.</span></span> <span data-ttu-id="4ebe2-125">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="4ebe2-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ebe2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ebe2-126">Request body</span></span>
<span data-ttu-id="4ebe2-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4ebe2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ebe2-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ebe2-128">Response</span></span>

<span data-ttu-id="4ebe2-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [Connector](../resources/connector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ebe2-129">If successful, this method returns a `200 OK` response code and collection of [connector](../resources/connector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ebe2-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ebe2-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4ebe2-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ebe2-131">Request</span></span>
<span data-ttu-id="4ebe2-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ebe2-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connectors"
}-->
```http
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors
```
##### <a name="response"></a><span data-ttu-id="4ebe2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ebe2-133">Response</span></span>
<span data-ttu-id="4ebe2-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4ebe2-134">The following is an example of the response.</span></span> <span data-ttu-id="4ebe2-135">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="4ebe2-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4ebe2-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4ebe2-136">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "value": [
    {
      "id": "id-value",
      "machineName": "machineName-value",
      "externalIp": "externalIp-value",
      "status": "status-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List connectors",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
