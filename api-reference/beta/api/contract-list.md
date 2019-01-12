---
title: Listar contratos
description: Recupere uma lista de objetos contract associados a um locatário do parceiro.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6df390cbe742443bf8a996362fa2cf2909ef83f3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971071"
---
# <a name="list-contracts"></a><span data-ttu-id="c8c2c-103">Listar contratos</span><span class="sxs-lookup"><span data-stu-id="c8c2c-103">List contracts</span></span>

> <span data-ttu-id="c8c2c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c8c2c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8c2c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c8c2c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c8c2c-106">Recupere uma lista de objetos [contract](../resources/contract.md) associados a um locatário do parceiro.</span><span class="sxs-lookup"><span data-stu-id="c8c2c-106">Retrieve a list of [contract](../resources/contract.md) objects associated to a partner tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8c2c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c8c2c-107">Permissions</span></span>

<span data-ttu-id="c8c2c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8c2c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c8c2c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c8c2c-110">Permission type</span></span>      | <span data-ttu-id="c8c2c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c8c2c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8c2c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c8c2c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c8c2c-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c8c2c-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c8c2c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c8c2c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8c2c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8c2c-115">Not supported.</span></span>    |
|<span data-ttu-id="c8c2c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8c2c-116">Application</span></span> | <span data-ttu-id="c8c2c-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8c2c-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8c2c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c8c2c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /contracts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c8c2c-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c8c2c-119">Optional query parameters</span></span>

<span data-ttu-id="c8c2c-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c8c2c-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> 

> <span data-ttu-id="c8c2c-121">A filtragem é compatível com customerId, defaultDomainName e displayName.</span><span class="sxs-lookup"><span data-stu-id="c8c2c-121">Filtering is supported for customerId, defaultDomainName, and displayName.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c8c2c-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c8c2c-122">Request headers</span></span>

| <span data-ttu-id="c8c2c-123">Nome</span><span class="sxs-lookup"><span data-stu-id="c8c2c-123">Name</span></span>      |<span data-ttu-id="c8c2c-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8c2c-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c8c2c-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c8c2c-125">Authorization</span></span>  | <span data-ttu-id="c8c2c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8c2c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c8c2c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c8c2c-128">Request body</span></span>

<span data-ttu-id="c8c2c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c8c2c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8c2c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8c2c-130">Response</span></span>

<span data-ttu-id="c8c2c-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Contract](../resources/contract.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c8c2c-131">If successful, this method returns a `200 OK` response code and a collection of [Contract](../resources/contract.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8c2c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c8c2c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c8c2c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c8c2c-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/beta/contracts
```

##### <a name="response"></a><span data-ttu-id="c8c2c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8c2c-134">Response</span></span>

<span data-ttu-id="c8c2c-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c8c2c-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Contract",
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
