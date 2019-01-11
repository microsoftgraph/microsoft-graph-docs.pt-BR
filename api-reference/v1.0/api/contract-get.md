---
title: Obter Contract
description: Recupere as propriedades e os relacionamentos do objeto contract.
localization_priority: Normal
ms.openlocfilehash: dd379286e161cc68e33af49bec20bb580512ef0b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805772"
---
# <a name="get-contract"></a><span data-ttu-id="4379a-103">Obter Contract</span><span class="sxs-lookup"><span data-stu-id="4379a-103">Get Contract</span></span>

<span data-ttu-id="4379a-104">Recupere as propriedades e os relacionamentos do objeto [contract](../resources/contract.md).</span><span class="sxs-lookup"><span data-stu-id="4379a-104">Retrieve the properties and relationships of [contract](../resources/contract.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4379a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4379a-105">Permissions</span></span>

<span data-ttu-id="4379a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4379a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4379a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4379a-108">Permission type</span></span>      | <span data-ttu-id="4379a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4379a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4379a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4379a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4379a-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4379a-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4379a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4379a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4379a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4379a-113">Not supported.</span></span>    |
|<span data-ttu-id="4379a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4379a-114">Application</span></span> | <span data-ttu-id="4379a-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4379a-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4379a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4379a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contracts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4379a-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4379a-117">Optional query parameters</span></span>

<span data-ttu-id="4379a-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4379a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4379a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4379a-119">Request headers</span></span>

| <span data-ttu-id="4379a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="4379a-120">Name</span></span>      |<span data-ttu-id="4379a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="4379a-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4379a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4379a-122">Authorization</span></span>  | <span data-ttu-id="4379a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4379a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4379a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4379a-125">Request body</span></span>

<span data-ttu-id="4379a-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4379a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4379a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="4379a-127">Response</span></span>

<span data-ttu-id="4379a-128">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Contract](../resources/contract.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4379a-128">If successful, this method returns a `200 OK` response code and [Contract](../resources/contract.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4379a-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4379a-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4379a-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4379a-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/v1.0/contracts/{id}
```

##### <a name="response"></a><span data-ttu-id="4379a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="4379a-131">Response</span></span>
<span data-ttu-id="4379a-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4379a-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contract"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 186

{
  "contractType": "contractType-value",
  "customerId": "customerId-value",
  "defaultDomainName": "defaultDomainName-value",
  "displayName": "displayName-value",
  "id": "id-value"
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
