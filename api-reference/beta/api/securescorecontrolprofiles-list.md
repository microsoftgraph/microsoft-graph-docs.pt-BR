---
title: Listar secureScoreControlProfiles
description: Recupere as propriedades e os relacionamentos de um objeto secureScoreControlProfiles.
localization_priority: Normal
ms.openlocfilehash: 29efa2c9bedaa295304eb82190a64fbc4a863cd1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331537"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="c7099-103">Listar secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="c7099-103">List secureScoreControlProfiles</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7099-104">Recupera uma lista de objetos [secureScoreControlProfile](../resources/securescorecontrolprofiles.md) para um locatário.</span><span class="sxs-lookup"><span data-stu-id="c7099-104">Retrieves a list of [secureScoreControlProfile](../resources/securescorecontrolprofiles.md) objects for a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7099-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c7099-105">Permissions</span></span>

<span data-ttu-id="c7099-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7099-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7099-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7099-108">Permission type</span></span>      | <span data-ttu-id="c7099-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c7099-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7099-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7099-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="c7099-111">Escopo securityevents. Read. All, escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="c7099-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="c7099-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7099-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c7099-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7099-113">Not supported.</span></span>  |
|<span data-ttu-id="c7099-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7099-114">Application</span></span> | <span data-ttu-id="c7099-115">Escopo securityevents. Read. All, escopo securityevents. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="c7099-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7099-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7099-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
```

## <a name="request-headers"></a><span data-ttu-id="c7099-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7099-117">Request headers</span></span>

| <span data-ttu-id="c7099-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c7099-118">Name</span></span>      |<span data-ttu-id="c7099-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7099-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c7099-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7099-120">Authorization</span></span>  | <span data-ttu-id="c7099-121">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="c7099-121">Bearer {code}.</span></span> <span data-ttu-id="c7099-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7099-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7099-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7099-123">Request body</span></span>

<span data-ttu-id="c7099-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c7099-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7099-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7099-125">Response</span></span>

<span data-ttu-id="c7099-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos **secureScoreControlProfile** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7099-126">If successful, this method returns a `200 OK` response code and a collection of **secureScoreControlProfile** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7099-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7099-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7099-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7099-128">Request</span></span>

<span data-ttu-id="c7099-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7099-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScoreControlProfiles
```

### <a name="response"></a><span data-ttu-id="c7099-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7099-130">Response</span></span>

<span data-ttu-id="c7099-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c7099-131">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "value": [
        {
            "actionType": "actionType.value",
            "actionUrl": "actionUrl.value",
            "controlCategory": "controlCategory.value",
            "title": "title.value",
            "deprecated": true,
            "implementationCost": "implementationCost.value",
            "lastModifiedDateTime": "lastModifiedDateTime.value",
            "maxScore": 1020.13,
            "rank": 100,
            "remediation": "remediation.value",
            "remediationImpact": "remediationImpact.value",
            "service": "service.value",
            "threats": [
                "threats.value"
            ],
            "tier": "tier.value",
            "userImpact": "userImpact.value",
            "id": "id.value",
            "azureTenantId": "azureTenantId.value",
            "controlStateUpdates": [
                {
                    "assignedTo": "assignedTo.value",
                    "comment": "comment.value",
                    "state": "state.value",
                    "updatedBy": "updatedBy.value",
                    "updatedDateTime": "updatedDateTime.value"
                }
            ],
            "vendorInformation": {
                "provider": "SecureScore",
                "providerVersion": null,
                "subProvider": null,
                "vendor": "Microsoft"
            }
         }
     ]
}
```


<!--
{
  "type": "#page.annotation",
  "description": "List secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
