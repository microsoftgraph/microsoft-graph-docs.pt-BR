---
title: Obter onPremisesPublishingProfile
description: Recupere as propriedades e os relacionamentos de um objeto [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 92e2800d03cb2e9aab59c119b7a9b7e9f09682d7
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841070"
---
# <a name="get-onpremisespublishingprofile"></a><span data-ttu-id="eb12d-103">Obter onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="eb12d-103">Get onPremisesPublishingProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb12d-104">Recupere as propriedades e os relacionamentos de um objeto [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="eb12d-104">Retrieve the properties and relationships of an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb12d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="eb12d-105">Permissions</span></span>

<span data-ttu-id="eb12d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb12d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eb12d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb12d-108">Permission type</span></span>                        | <span data-ttu-id="eb12d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eb12d-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="eb12d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb12d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="eb12d-111">OnPremisesPublishingProfiles. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="eb12d-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="eb12d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb12d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb12d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb12d-113">Not supported.</span></span> |
| <span data-ttu-id="eb12d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb12d-114">Application</span></span>                            | <span data-ttu-id="eb12d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb12d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb12d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb12d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eb12d-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="eb12d-117">Optional query parameters</span></span>

<span data-ttu-id="eb12d-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="eb12d-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eb12d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb12d-119">Request headers</span></span>

| <span data-ttu-id="eb12d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="eb12d-120">Name</span></span>      |<span data-ttu-id="eb12d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb12d-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="eb12d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb12d-122">Authorization</span></span> | <span data-ttu-id="eb12d-123">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="eb12d-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb12d-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb12d-124">Request body</span></span>

<span data-ttu-id="eb12d-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eb12d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb12d-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb12d-126">Response</span></span>

<span data-ttu-id="eb12d-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb12d-127">If successful, this method returns a `200 OK` response code and an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eb12d-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="eb12d-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eb12d-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb12d-129">Request</span></span>

<span data-ttu-id="eb12d-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb12d-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_onpremisespublishingprofile"
}-->

```http
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning?$expand=publishedResources,agents,agentGroups
```

### <a name="response"></a><span data-ttu-id="eb12d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb12d-131">Response</span></span>

<span data-ttu-id="eb12d-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="eb12d-132">The following is an example of the response.</span></span>

> <span data-ttu-id="eb12d-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb12d-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
