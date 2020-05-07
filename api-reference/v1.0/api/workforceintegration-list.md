---
title: Listar workforceIntegrations
description: Recupere uma lista de objetos workforceIntegration.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6f5e37feb028e5929bdb48ccf54b62083de9cbc9
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154042"
---
# <a name="list-workforceintegrations"></a><span data-ttu-id="6efe9-103">Listar workforceIntegrations</span><span class="sxs-lookup"><span data-stu-id="6efe9-103">List workforceIntegrations</span></span>

<span data-ttu-id="6efe9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6efe9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6efe9-105">Recupere uma lista de objetos [workforceIntegration](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="6efe9-105">Retrieve a list of [workforceIntegration](../resources/workforceintegration.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="6efe9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6efe9-106">Permissions</span></span>

<span data-ttu-id="6efe9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6efe9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6efe9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6efe9-109">Permission type</span></span>                        | <span data-ttu-id="6efe9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6efe9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6efe9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6efe9-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="6efe9-112">WorkforceIntegration. Read. All, WorkforceIntegration. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6efe9-112">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="6efe9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6efe9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6efe9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6efe9-114">Not supported.</span></span> |
| <span data-ttu-id="6efe9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6efe9-115">Application</span></span>                            | <span data-ttu-id="6efe9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6efe9-116">Not supported.</span></span> |

> <span data-ttu-id="6efe9-117">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="6efe9-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="6efe9-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="6efe9-118">Global admins can access groups that they are not a member of.</span></span>


## <a name="http-request"></a><span data-ttu-id="6efe9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6efe9-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teamwork/workforceIntegrations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6efe9-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6efe9-120">Optional query parameters</span></span>

<span data-ttu-id="6efe9-121">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6efe9-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6efe9-122">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6efe9-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6efe9-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6efe9-123">Request headers</span></span>

| <span data-ttu-id="6efe9-124">Nome</span><span class="sxs-lookup"><span data-stu-id="6efe9-124">Name</span></span>      |<span data-ttu-id="6efe9-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="6efe9-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6efe9-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="6efe9-126">Authorization</span></span> | <span data-ttu-id="6efe9-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6efe9-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6efe9-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6efe9-129">Request body</span></span>

<span data-ttu-id="6efe9-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6efe9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6efe9-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6efe9-131">Response</span></span>

<span data-ttu-id="6efe9-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [workforceIntegration](../resources/workforceintegration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6efe9-132">If successful, this method returns a `200 OK` response code and a collection of [workforceIntegration](../resources/workforceintegration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6efe9-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6efe9-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6efe9-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6efe9-134">Request</span></span>

<span data-ttu-id="6efe9-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6efe9-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_workforceintegrations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations
```

---


### <a name="response"></a><span data-ttu-id="6efe9-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="6efe9-136">Response</span></span>

<span data-ttu-id="6efe9-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6efe9-137">The following is an example of the response.</span></span>

> <span data-ttu-id="6efe9-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6efe9-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "displayName": "displayName-value",
      "apiVersion": 99,
      "encryption": {
        "protocol": "protocol-value",
        "secret": "secret-value"
      },
      "isActive": true,
      "url": "url-value",
      "supportedEntities": "supportedEntities-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List workforceIntegrations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
