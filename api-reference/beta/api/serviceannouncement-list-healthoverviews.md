---
title: Listar healthOverviews
description: Recupere os recursos serviceHealth da propriedade de navegação healthOverviews.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: d8e2905acb0989d2d47d1f3df7c71237dca083c4
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210891"
---
# <a name="list-healthoverviews"></a><span data-ttu-id="4376c-103">Listar healthOverviews</span><span class="sxs-lookup"><span data-stu-id="4376c-103">List healthOverviews</span></span>
<span data-ttu-id="4376c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4376c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4376c-105">Recupere os [recursos serviceHealth](../resources/servicehealth.md) da **propriedade de navegação healthOverviews.**</span><span class="sxs-lookup"><span data-stu-id="4376c-105">Retrieve the [serviceHealth](../resources/servicehealth.md) resources from the **healthOverviews** navigation property.</span></span>

<span data-ttu-id="4376c-106">Esta operação fornece o relatório de saúde de todos os serviços inscritos para um locatário.</span><span class="sxs-lookup"><span data-stu-id="4376c-106">This operation provides the health report of all subscribed services for a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="4376c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="4376c-107">Permissions</span></span>
<span data-ttu-id="4376c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4376c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4376c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4376c-110">Permission type</span></span>|<span data-ttu-id="4376c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4376c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4376c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4376c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4376c-113">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="4376c-113">ServiceHealth.Read.All</span></span>|
|<span data-ttu-id="4376c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4376c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4376c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4376c-115">Not supported.</span></span>|
|<span data-ttu-id="4376c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4376c-116">Application</span></span>|<span data-ttu-id="4376c-117">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="4376c-117">ServiceHealth.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4376c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4376c-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/serviceAnnouncement/healthOverviews
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4376c-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4376c-119">Optional query parameters</span></span>
<span data-ttu-id="4376c-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4376c-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4376c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4376c-121">Request headers</span></span>
|<span data-ttu-id="4376c-122">Nome</span><span class="sxs-lookup"><span data-stu-id="4376c-122">Name</span></span>|<span data-ttu-id="4376c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="4376c-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4376c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4376c-124">Authorization</span></span>|<span data-ttu-id="4376c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4376c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4376c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4376c-127">Request body</span></span>
<span data-ttu-id="4376c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4376c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4376c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4376c-129">Response</span></span>

<span data-ttu-id="4376c-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos serviceHealth](../resources/servicehealth.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4376c-130">If successful, this method returns a `200 OK` response code and a collection of [serviceHealth](../resources/servicehealth.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4376c-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4376c-131">Examples</span></span>

### <a name="example-1-get-servicehealth-resources"></a><span data-ttu-id="4376c-132">Exemplo 1: Obter recursos serviceHealth</span><span class="sxs-lookup"><span data-stu-id="4376c-132">Example 1: Get serviceHealth resources</span></span>

#### <a name="request"></a><span data-ttu-id="4376c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4376c-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4376c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="4376c-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_healthoverviews"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/healthOverviews
```
# <a name="c"></a>[<span data-ttu-id="4376c-135">C#</span><span class="sxs-lookup"><span data-stu-id="4376c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-healthoverviews-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4376c-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4376c-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-healthoverviews-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4376c-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4376c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-healthoverviews-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4376c-138">Java</span><span class="sxs-lookup"><span data-stu-id="4376c-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-healthoverviews-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4376c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="4376c-139">Response</span></span>
><span data-ttu-id="4376c-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4376c-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceHealth",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#admin/serviceAnnouncement/healthOverviews",
  "value": [
    {
        "service": "Exchange Online",
        "status": "ServicaOperational",
        "id": "Exchange"
    },
    {
        "service": "Identity Service",
        "status": "ServiceRestored",
        "id": "OrgLiveID"
    },
    {
        "service": "Microsoft 365 suite",
        "status": "ServiceOperational",
        "id": "OSDPPlatform"
    }
  ]
}
```

### <a name="example-2-include-navigation-property-issues"></a><span data-ttu-id="4376c-141">Exemplo 2: Incluir problemas de propriedade de navegação</span><span class="sxs-lookup"><span data-stu-id="4376c-141">Example 2: Include navigation property issues</span></span>

#### <a name="request"></a><span data-ttu-id="4376c-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4376c-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4376c-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="4376c-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_healthoverviews_with_issues"
}
-->

``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/healthOverviews?$expand=issues
```
# <a name="c"></a>[<span data-ttu-id="4376c-144">C#</span><span class="sxs-lookup"><span data-stu-id="4376c-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-healthoverviews-with-issues-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4376c-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4376c-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-healthoverviews-with-issues-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4376c-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4376c-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-healthoverviews-with-issues-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4376c-147">Java</span><span class="sxs-lookup"><span data-stu-id="4376c-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-healthoverviews-with-issues-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4376c-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="4376c-148">Response</span></span>
><span data-ttu-id="4376c-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4376c-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceHealth",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#admin/serviceAnnouncement/healthOverviews(issues())",
  "value": [
    {
      "service": "Exchange Online",
      "status": "ServiceOperational",
      "id": "Exchange",
      "issues": [
          {
              "startDateTime": "2020-11-04T00:00:00Z",
              "endDateTime": "2020-11-20T17:00:00Z",
              "lastModifiedDateTime": "2020-11-20T17:56:31.39Z",
              "title": "Admins are unable to migrate some user mailboxes from IMAP using the Exchange admin center or PowerShell",
              "id": "EX226574",
              "impactDescription": "Admins attempting to migrate some user mailboxes using the Exchange admin center or PowerShell experienced failures.",
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
                        "content": "Title: Exchange Online service has login issue. We'll provide an update within 30 minutes."
                    }
                  }
                ]
          }
        ]
    }
  ]
}
```
