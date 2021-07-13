---
title: Listar incompatívelAccessPackages
description: Recupere uma lista de pacotes de acesso cujos direitos de acesso são incompatíveis com um pacote de acesso específico.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: fc30ee9ae6a80b04820b363dea87f376e5db638b
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401028"
---
# <a name="list-incompatibleaccesspackages"></a><span data-ttu-id="a0ec2-103">Listar incompatívelAccessPackages</span><span class="sxs-lookup"><span data-stu-id="a0ec2-103">List incompatibleAccessPackages</span></span>

<span data-ttu-id="a0ec2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0ec2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0ec2-105">Recuperar uma lista dos [objetos accessPackage](../resources/accesspackage.md) que foram marcados como incompatíveis em [um accessPackage](../resources/accesspackage.md).</span><span class="sxs-lookup"><span data-stu-id="a0ec2-105">Retrieve a list of the [accessPackage](../resources/accesspackage.md) objects that have been marked as incompatible on an [accessPackage](../resources/accesspackage.md).</span></span>  

## <a name="permissions"></a><span data-ttu-id="a0ec2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a0ec2-106">Permissions</span></span>

<span data-ttu-id="a0ec2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0ec2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a0ec2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0ec2-109">Permission type</span></span>                        | <span data-ttu-id="a0ec2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a0ec2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a0ec2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0ec2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a0ec2-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0ec2-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="a0ec2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0ec2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0ec2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0ec2-114">Not supported.</span></span> |
| <span data-ttu-id="a0ec2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0ec2-115">Application</span></span>                            | <span data-ttu-id="a0ec2-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0ec2-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0ec2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0ec2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackage/{id}/incompatibleAccessPackages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a0ec2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a0ec2-118">Optional query parameters</span></span>

<span data-ttu-id="a0ec2-119">Este método dá suporte aos parâmetros de consulta OData para pajamento no lado do servidor por meio de uma resposta grande.</span><span class="sxs-lookup"><span data-stu-id="a0ec2-119">This method supports the OData query parameters for server-side paging through a large response.</span></span> <span data-ttu-id="a0ec2-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a0ec2-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0ec2-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0ec2-121">Request headers</span></span>

| <span data-ttu-id="a0ec2-122">Nome</span><span class="sxs-lookup"><span data-stu-id="a0ec2-122">Name</span></span>      |<span data-ttu-id="a0ec2-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0ec2-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a0ec2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0ec2-124">Authorization</span></span> | <span data-ttu-id="a0ec2-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0ec2-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0ec2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0ec2-127">Request body</span></span>

<span data-ttu-id="a0ec2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a0ec2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0ec2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0ec2-129">Response</span></span>

<span data-ttu-id="a0ec2-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos accessPackage](../resources/accesspackage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0ec2-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackage](../resources/accesspackage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a0ec2-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a0ec2-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a0ec2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0ec2-132">Request</span></span>

<span data-ttu-id="a0ec2-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0ec2-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_incompatibleaccesspackages"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleAccessPackages
### Response

The following is an example of the response.

> **Note:** The response object shown here might be shortened for readability.

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
  "description": "List incompatibleAccessPackages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

