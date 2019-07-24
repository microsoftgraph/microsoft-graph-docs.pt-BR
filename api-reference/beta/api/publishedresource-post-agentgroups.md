---
title: Atribuir publishedResource a onPremisesAgentGroup
description: Atribua um objeto **publishedResource** a um objeto **onPremisesAgentGroup** .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9ec20b1208906129e5559307fc347e9d39c6dd7e
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840965"
---
# <a name="assign-publishedresource-to-onpremisesagentgroup"></a><span data-ttu-id="5b06d-103">Atribuir publishedResource a onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="5b06d-103">Assign publishedResource to onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b06d-104">Atribua um objeto [publishedResource](../resources/publishedresource.md) ao objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="5b06d-104">Assign a [publishedResource](../resources/publishedresource.md) object to [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b06d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5b06d-105">Permissions</span></span>

<span data-ttu-id="5b06d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b06d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5b06d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b06d-108">Permission type</span></span>                        | <span data-ttu-id="5b06d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5b06d-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="5b06d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b06d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5b06d-111">OnPremisesPublishingProfiles. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="5b06d-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="5b06d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b06d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b06d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b06d-113">Not supported.</span></span> |
| <span data-ttu-id="5b06d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b06d-114">Application</span></span>                            | <span data-ttu-id="5b06d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b06d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b06d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b06d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}/agentGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="5b06d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b06d-117">Request headers</span></span>

| <span data-ttu-id="5b06d-118">Nome</span><span class="sxs-lookup"><span data-stu-id="5b06d-118">Name</span></span>          | <span data-ttu-id="5b06d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b06d-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="5b06d-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b06d-120">Authorization</span></span> | <span data-ttu-id="5b06d-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="5b06d-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b06d-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b06d-122">Request body</span></span>

<span data-ttu-id="5b06d-123">No corpo da solicitação, forneça uma representação JSON de um objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="5b06d-123">In the request body, supply a JSON representation of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5b06d-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b06d-124">Response</span></span>

<span data-ttu-id="5b06d-125">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [publishedResource](../resources/publishedresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5b06d-125">If successful, this method returns a `201 Created` response code and a [publishedResource](../resources/publishedresource.md) object  in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5b06d-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5b06d-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5b06d-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b06d-127">Request</span></span>

<span data-ttu-id="5b06d-128">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b06d-128">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5b06d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b06d-129">Response</span></span>

<span data-ttu-id="5b06d-130">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5b06d-130">The following is an example of the response.</span></span>

> <span data-ttu-id="5b06d-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5b06d-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
