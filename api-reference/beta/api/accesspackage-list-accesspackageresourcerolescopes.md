---
title: Listar accessPackageResourceRoleScopes
description: Recupere uma lista de objetos accesspackageresourcerolescope.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8383c80c6599391791739d28a9cc6f5ccaa5cb3c
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37935055"
---
# <a name="list-accesspackageresourcerolescopes"></a><span data-ttu-id="9201f-103">Listar accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="9201f-103">List accessPackageResourceRoleScopes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9201f-104">Recupere um pacote do Access com uma lista de objetos [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) .</span><span class="sxs-lookup"><span data-stu-id="9201f-104">Retrieve an access package with a list of [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) objects.</span></span>  <span data-ttu-id="9201f-105">Cada objeto é vinculado a um [accessPackageResourceRole](../resources/accesspackageresourcerole.md) e um [accessPackageResourceScope](../resources/accesspackageresourcescope.md).</span><span class="sxs-lookup"><span data-stu-id="9201f-105">Each object links to an [accessPackageResourceRole](../resources/accesspackageresourcerole.md) and an [accessPackageResourceScope](../resources/accesspackageresourcescope.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9201f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9201f-106">Permissions</span></span>

<span data-ttu-id="9201f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9201f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9201f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9201f-109">Permission type</span></span>                        | <span data-ttu-id="9201f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9201f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9201f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9201f-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="9201f-112">EntitlementManagement. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9201f-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="9201f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9201f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9201f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9201f-114">Not supported.</span></span> |
| <span data-ttu-id="9201f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9201f-115">Application</span></span>                            | <span data-ttu-id="9201f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9201f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9201f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9201f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackages/{id}?$expand=accessPackageResourceRoleScopes($expand=accessPackageResourceRole,accessPackageResourceScope)
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9201f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9201f-118">Optional query parameters</span></span>

<span data-ttu-id="9201f-119">Esse método usa parâmetros de consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9201f-119">This method uses OData query parameters to customize the response.</span></span> <span data-ttu-id="9201f-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9201f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9201f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9201f-121">Request headers</span></span>

| <span data-ttu-id="9201f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="9201f-122">Name</span></span>      |<span data-ttu-id="9201f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9201f-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9201f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9201f-124">Authorization</span></span> | <span data-ttu-id="9201f-125">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="9201f-125">Bearer \{token\}.</span></span> <span data-ttu-id="9201f-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9201f-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9201f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9201f-127">Request body</span></span>

<span data-ttu-id="9201f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9201f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9201f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9201f-129">Response</span></span>

<span data-ttu-id="9201f-130">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um [accessPackage](../resources/accesspackage.md) que contém uma coleção de objetos [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9201f-130">If successful, this method returns a `200 OK` response code and an [accessPackage](../resources/accesspackage.md) containing a collection of [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9201f-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9201f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9201f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9201f-132">Request</span></span>

<span data-ttu-id="9201f-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9201f-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourcerolescopes"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}?$expand=accessPackageResourceRoleScopes($expand=accessPackageResourceRole,accessPackageResourceScope)
```

### <a name="response"></a><span data-ttu-id="9201f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="9201f-134">Response</span></span>

<span data-ttu-id="9201f-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9201f-135">The following is an example of the response.</span></span>

> <span data-ttu-id="9201f-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9201f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "id": "933a4822-aed1-445b-9623-62116cd07a39",
    "catalogId": "32efb28c-9a7a-446c-986b-ca6528c6669d",
    "displayName": "Test Package 9-9",
    "description": "Test Package 9-9",
    "isHidden": false,
    "accessPackageResourceRoleScopes": [
        {
            "id": "70113acf-4dcb-453f-b517-2394598d974e_22bfd707-ab6f-404f-b0b5-a5e6f5d0ba36",
            "createdBy": "alice@contoso.com",
            "createdDateTime": "2019-09-09T19:54:14.853Z",
            "modifiedBy": "alice@contoso.com",
            "modifiedDateTime": "2019-09-09T19:54:14.853Z",
            "accessPackageResourceRole": {
                "id": "70113acf-4dcb-453f-b517-2394598d974e",
                "displayName": "Owner",
                "originSystem": "origin-type",
                "originId": "Owner_7b56ede0-9b58-40bd-b11e-b3d18fc32698"
            },
            "accessPackageResourceScope": {
                "id": "22bfd707-ab6f-404f-b0b5-a5e6f5d0ba36",
                "displayName": "Root",
                "description": "Root Scope",
                "originId": "7b56ede0-9b58-40bd-b11e-b3d18fc32698",
                "originSystem": "origin-type",
                "isRootScope": true
            }
        }
    ]
}

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResourceRoleScopes",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
