---
title: Listar se aplica
description: Obtenha uma lista de objetos directoryobject aos quais um objeto claimsMappingPolicy foi aplicado.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ecb26248a99f471c7580fdee33adf7520e80841e
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234078"
---
# <a name="list-appliesto"></a><span data-ttu-id="b65a7-103">Listar se aplica</span><span class="sxs-lookup"><span data-stu-id="b65a7-103">List appliesTo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b65a7-104">Obtenha uma lista de objetos [directoryobject](../resources/directoryObject.md) aos quais um objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) foi aplicado.</span><span class="sxs-lookup"><span data-stu-id="b65a7-104">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object has been applied to.</span></span> <span data-ttu-id="b65a7-105">O claimsMappingPolicy só pode ser aplicado aos recursos [Application](../resources/application.md) e [servicePrincipalName](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="b65a7-105">The claimsMappingPolicy can only be applied to [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="b65a7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b65a7-106">Permissions</span></span>

<span data-ttu-id="b65a7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b65a7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b65a7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b65a7-109">Permission type</span></span>                        | <span data-ttu-id="b65a7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b65a7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b65a7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b65a7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b65a7-112">Policy. Read. All e Application. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="b65a7-112">Policy.Read.All and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="b65a7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b65a7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b65a7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b65a7-114">Not supported.</span></span> |
| <span data-ttu-id="b65a7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b65a7-115">Application</span></span>                            | <span data-ttu-id="b65a7-116">Policy. Read. All e Application. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="b65a7-116">Policy.Read.All and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b65a7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b65a7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/claimsMappingPolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b65a7-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b65a7-118">Optional query parameters</span></span>

<span data-ttu-id="b65a7-119">Este método oferece suporte `$expand`ao `$select` e `$top` aos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b65a7-119">This method supports the `$expand`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="b65a7-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b65a7-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="b65a7-121">Ao usar `$expand` certifique-se de que seu aplicativo solicite permissões para ler os objetos expandidos.</span><span class="sxs-lookup"><span data-stu-id="b65a7-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b65a7-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b65a7-122">Request headers</span></span>

| <span data-ttu-id="b65a7-123">Nome</span><span class="sxs-lookup"><span data-stu-id="b65a7-123">Name</span></span>      |<span data-ttu-id="b65a7-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b65a7-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b65a7-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b65a7-125">Authorization</span></span> | <span data-ttu-id="b65a7-126">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="b65a7-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b65a7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b65a7-127">Request body</span></span>

<span data-ttu-id="b65a7-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b65a7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b65a7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b65a7-129">Response</span></span>

<span data-ttu-id="b65a7-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b65a7-130">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b65a7-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b65a7-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b65a7-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b65a7-132">Request</span></span>

<span data-ttu-id="b65a7-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b65a7-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_appliesto"
}-->

```http
GET https://graph.microsoft.com/beta/claimsMappingPolicies/{id}/appliesTo
```

### <a name="response"></a><span data-ttu-id="b65a7-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b65a7-134">Response</span></span>

<span data-ttu-id="b65a7-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b65a7-135">The following is an example of the response.</span></span>

> <span data-ttu-id="b65a7-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b65a7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "deletedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List appliesTo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->