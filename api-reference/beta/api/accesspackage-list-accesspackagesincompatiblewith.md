---
title: Listar accessPackagesIncompatibleWith
description: Recupere uma lista de pacotes de acesso que indicaram que seus direitos de acesso são incompatíveis com um pacote de acesso específico.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: aeb918ef4c3675a3ab2e4539dc48d2b8f297c7be
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401029"
---
# <a name="list-accesspackagesincompatiblewith"></a><span data-ttu-id="52384-103">Listar accessPackagesIncompatibleWith</span><span class="sxs-lookup"><span data-stu-id="52384-103">List accessPackagesIncompatibleWith</span></span>

<span data-ttu-id="52384-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52384-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52384-105">Recupere uma lista dos [objetos accessPackage](../resources/accesspackage.md) que marcaram um [accessPackage especificado](../resources/accesspackage.md) como incompatível.</span><span class="sxs-lookup"><span data-stu-id="52384-105">Retrieve a list of the [accessPackage](../resources/accesspackage.md) objects that have marked a specified [accessPackage](../resources/accesspackage.md) as incompatible.</span></span>

## <a name="permissions"></a><span data-ttu-id="52384-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="52384-106">Permissions</span></span>

<span data-ttu-id="52384-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52384-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="52384-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52384-109">Permission type</span></span>                        | <span data-ttu-id="52384-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="52384-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="52384-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52384-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="52384-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52384-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="52384-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52384-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52384-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52384-114">Not supported.</span></span> |
| <span data-ttu-id="52384-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52384-115">Application</span></span>                            | <span data-ttu-id="52384-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52384-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="52384-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52384-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackage/{id}/accessPackagesIncompatibleWith
```

## <a name="optional-query-parameters"></a><span data-ttu-id="52384-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="52384-118">Optional query parameters</span></span>

<span data-ttu-id="52384-119">Este método dá suporte aos parâmetros de consulta OData para pajamento no lado do servidor por meio de uma resposta grande.</span><span class="sxs-lookup"><span data-stu-id="52384-119">This method supports the OData query parameters for server-side paging through a large response.</span></span> <span data-ttu-id="52384-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="52384-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="52384-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52384-121">Request headers</span></span>

| <span data-ttu-id="52384-122">Nome</span><span class="sxs-lookup"><span data-stu-id="52384-122">Name</span></span>      |<span data-ttu-id="52384-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="52384-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="52384-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="52384-124">Authorization</span></span> | <span data-ttu-id="52384-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52384-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="52384-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52384-127">Request body</span></span>

<span data-ttu-id="52384-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="52384-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52384-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="52384-129">Response</span></span>

<span data-ttu-id="52384-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos accessPackage](../resources/accesspackage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52384-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackage](../resources/accesspackage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="52384-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="52384-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="52384-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52384-132">Request</span></span>

<span data-ttu-id="52384-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="52384-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accesspackagesincompatiblewith"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/accessPackagesIncompatibleWith
```


### <a name="response"></a><span data-ttu-id="52384-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="52384-134">Response</span></span>

<span data-ttu-id="52384-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="52384-135">The following is an example of the response.</span></span>

> <span data-ttu-id="52384-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="52384-136">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "c0a74b4d-2694-4d5d-a964-1bee4ff0aaf2",
      "catalogId": "c955f54f-e248-4155-b314-0bdd63f5aae9",
      "displayName": "accesspackage"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackagesIncompatibleWith",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


