---
title: Listar contratos
description: Recupere uma lista de objetos contract associados a um locatário do parceiro.
ms.openlocfilehash: ed2e7ea7c422372adc8377863713982cc3c688aa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005942"
---
# <a name="list-contracts"></a><span data-ttu-id="c8ad6-103">Listar contratos</span><span class="sxs-lookup"><span data-stu-id="c8ad6-103">List contracts</span></span>

<span data-ttu-id="c8ad6-104">Recupere uma lista de objetos [contract](../resources/contract.md) associados a um locatário do parceiro.</span><span class="sxs-lookup"><span data-stu-id="c8ad6-104">Retrieve a list of [contract](../resources/contract.md) objects associated to a partner tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8ad6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c8ad6-105">Permissions</span></span>

<span data-ttu-id="c8ad6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8ad6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c8ad6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c8ad6-108">Permission type</span></span>      | <span data-ttu-id="c8ad6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c8ad6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8ad6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c8ad6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c8ad6-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c8ad6-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c8ad6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c8ad6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8ad6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8ad6-113">Not supported.</span></span>    |
|<span data-ttu-id="c8ad6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8ad6-114">Application</span></span> | <span data-ttu-id="c8ad6-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8ad6-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8ad6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c8ad6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /contracts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c8ad6-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c8ad6-117">Optional query parameters</span></span>

<span data-ttu-id="c8ad6-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c8ad6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> 

> <span data-ttu-id="c8ad6-119">A filtragem é compatível com customerId, defaultDomainName e displayName.</span><span class="sxs-lookup"><span data-stu-id="c8ad6-119">Filtering is supported for customerId, defaultDomainName, and displayName.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c8ad6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c8ad6-120">Request headers</span></span>

| <span data-ttu-id="c8ad6-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c8ad6-121">Name</span></span>      |<span data-ttu-id="c8ad6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8ad6-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c8ad6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c8ad6-123">Authorization</span></span>  | <span data-ttu-id="c8ad6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8ad6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c8ad6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c8ad6-126">Request body</span></span>

<span data-ttu-id="c8ad6-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c8ad6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8ad6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8ad6-128">Response</span></span>

<span data-ttu-id="c8ad6-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Contract](../resources/contract.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c8ad6-129">If successful, this method returns a `200 OK` response code and a collection of [Contract](../resources/contract.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8ad6-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c8ad6-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c8ad6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c8ad6-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/v1.0/contracts
```

##### <a name="response"></a><span data-ttu-id="c8ad6-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8ad6-132">Response</span></span>

<span data-ttu-id="c8ad6-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c8ad6-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contract",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
    {
      "contractType": "contractType-value",
      "customerId": "customerId-value",
      "defaultDomainName": "defaultDomainName-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Contract",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->