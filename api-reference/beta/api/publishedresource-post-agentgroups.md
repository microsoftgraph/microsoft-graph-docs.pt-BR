---
title: Atribuir publishedResource ao onPremisesAgentGroup
description: Atribua um **objeto publishedResource** a um **objeto onPremisesAgentGroup.**
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 3cbd9e434701cad6ac7eff47daed6080c5979863
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055166"
---
# <a name="assign-publishedresource-to-onpremisesagentgroup"></a><span data-ttu-id="f4322-103">Atribuir publishedResource ao onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="f4322-103">Assign publishedResource to onPremisesAgentGroup</span></span>

<span data-ttu-id="f4322-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4322-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4322-105">Atribua um [objeto publishedResource](../resources/publishedresource.md) [ao objeto onPremisesAgentGroup.](../resources/onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="f4322-105">Assign a [publishedResource](../resources/publishedresource.md) object to [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4322-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f4322-106">Permissions</span></span>

<span data-ttu-id="f4322-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4322-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f4322-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4322-109">Permission type</span></span>                        | <span data-ttu-id="f4322-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f4322-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="f4322-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4322-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f4322-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4322-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="f4322-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4322-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4322-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4322-114">Not supported.</span></span> |
| <span data-ttu-id="f4322-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4322-115">Application</span></span>                            | <span data-ttu-id="f4322-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4322-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4322-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4322-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}/agentGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="f4322-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4322-118">Request headers</span></span>

| <span data-ttu-id="f4322-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f4322-119">Name</span></span>          | <span data-ttu-id="f4322-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4322-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f4322-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4322-121">Authorization</span></span> | <span data-ttu-id="f4322-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="f4322-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4322-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4322-123">Request body</span></span>

<span data-ttu-id="f4322-124">No corpo da solicitação, fornece uma representação JSON de um [objeto onPremisesAgentGroup.](../resources/onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="f4322-124">In the request body, supply a JSON representation of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f4322-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4322-125">Response</span></span>

<span data-ttu-id="f4322-126">Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [publishedResource](../resources/publishedresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f4322-126">If successful, this method returns a `201 Created` response code and a [publishedResource](../resources/publishedresource.md) object  in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f4322-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f4322-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f4322-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4322-128">Request</span></span>

<span data-ttu-id="f4322-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4322-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_onpremisespublishingprofile"
}-->

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/$ref
Content-type: application/json

```http
{
 "@odata.id": "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/2B032383-897C-42BA-917E-700B6890BDC3/"
}
```

### <a name="response"></a><span data-ttu-id="f4322-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4322-130">Response</span></span>

<span data-ttu-id="f4322-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f4322-131">The following is an example of the response.</span></span>

> <span data-ttu-id="f4322-132">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f4322-132">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgentGroup"
} -->

```http
HTTP/1.1 204
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create onPremisesAgentGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



