---
title: Atribuir publishedResource a onPremisesAgentGroup
description: Atribua um objeto **publishedResource** a um objeto **onPremisesAgentGroup** .
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6654f4e9b9c67d8fd6b9df58b9a1dfd91a79076c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47999171"
---
# <a name="assign-publishedresource-to-onpremisesagentgroup"></a><span data-ttu-id="857be-103">Atribuir publishedResource a onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="857be-103">Assign publishedResource to onPremisesAgentGroup</span></span>

<span data-ttu-id="857be-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="857be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="857be-105">Atribua um objeto [publishedResource](../resources/publishedresource.md) ao objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="857be-105">Assign a [publishedResource](../resources/publishedresource.md) object to [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="857be-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="857be-106">Permissions</span></span>

<span data-ttu-id="857be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="857be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="857be-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="857be-109">Permission type</span></span>                        | <span data-ttu-id="857be-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="857be-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="857be-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="857be-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="857be-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="857be-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="857be-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="857be-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="857be-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="857be-114">Not supported.</span></span> |
| <span data-ttu-id="857be-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="857be-115">Application</span></span>                            | <span data-ttu-id="857be-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="857be-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="857be-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="857be-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}/agentGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="857be-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="857be-118">Request headers</span></span>

| <span data-ttu-id="857be-119">Nome</span><span class="sxs-lookup"><span data-stu-id="857be-119">Name</span></span>          | <span data-ttu-id="857be-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="857be-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="857be-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="857be-121">Authorization</span></span> | <span data-ttu-id="857be-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="857be-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="857be-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="857be-123">Request body</span></span>

<span data-ttu-id="857be-124">No corpo da solicitação, forneça uma representação JSON de um objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="857be-124">In the request body, supply a JSON representation of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="857be-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="857be-125">Response</span></span>

<span data-ttu-id="857be-126">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [publishedResource](../resources/publishedresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="857be-126">If successful, this method returns a `201 Created` response code and a [publishedResource](../resources/publishedresource.md) object  in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="857be-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="857be-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="857be-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="857be-128">Request</span></span>

<span data-ttu-id="857be-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="857be-129">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="857be-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="857be-130">Response</span></span>

<span data-ttu-id="857be-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="857be-131">The following is an example of the response.</span></span>

> <span data-ttu-id="857be-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="857be-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


