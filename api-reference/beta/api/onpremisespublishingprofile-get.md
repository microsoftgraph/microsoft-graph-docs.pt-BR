---
title: Obter onPremisesPublishingProfile
description: Recupere as propriedades e os relacionamentos de um objeto [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fb3d6b43473ea1660976170625009ecea5c50baf
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878346"
---
# <a name="get-onpremisespublishingprofile"></a><span data-ttu-id="9fcca-103">Obter onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="9fcca-103">Get onPremisesPublishingProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fcca-104">Recupere as propriedades e os relacionamentos de um objeto [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="9fcca-104">Retrieve the properties and relationships of an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9fcca-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9fcca-105">Permissions</span></span>

<span data-ttu-id="9fcca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fcca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9fcca-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9fcca-108">Permission type</span></span>                        | <span data-ttu-id="9fcca-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9fcca-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="9fcca-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9fcca-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9fcca-111">OnPremisesPublishingProfiles. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9fcca-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="9fcca-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9fcca-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fcca-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9fcca-113">Not supported.</span></span> |
| <span data-ttu-id="9fcca-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9fcca-114">Application</span></span>                            | <span data-ttu-id="9fcca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9fcca-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9fcca-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9fcca-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9fcca-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9fcca-117">Optional query parameters</span></span>

<span data-ttu-id="9fcca-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9fcca-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9fcca-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9fcca-119">Request headers</span></span>

| <span data-ttu-id="9fcca-120">Nome</span><span class="sxs-lookup"><span data-stu-id="9fcca-120">Name</span></span>      |<span data-ttu-id="9fcca-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fcca-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9fcca-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9fcca-122">Authorization</span></span> | <span data-ttu-id="9fcca-123">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="9fcca-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9fcca-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9fcca-124">Request body</span></span>

<span data-ttu-id="9fcca-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9fcca-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9fcca-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fcca-126">Response</span></span>

<span data-ttu-id="9fcca-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9fcca-127">If successful, this method returns a `200 OK` response code and an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9fcca-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9fcca-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9fcca-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9fcca-129">Request</span></span>

<span data-ttu-id="9fcca-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9fcca-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9fcca-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="9fcca-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_onpremisespublishingprofile"
}-->

```http
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning?$expand=publishedResources,agents,agentGroups
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9fcca-132">C#</span><span class="sxs-lookup"><span data-stu-id="9fcca-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onpremisespublishingprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9fcca-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="9fcca-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onpremisespublishingprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9fcca-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9fcca-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onpremisespublishingprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9fcca-135">Java</span><span class="sxs-lookup"><span data-stu-id="9fcca-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-onpremisespublishingprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9fcca-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fcca-136">Response</span></span>

<span data-ttu-id="9fcca-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9fcca-137">The following is an example of the response.</span></span>

> <span data-ttu-id="9fcca-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9fcca-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```json
HTTP/1.1 200 OK

{
    "publishedResources": [
        {
            "publishingType": "provisioning",
            "displayName": "Demo Provisioning",
            "id": "aed0b780-965f-4149-85c5-a8c73e58b67d",
            "resourceName": "domain1.contoso.com",
            "agentGroups": [
                {
                    "id": "2d55ed41-1619-4848-92bb-0576d3038682",
                    "displayName": "Group 1"
                }
            ]
        }
    ],
    "agents": [
        {
            "id": "1234b780-965f-4149-85c5-a8c73e58b67d",
            "status": "Active",
            "machineName": "server 1",
            "externalIp": "1.0.0.127",
            "agentGroups": [
                 {
                    "id": "2d55ed41-1619-4848-92bb-0576d3038682",
                    "displayName": "Group 1"
                 }
            ]
        }
    ],
    "agentGroups": [
        {
            "id": "2d55ed41-1619-4848-92bb-0576d3038682",
            "displayName": "Group 1",
            "publishingType": "provisioning",
            "isDefault": false,
            "agents": [
                 {
                    "id": "1234b780-965f-4149-85c5-a8c73e58b67d",
                    "status": "Active"
                 }
            ],
            "publishedResources": [
                {
                    "displayName": "Demo Provisioning",
                    "id": "aed0b780-965f-4149-85c5-a8c73e58b67d",
                    "resourceName": "domain1.contoso.com"
                }
            ]
        }
    ],
  "hybridAgentUpdaterConfiguration": {
       "deferUpdateDateTime" : "2018-08-12T12:00",
       "updateWindow" :
          {
            "updateWindowStartTime" : "0:00:00",
            "updateWindowEndTime" : "23:59:00.0000000"
          },
       "allowUpdateConfigurationOverride" : false
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get onPremisesPublishingProfile",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
