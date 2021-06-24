---
title: Obter serviceHealthIssue
description: Recupere as propriedades e as relações de um objeto serviceHealthIssue.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: a848773e047ed36cdd8aecd082aabffec7f1311b
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107775"
---
# <a name="get-servicehealthissue"></a><span data-ttu-id="f2ea1-103">Obter serviceHealthIssue</span><span class="sxs-lookup"><span data-stu-id="f2ea1-103">Get serviceHealthIssue</span></span>
<span data-ttu-id="f2ea1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2ea1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2ea1-105">Recupere as propriedades e as relações de um [objeto serviceHealthIssue.](../resources/servicehealthissue.md)</span><span class="sxs-lookup"><span data-stu-id="f2ea1-105">Retrieve the properties and relationships of a [serviceHealthIssue](../resources/servicehealthissue.md) object.</span></span>

<span data-ttu-id="f2ea1-106">Essa operação recupera um problema de saúde do serviço especificado para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f2ea1-106">This operation retrieves a specified service health issue for tenant.</span></span> <span data-ttu-id="f2ea1-107">A operação retornará um erro se o problema não existir para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f2ea1-107">The operation returns an error if the issue does not exist for the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2ea1-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f2ea1-108">Permissions</span></span>
<span data-ttu-id="f2ea1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2ea1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2ea1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2ea1-111">Permission type</span></span>|<span data-ttu-id="f2ea1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f2ea1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2ea1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2ea1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f2ea1-114">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2ea1-114">ServiceHealth.Read.All</span></span>|
|<span data-ttu-id="f2ea1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2ea1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2ea1-116">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2ea1-116">ServiceHealth.Read.All</span></span>|
|<span data-ttu-id="f2ea1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2ea1-117">Application</span></span>|<span data-ttu-id="f2ea1-118">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2ea1-118">ServiceHealth.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2ea1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2ea1-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/serviceAnnouncement/issues/{serviceHealthIssueId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f2ea1-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f2ea1-120">Optional query parameters</span></span>
<span data-ttu-id="f2ea1-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f2ea1-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2ea1-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2ea1-122">Request headers</span></span>
|<span data-ttu-id="f2ea1-123">Nome</span><span class="sxs-lookup"><span data-stu-id="f2ea1-123">Name</span></span>|<span data-ttu-id="f2ea1-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2ea1-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f2ea1-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2ea1-125">Authorization</span></span>|<span data-ttu-id="f2ea1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2ea1-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2ea1-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2ea1-128">Request body</span></span>
<span data-ttu-id="f2ea1-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f2ea1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2ea1-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2ea1-130">Response</span></span>

<span data-ttu-id="f2ea1-131">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto serviceHealthIssue](../resources/servicehealthissue.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2ea1-131">If successful, this method returns a `200 OK` response code and a [serviceHealthIssue](../resources/servicehealthissue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2ea1-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2ea1-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2ea1-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2ea1-133">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["MO226784"],
  "name": "get_servicehealthissue"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/issues/MO226784
```


### <a name="response"></a><span data-ttu-id="f2ea1-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2ea1-134">Response</span></span>
><span data-ttu-id="f2ea1-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f2ea1-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceHealthIssue"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#admin/serviceAnnouncement/issues/$entity",
  "startDateTime": "2020-11-14T08:15:00Z",
  "endDateTime": "2020-11-14T09:45:00Z",
  "lastModifiedDateTime": "2020-11-14T11:06:53.353Z",
  "title": "Intermittently unable to access some Microsoft 365 services",
  "id": "MO226784",
  "impactDescription": "Users may have been intermittently unable to access some Microsoft 365 services.",
  "classification": "Advisory",
  "origin": "Microsoft",
  "status": "ServiceRestored",
  "service": "Microsoft 365 suite",
  "feature": "Access",
  "featureGroup": "Portal",
  "isResolved": true,
  "details": [],
  "posts": [
    {
      "createdDateTime": "2020-11-12T07:07:38.97Z",
      "postType": "Regular",
      "description": {
        "contentType": "Text",
        "content": "Title: Intermittently unable to invite partners to meetings using some Microsoft 365 services\n\nUser Impact: Users may have been intermittently unable to invite partners to meetings using some Microsoft 365 services."
      }
    }
  ]
}
```

