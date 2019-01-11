---
title: Obter Contract
description: Recupere as propriedades e os relacionamentos do objeto contract.
localization_priority: Normal
ms.openlocfilehash: 6e23594c0c897bd5827e1eb251907c9a1a646a1f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843845"
---
# <a name="get-contract"></a><span data-ttu-id="75808-103">Obter Contract</span><span class="sxs-lookup"><span data-stu-id="75808-103">Get Contract</span></span>

> <span data-ttu-id="75808-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="75808-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="75808-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="75808-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="75808-106">Recupere as propriedades e os relacionamentos do objeto [contract](../resources/contract.md).</span><span class="sxs-lookup"><span data-stu-id="75808-106">Retrieve the properties and relationships of [contract](../resources/contract.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="75808-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="75808-107">Permissions</span></span>

<span data-ttu-id="75808-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75808-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="75808-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75808-110">Permission type</span></span>      | <span data-ttu-id="75808-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="75808-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75808-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75808-112">Delegated (work or school account)</span></span> | <span data-ttu-id="75808-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="75808-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="75808-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="75808-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75808-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75808-115">Not supported.</span></span>    |
|<span data-ttu-id="75808-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="75808-116">Application</span></span> | <span data-ttu-id="75808-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75808-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="75808-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75808-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contracts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="75808-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="75808-119">Optional query parameters</span></span>

<span data-ttu-id="75808-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="75808-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="75808-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="75808-121">Request headers</span></span>

| <span data-ttu-id="75808-122">Nome</span><span class="sxs-lookup"><span data-stu-id="75808-122">Name</span></span>      |<span data-ttu-id="75808-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="75808-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="75808-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="75808-124">Authorization</span></span>  | <span data-ttu-id="75808-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="75808-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="75808-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75808-127">Request body</span></span>

<span data-ttu-id="75808-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="75808-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75808-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="75808-129">Response</span></span>

<span data-ttu-id="75808-130">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Contract](../resources/contract.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75808-130">If successful, this method returns a `200 OK` response code and [Contract](../resources/contract.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75808-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="75808-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="75808-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75808-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/beta/contracts/{id}
```

##### <a name="response"></a><span data-ttu-id="75808-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="75808-133">Response</span></span>
<span data-ttu-id="75808-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="75808-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Contract"
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
