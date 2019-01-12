---
title: Obter Contract
description: Recupere as propriedades e os relacionamentos do objeto contract.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 86bf035bf015aa85a47c3f5cad62ef497c12e99a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916667"
---
# <a name="get-contract"></a><span data-ttu-id="f836f-103">Obter Contract</span><span class="sxs-lookup"><span data-stu-id="f836f-103">Get Contract</span></span>

> <span data-ttu-id="f836f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f836f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f836f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f836f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f836f-106">Recupere as propriedades e os relacionamentos do objeto [contract](../resources/contract.md).</span><span class="sxs-lookup"><span data-stu-id="f836f-106">Retrieve the properties and relationships of [contract](../resources/contract.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f836f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f836f-107">Permissions</span></span>

<span data-ttu-id="f836f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f836f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f836f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f836f-110">Permission type</span></span>      | <span data-ttu-id="f836f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f836f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f836f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f836f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f836f-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f836f-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f836f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f836f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f836f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f836f-115">Not supported.</span></span>    |
|<span data-ttu-id="f836f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f836f-116">Application</span></span> | <span data-ttu-id="f836f-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f836f-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f836f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f836f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contracts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f836f-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f836f-119">Optional query parameters</span></span>

<span data-ttu-id="f836f-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f836f-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f836f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f836f-121">Request headers</span></span>

| <span data-ttu-id="f836f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f836f-122">Name</span></span>      |<span data-ttu-id="f836f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f836f-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f836f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f836f-124">Authorization</span></span>  | <span data-ttu-id="f836f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f836f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f836f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f836f-127">Request body</span></span>

<span data-ttu-id="f836f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f836f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f836f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f836f-129">Response</span></span>

<span data-ttu-id="f836f-130">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Contract](../resources/contract.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f836f-130">If successful, this method returns a `200 OK` response code and [Contract](../resources/contract.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f836f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f836f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f836f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f836f-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/beta/contracts/{id}
```

##### <a name="response"></a><span data-ttu-id="f836f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f836f-133">Response</span></span>
<span data-ttu-id="f836f-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f836f-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
