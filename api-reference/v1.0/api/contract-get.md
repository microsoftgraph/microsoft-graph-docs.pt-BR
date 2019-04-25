---
title: Obter contrato
description: Recupere as propriedades e os relacionamentos do objeto Contract.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ba6ba3dd1e0dc631f5aeb61dd6d714e9d7a81bb6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566175"
---
# <a name="get-contract"></a><span data-ttu-id="5f4a6-103">Obter contrato</span><span class="sxs-lookup"><span data-stu-id="5f4a6-103">Get Contract</span></span>

<span data-ttu-id="5f4a6-104">Recupere as propriedades e os relacionamentos do objeto [Contract](../resources/contract.md) .</span><span class="sxs-lookup"><span data-stu-id="5f4a6-104">Retrieve the properties and relationships of [contract](../resources/contract.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f4a6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5f4a6-105">Permissions</span></span>

<span data-ttu-id="5f4a6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f4a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5f4a6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f4a6-108">Permission type</span></span>      | <span data-ttu-id="5f4a6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5f4a6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f4a6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f4a6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5f4a6-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5f4a6-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5f4a6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f4a6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f4a6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f4a6-113">Not supported.</span></span>    |
|<span data-ttu-id="5f4a6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5f4a6-114">Application</span></span> | <span data-ttu-id="5f4a6-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f4a6-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f4a6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f4a6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contracts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5f4a6-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5f4a6-117">Optional query parameters</span></span>

<span data-ttu-id="5f4a6-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5f4a6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5f4a6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f4a6-119">Request headers</span></span>

| <span data-ttu-id="5f4a6-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5f4a6-120">Name</span></span>      |<span data-ttu-id="5f4a6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f4a6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5f4a6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f4a6-122">Authorization</span></span>  | <span data-ttu-id="5f4a6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f4a6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5f4a6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5f4a6-125">Request body</span></span>

<span data-ttu-id="5f4a6-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5f4a6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f4a6-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f4a6-127">Response</span></span>

<span data-ttu-id="5f4a6-128">Se bem-sucedido, este método retorna o `200 OK` código de resposta e o objeto [Contract](../resources/contract.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5f4a6-128">If successful, this method returns a `200 OK` response code and [Contract](../resources/contract.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f4a6-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5f4a6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5f4a6-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f4a6-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/v1.0/contracts/{id}
```

##### <a name="response"></a><span data-ttu-id="5f4a6-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f4a6-131">Response</span></span>
<span data-ttu-id="5f4a6-p103">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5f4a6-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
