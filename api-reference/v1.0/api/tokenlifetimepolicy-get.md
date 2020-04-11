---
title: Obter tokenLifetimePolicy
description: Recupere as propriedades e os relacionamentos do objeto tokenLifetimePolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8099c651470c30375b0e1118540e5b77b96e91ae
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229546"
---
# <a name="get-tokenlifetimepolicy"></a><span data-ttu-id="71472-103">Obter tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="71472-103">Get tokenLifetimePolicy</span></span>

<span data-ttu-id="71472-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71472-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="71472-105">Recupere as propriedades e os relacionamentos de um objeto [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="71472-105">Retrieve the properties and relationships of a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="71472-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="71472-106">Permissions</span></span>

<span data-ttu-id="71472-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71472-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="71472-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71472-109">Permission type</span></span>                        | <span data-ttu-id="71472-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="71472-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="71472-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71472-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="71472-112">Policy. Read. All, Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="71472-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="71472-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71472-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71472-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71472-114">Not supported.</span></span> |
| <span data-ttu-id="71472-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71472-115">Application</span></span>                            | <span data-ttu-id="71472-116">Policy. Read. All, Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="71472-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="71472-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71472-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/tokenLifetimePolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="71472-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="71472-118">Optional query parameters</span></span>

<span data-ttu-id="71472-119">Este método oferece suporte `$expand` aos `$select` parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="71472-119">This method supports the `$expand` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="71472-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="71472-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="71472-121">Ao usar `$expand` certifique-se de que seu aplicativo solicite permissões para ler os objetos expandidos.</span><span class="sxs-lookup"><span data-stu-id="71472-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71472-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71472-122">Request headers</span></span>

| <span data-ttu-id="71472-123">Nome</span><span class="sxs-lookup"><span data-stu-id="71472-123">Name</span></span>      |<span data-ttu-id="71472-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="71472-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="71472-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="71472-125">Authorization</span></span> | <span data-ttu-id="71472-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71472-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71472-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71472-128">Request body</span></span>

<span data-ttu-id="71472-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="71472-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71472-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="71472-130">Response</span></span>

<span data-ttu-id="71472-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71472-131">If successful, this method returns a `200 OK` response code and the requested [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="71472-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="71472-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="71472-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71472-133">Request</span></span>

<span data-ttu-id="71472-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="71472-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_tokenlifetimepolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/tokenLifetimePolicies/{id}
```

### <a name="response"></a><span data-ttu-id="71472-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="71472-135">Response</span></span>

<span data-ttu-id="71472-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="71472-136">The following is an example of the response.</span></span>

> <span data-ttu-id="71472-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="71472-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
