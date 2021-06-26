---
title: Obter serviceHealth
description: Recupere as propriedades e as relações de um objeto serviceHealth.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 02fadfb7b6937e0e3bdf05d9d491192114268928
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151675"
---
# <a name="get-servicehealth"></a><span data-ttu-id="e51da-103">Obter serviceHealth</span><span class="sxs-lookup"><span data-stu-id="e51da-103">Get serviceHealth</span></span>
<span data-ttu-id="e51da-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e51da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e51da-105">Recupere as propriedades e as relações de um [objeto serviceHealth.](../resources/servicehealth.md)</span><span class="sxs-lookup"><span data-stu-id="e51da-105">Retrieve the properties and relationships of a [serviceHealth](../resources/servicehealth.md) object.</span></span>

<span data-ttu-id="e51da-106">Esta operação fornece as informações de saúde de um serviço especificado para um locatário.</span><span class="sxs-lookup"><span data-stu-id="e51da-106">This operation provides the health information of a specified service for a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="e51da-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e51da-107">Permissions</span></span>
<span data-ttu-id="e51da-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e51da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e51da-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e51da-110">Permission type</span></span>|<span data-ttu-id="e51da-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e51da-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e51da-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e51da-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e51da-113">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="e51da-113">ServiceHealth.Read.All</span></span>|
|<span data-ttu-id="e51da-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e51da-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e51da-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e51da-115">Not supported.</span></span>|
|<span data-ttu-id="e51da-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e51da-116">Application</span></span>|<span data-ttu-id="e51da-117">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="e51da-117">ServiceHealth.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e51da-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e51da-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /admin/serviceAnnouncement/healthOverviews/{ServiceName}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e51da-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e51da-119">Optional query parameters</span></span>
<span data-ttu-id="e51da-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e51da-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e51da-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e51da-121">Request headers</span></span>
|<span data-ttu-id="e51da-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e51da-122">Name</span></span>|<span data-ttu-id="e51da-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e51da-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e51da-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e51da-124">Authorization</span></span>|<span data-ttu-id="e51da-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e51da-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e51da-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e51da-127">Request body</span></span>
<span data-ttu-id="e51da-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e51da-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e51da-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e51da-129">Response</span></span>

<span data-ttu-id="e51da-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto serviceHealth](../resources/servicehealth.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e51da-130">If successful, this method returns a `200 OK` response code and a [serviceHealth](../resources/servicehealth.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e51da-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e51da-131">Examples</span></span>

### <a name="example-1-get-the-properties-of-a-servicehealth-object"></a><span data-ttu-id="e51da-132">Exemplo 1: Obter as propriedades de um objeto serviceHealth</span><span class="sxs-lookup"><span data-stu-id="e51da-132">Example 1: Get the properties of a serviceHealth object</span></span>

#### <a name="request"></a><span data-ttu-id="e51da-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e51da-133">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["Microsoft 365 suite"],
  "name": "get_servicehealth"
}
-->

``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/healthOverviews/Microsoft 365 suite
```

#### <a name="response"></a><span data-ttu-id="e51da-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e51da-134">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceHealth"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#admin/serviceAnnouncement/healthOverviews/$entity",
    "service": "Microsoft 365 suite",
    "status": "RestoringService",
    "id": "OSDPPlatform"
}
```

### <a name="example-2-include-navigation-property-issues"></a><span data-ttu-id="e51da-135">Exemplo 2: Incluir problemas de propriedade de navegação</span><span class="sxs-lookup"><span data-stu-id="e51da-135">Example 2: Include navigation property issues</span></span>

#### <a name="request"></a><span data-ttu-id="e51da-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e51da-136">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["Microsoft 365 suite"],
  "name": "get_servicehealth_with_issues"
}
-->

``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/healthOverviews/Microsoft 365 suite?$expand=issues
```

#### <a name="response"></a><span data-ttu-id="e51da-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e51da-137">Response</span></span>
><span data-ttu-id="e51da-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e51da-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceHealth"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#admin/serviceAnnouncement/healthOverviews(issues())/$entity",
  "service": "Microsoft 365 suite",
  "status": "ServiceOperational",
  "id": "OSDPPlatform",
  "issues": [
        {
          "startDateTime": "2020-11-04T00:00:00Z",
          "endDateTime": "2020-11-20T17:00:00Z",
          "lastModifiedDateTime": "2020-11-20T17:56:31.39Z",
          "title": "Intermittently unable to access some Microsoft 365 services",
          "id": "MO226574",
          "impactDescription": "Users may have been intermittently unable to access some Microsoft 365 services.",
          "classification": "Advisory",
          "origin": "Microsoft",
          "status": "ServiceRestored",
          "service": "Exchange Online",
          "feature": "Tenant Administration (Provisioning, Remote PowerShell)",
          "featureGroup": "Management and Provisioning",
          "isResolved": true,
          "details": [],
          "posts": [
              {
                "createdDateTime": "2020-11-12T07:07:38.97Z",
                "postType": "Regular",
                "description": {
                    "contentType": "Text",
                    "content": "Users may have been intermittently unable to access some Microsoft 365 services. We'll provide an update within 30 minutes."
                  }
              }
          ]
        }
    ]
}
```