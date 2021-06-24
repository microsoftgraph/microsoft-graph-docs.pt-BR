---
title: Listar problemas
description: Recupere os recursos serviceHealthIssue da propriedade de navegação de problemas.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 887caf3463e64e05c9f2738bc836d2f200d4dbee
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109055"
---
# <a name="list-issues"></a><span data-ttu-id="4fec1-103">Listar problemas</span><span class="sxs-lookup"><span data-stu-id="4fec1-103">List issues</span></span>
<span data-ttu-id="4fec1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4fec1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4fec1-105">Recupere [os recursos serviceHealthIssue](../resources/servicehealthissue.md) da propriedade **de navegação de** problemas.</span><span class="sxs-lookup"><span data-stu-id="4fec1-105">Retrieve [serviceHealthIssue](../resources/servicehealthissue.md) resources from the **issues** navigation property.</span></span>

<span data-ttu-id="4fec1-106">Essa operação recupera informações sobre todos os problemas de saúde do serviço existentes para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4fec1-106">This operation retrieves information about all service health issues that exist for the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="4fec1-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="4fec1-107">Permissions</span></span>
<span data-ttu-id="4fec1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4fec1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fec1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4fec1-110">Permission type</span></span>|<span data-ttu-id="4fec1-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4fec1-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fec1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4fec1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4fec1-113">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="4fec1-113">ServiceHealth.Read.All</span></span>|
|<span data-ttu-id="4fec1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4fec1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fec1-115">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="4fec1-115">ServiceHealth.Read.All</span></span>|
|<span data-ttu-id="4fec1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4fec1-116">Application</span></span>|<span data-ttu-id="4fec1-117">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="4fec1-117">ServiceHealth.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fec1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4fec1-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/serviceAnnouncement/issues
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4fec1-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4fec1-119">Optional query parameters</span></span>
<span data-ttu-id="4fec1-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4fec1-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4fec1-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4fec1-121">Request headers</span></span>
|<span data-ttu-id="4fec1-122">Nome</span><span class="sxs-lookup"><span data-stu-id="4fec1-122">Name</span></span>|<span data-ttu-id="4fec1-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="4fec1-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4fec1-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4fec1-124">Authorization</span></span>|<span data-ttu-id="4fec1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4fec1-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fec1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4fec1-127">Request body</span></span>
<span data-ttu-id="4fec1-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4fec1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4fec1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4fec1-129">Response</span></span>

<span data-ttu-id="4fec1-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos serviceHealthIssue](../resources/servicehealthissue.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4fec1-130">If successful, this method returns a `200 OK` response code and a collection of [serviceHealthIssue](../resources/servicehealthissue.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fec1-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4fec1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4fec1-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4fec1-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_servicehealthissue"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/issues
```


### <a name="response"></a><span data-ttu-id="4fec1-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="4fec1-133">Response</span></span>
><span data-ttu-id="4fec1-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4fec1-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceHealthIssue",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#admin/serviceAnnouncement/issues",
  "value": [
    {
      "startDateTime": "2020-11-13T21:00:00Z",
      "endDateTime": "2020-11-14T17:15:00Z",
      "lastModifiedDateTime": "2020-11-14T18:20:24.767Z",
      "title": "Limited number of users unable to send or receive email through the Exchange Online service",
      "id": "EX226792",
      "impactDescription": "Users may have been unable to send or receive email through the Exchange Online service.",
      "classification": "Incident",
      "origin": "Microsoft",
      "status": "ServiceRestored",
      "service": "Exchange Online",
      "feature": "Mailflow - delayed delivery from Internet",
      "featureGroup": "E-Mail timely delivery",
      "isResolved": true,
      "details": [
        {
          "name": "NotifyInApp",
          "value": "True"
        }
      ],
      "posts": [
        {
          "createdDateTime": "2020-11-12T07:07:38.97Z",
          "postType": "Regular",
          "description": {
            "contentType": "Text",
            "content": "Title: Limited number of users unable to send or receive email through the Exchange Online service\n\nUser Impact: Users may be unable to send or receive email through the Exchange Online service."
          }
        }
      ]
    }
  ]
}
```

