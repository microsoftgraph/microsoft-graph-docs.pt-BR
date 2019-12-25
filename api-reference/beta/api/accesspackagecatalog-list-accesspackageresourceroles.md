---
title: Listar accessPackageResourceRoles
description: Recupere uma lista de objetos accessPackageResourceRole.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3bd46b8bc5bc542025d12f6c0685f31e0dc70402
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871709"
---
# <a name="list-accesspackageresourceroles"></a><span data-ttu-id="863a2-103">Listar accessPackageResourceRoles</span><span class="sxs-lookup"><span data-stu-id="863a2-103">List accessPackageResourceRoles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="863a2-104">Recupere uma lista de objetos [accessPackageResourceRole](../resources/accesspackageresourcerole.md) de um [AccessPackageResource](../resources/accesspackageresource.md) em um [accessPackageCatalog](../resources/accesspackagecatalog.md).</span><span class="sxs-lookup"><span data-stu-id="863a2-104">Retrieve a list of [accessPackageResourceRole](../resources/accesspackageresourcerole.md) objects of an [accessPackageResource](../resources/accesspackageresource.md) in an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>  <span data-ttu-id="863a2-105">Essa lista de funções pode ser usada pelo chamador para selecionar uma função, que é necessária ao [criar um accessPackageResourceRoleScope](accesspackage-post-accesspackageresourcerolescopes.md).</span><span class="sxs-lookup"><span data-stu-id="863a2-105">This list of roles can then be used by the caller to select a role, which is needed when subsequently [creating an accessPackageResourceRoleScope](accesspackage-post-accesspackageresourcerolescopes.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="863a2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="863a2-106">Permissions</span></span>

<span data-ttu-id="863a2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="863a2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="863a2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="863a2-109">Permission type</span></span>                        | <span data-ttu-id="863a2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="863a2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="863a2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="863a2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="863a2-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="863a2-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="863a2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="863a2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="863a2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="863a2-114">Not supported.</span></span> |
| <span data-ttu-id="863a2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="863a2-115">Application</span></span>                            | <span data-ttu-id="863a2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="863a2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="863a2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="863a2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{catalogId}/accessPackageResourceRoles?$filter=(originSystem+eq+%27{originSystemType}%27+and+accessPackageResource/id+eq+%27{resourceId}%27)&$expand=accessPackageResource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="863a2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="863a2-118">Optional query parameters</span></span>

<span data-ttu-id="863a2-119">Este método usa parâmetros de consulta OData para construir a resposta.</span><span class="sxs-lookup"><span data-stu-id="863a2-119">This method uses OData query parameters to construct the response.</span></span> <span data-ttu-id="863a2-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="863a2-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="863a2-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="863a2-121">Request headers</span></span>

| <span data-ttu-id="863a2-122">Nome</span><span class="sxs-lookup"><span data-stu-id="863a2-122">Name</span></span>      |<span data-ttu-id="863a2-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="863a2-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="863a2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="863a2-124">Authorization</span></span> | <span data-ttu-id="863a2-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="863a2-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="863a2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="863a2-127">Request body</span></span>

<span data-ttu-id="863a2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="863a2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="863a2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="863a2-129">Response</span></span>

<span data-ttu-id="863a2-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [accessPackageResourceRole](../resources/accesspackageresourcerole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="863a2-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceRole](../resources/accesspackageresourcerole.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="863a2-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="863a2-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="863a2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="863a2-132">Request</span></span>

<span data-ttu-id="863a2-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="863a2-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourceroles"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/15d889df-3eb8-4e9b-bfb4-b1908849aec4/accessPackageResourceRoles?$filter=(originSystem+eq+%27AadGroup%27+and+accessPackageResource/id+eq+%27a35bef72-a8aa-4ca3-af30-f6b2ece7208f%27)&$expand=accessPackageResource
```

### <a name="response"></a><span data-ttu-id="863a2-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="863a2-134">Response</span></span>

<span data-ttu-id="863a2-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="863a2-135">The following is an example of the response.</span></span>

> <span data-ttu-id="863a2-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="863a2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRole",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "displayName": "Member",
      "description": "description-value",
      "originId": "originId-value",
      "originSystem": "originSystem-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResourceRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
