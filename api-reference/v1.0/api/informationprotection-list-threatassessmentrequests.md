---
title: Listar threatAssessmentRequests
description: Recupere uma lista de objetos threatassessmentrequest.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d81f4580072a20cfaab6e4746074ced78ebdba8f
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591583"
---
# <a name="list-threatassessmentrequests"></a><span data-ttu-id="5ec04-103">Listar threatAssessmentRequests</span><span class="sxs-lookup"><span data-stu-id="5ec04-103">List threatAssessmentRequests</span></span>

<span data-ttu-id="5ec04-104">Recupere uma lista de objetos [threatAssessmentRequest](../resources/threatassessmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="5ec04-104">Retrieve a list of [threatAssessmentRequest](../resources/threatassessmentrequest.md) objects.</span></span>

<span data-ttu-id="5ec04-105">Uma solicitação de avaliação de ameaça pode ser um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="5ec04-105">A threat assessment request can be one of the following types:</span></span>

* [<span data-ttu-id="5ec04-106">Email</span><span class="sxs-lookup"><span data-stu-id="5ec04-106">Mail</span></span>](../resources/mailAssessmentRequest.md)
* [<span data-ttu-id="5ec04-107">Arquivo de email</span><span class="sxs-lookup"><span data-stu-id="5ec04-107">Email file</span></span>](../resources/emailFileAssessmentRequest.md)
* [<span data-ttu-id="5ec04-108">Arquivo</span><span class="sxs-lookup"><span data-stu-id="5ec04-108">File</span></span>](../resources/fileAssessmentRequest.md)
* [<span data-ttu-id="5ec04-109">URL</span><span class="sxs-lookup"><span data-stu-id="5ec04-109">URL</span></span>](../resources/urlAssessmentRequest.md)

## <a name="permissions"></a><span data-ttu-id="5ec04-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="5ec04-110">Permissions</span></span>

<span data-ttu-id="5ec04-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ec04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5ec04-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ec04-113">Permission type</span></span>                        | <span data-ttu-id="5ec04-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ec04-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5ec04-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ec04-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="5ec04-116">ThreatAssessment. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="5ec04-116">ThreatAssessment.ReadWrite.All.</span></span>             |
| <span data-ttu-id="5ec04-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ec04-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ec04-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ec04-118">Not supported.</span></span>                              |
| <span data-ttu-id="5ec04-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ec04-119">Application</span></span>                            | <span data-ttu-id="5ec04-120">ThreatAssessment. Read. All.</span><span class="sxs-lookup"><span data-stu-id="5ec04-120">ThreatAssessment.Read.All.</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="5ec04-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ec04-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /informationProtection/threatAssessmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5ec04-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5ec04-122">Optional query parameters</span></span>

<span data-ttu-id="5ec04-123">Este método oferece suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5ec04-123">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="5ec04-124">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5ec04-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="5ec04-125">Nome</span><span class="sxs-lookup"><span data-stu-id="5ec04-125">Name</span></span>            |<span data-ttu-id="5ec04-126">Valor</span><span class="sxs-lookup"><span data-stu-id="5ec04-126">Value</span></span>    |<span data-ttu-id="5ec04-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ec04-127">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="5ec04-128">$filter</span><span class="sxs-lookup"><span data-stu-id="5ec04-128">$filter</span></span>         |<span data-ttu-id="5ec04-129">string</span><span class="sxs-lookup"><span data-stu-id="5ec04-129">string</span></span>   |<span data-ttu-id="5ec04-130">Limita a resposta somente aos objetos que contêm os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="5ec04-130">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="5ec04-131">$orderby</span><span class="sxs-lookup"><span data-stu-id="5ec04-131">$orderby</span></span>        |<span data-ttu-id="5ec04-132">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ec04-132">string</span></span>   |<span data-ttu-id="5ec04-133">Por padrão, os objetos na resposta são decrescentes ordenados por seu valor **createdDateTime** .</span><span class="sxs-lookup"><span data-stu-id="5ec04-133">By default, the objects in the response are descending ordered by their **createdDateTime** value.</span></span>                                                                          |
|<span data-ttu-id="5ec04-134">$select</span><span class="sxs-lookup"><span data-stu-id="5ec04-134">$select</span></span>         |<span data-ttu-id="5ec04-135">string</span><span class="sxs-lookup"><span data-stu-id="5ec04-135">string</span></span>   |<span data-ttu-id="5ec04-p103">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="5ec04-p103">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="5ec04-138">$skipToken</span><span class="sxs-lookup"><span data-stu-id="5ec04-138">$skipToken</span></span>      |<span data-ttu-id="5ec04-139">string</span><span class="sxs-lookup"><span data-stu-id="5ec04-139">string</span></span>   |<span data-ttu-id="5ec04-140">Recupera a próxima página de resultados de conjuntos de resultados que abrangem várias páginas.</span><span class="sxs-lookup"><span data-stu-id="5ec04-140">Retrieves the next page of results from result sets that span multiple pages.</span></span>                                                                                               |

## <a name="request-headers"></a><span data-ttu-id="5ec04-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ec04-141">Request headers</span></span>

| <span data-ttu-id="5ec04-142">Nome</span><span class="sxs-lookup"><span data-stu-id="5ec04-142">Name</span></span>      |<span data-ttu-id="5ec04-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ec04-143">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5ec04-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ec04-144">Authorization</span></span> | <span data-ttu-id="5ec04-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ec04-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ec04-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ec04-147">Request body</span></span>

<span data-ttu-id="5ec04-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5ec04-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ec04-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ec04-149">Response</span></span>

<span data-ttu-id="5ec04-150">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [threatAssessmentRequest](../resources/threatassessmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ec04-150">If successful, this method returns a `200 OK` response code and a collection of [threatAssessmentRequest](../resources/threatassessmentrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5ec04-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5ec04-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5ec04-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ec04-152">Request</span></span>

<span data-ttu-id="5ec04-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ec04-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5ec04-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ec04-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_threatassessmentrequests"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests
```

### <a name="response"></a><span data-ttu-id="5ec04-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ec04-155">Response</span></span>

<span data-ttu-id="5ec04-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5ec04-156">The following is an example of the response.</span></span>

> <span data-ttu-id="5ec04-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ec04-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.threatAssessmentRequest",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#informationProtection/threatAssessmentRequests",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests?$skiptoken=eyJQYWdlQ29va2llIjoiPHJvdyBpZF9JZGVudGl0",
  "value": [
    {
      "@odata.type": "#microsoft.graph.mailAssessmentRequest",
      "id": "49c5ef5b-1f65-444a-e6b9-08d772ea2059",
      "createdDateTime": "2019-11-27T03:30:18.6890937Z",
      "contentType": "mail",
      "expectedAssessment": "block",
      "category": "spam",
      "status": "pending",
      "requestSource": "administrator",
      "recipientEmail": "tifc@a830edad9050849eqtpwbjzxodq.onmicrosoft.com",
      "destinationRoutingReason": "notJunk",
      "messageUri": "https://graph.microsoft.com/v1.0/users/c52ce8db-3e4b-4181-93c4-7d6b6bffaf60/messages/AAMkADU3MWUxOTU0LWNlOTEt=",
      "createdBy": {
        "user": {
          "id": "c52ce8db-3e4b-4181-93c4-7d6b6bffaf60",
          "displayName": "Ronald Admin"
        }
      }
    },
    {
      "@odata.type": "#microsoft.graph.emailFileAssessmentRequest",
      "id": "ab2ad9b3-2213-4091-ae0c-08d76ddbcacf",
      "createdDateTime": "2019-11-20T17:05:06.4088076Z",
      "contentType": "mail",
      "expectedAssessment": "block",
      "category": "malware",
      "status": "completed",
      "requestSource": "administrator",
      "recipientEmail": "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com",
      "destinationRoutingReason": "notJunk",
      "contentData": "",
      "createdBy": {
        "user": {
          "id": "c52ce8db-3e4b-4181-93c4-7d6b6bffaf60",
          "displayName": "Ronald Admin"
        }
      }
    },
    {
      "@odata.type": "#microsoft.graph.fileAssessmentRequest",
      "id": "18406a56-7209-4720-a250-08d772fccdaa",
      "createdDateTime": "2019-11-27T05:44:00.4051536Z",
      "contentType": "file",
      "expectedAssessment": "block",
      "category": "malware",
      "status": "completed",
      "requestSource": "administrator",
      "fileName": "b3d5b715-4b88-4bbb-b0ae-9a9281a3f18a.csv",
      "contentData": "",
      "createdBy": {
        "user": {
          "id": "c52ce8db-3e4b-4181-93c4-7d6b6bffaf60",
          "displayName": "Ronald Admin"
        }
      }
    },
    {
      "@odata.type": "#microsoft.graph.urlAssessmentRequest",
      "id": "723c35be-8b5a-47ae-29c0-08d76ddb7f5b",
      "createdDateTime": "2019-11-20T17:02:59.8160832Z",
      "contentType": "url",
      "expectedAssessment": "unblock",
      "category": "phishing",
      "status": "completed",
      "requestSource": "administrator",
      "url": "http://test.com",
      "createdBy": {
        "user": {
          "id": "c52ce8db-3e4b-4181-93c4-7d6b6bffaf60",
          "displayName": "Ronald Admin"
        }
      }
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List threatAssessmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
