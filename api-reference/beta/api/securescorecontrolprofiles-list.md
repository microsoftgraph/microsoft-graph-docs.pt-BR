---
title: Lista secureScoreControlProfiles
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.openlocfilehash: 33d0f6059d66350c9fa763097277f83c041e96ee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036332"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="f39b4-104">Lista secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="f39b4-104">List secureScoreControlProfiles</span></span>

 > <span data-ttu-id="f39b4-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f39b4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f39b4-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f39b4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f39b4-107">Recupere as propriedades e relacionamentos de um objeto [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) .</span><span class="sxs-lookup"><span data-stu-id="f39b4-107">Retrieve the properties and relationships of a [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f39b4-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="f39b4-108">Permissions</span></span>

<span data-ttu-id="f39b4-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f39b4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f39b4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f39b4-111">Permission type</span></span>      | <span data-ttu-id="f39b4-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f39b4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f39b4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f39b4-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="f39b4-114">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="f39b4-114">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="f39b4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f39b4-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f39b4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f39b4-116">Not supported.</span></span>  |
|<span data-ttu-id="f39b4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f39b4-117">Application</span></span> | <span data-ttu-id="f39b4-118">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="f39b4-118">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f39b4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f39b4-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
```

## <a name="request-headers"></a><span data-ttu-id="f39b4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f39b4-120">Request headers</span></span>

| <span data-ttu-id="f39b4-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f39b4-121">Name</span></span>      |<span data-ttu-id="f39b4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f39b4-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f39b4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f39b4-123">Authorization</span></span>  | <span data-ttu-id="f39b4-p104">Portador {código}. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f39b4-p104">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f39b4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f39b4-126">Request body</span></span>

<span data-ttu-id="f39b4-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f39b4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f39b4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f39b4-128">Response</span></span>

<span data-ttu-id="f39b4-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **secureScoreControlProfiles** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f39b4-129">If successful, this method returns a `200 OK` response code and a **secureScoreControlProfiles** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f39b4-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f39b4-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f39b4-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f39b4-131">Request</span></span>

<span data-ttu-id="f39b4-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f39b4-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScoreControlProfiles
```

### <a name="response"></a><span data-ttu-id="f39b4-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f39b4-133">Response</span></span>

<span data-ttu-id="f39b4-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f39b4-134">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.secureScoreControlProfiles"
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
            "deprecated": "deprecated.value",
            "implementationCost": "implementationCost.value",
            "lastModifiedDateTime": "lastModifiedDateTime.value",
            "maxScore": "maxScore.value",
            "rank": "rank.value",
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


<!-- {
  "type": "#page.annotation",
  "description": "List secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
