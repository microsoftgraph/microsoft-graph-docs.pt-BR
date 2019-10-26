---
title: Criar userflow
description: Use esta API para criar um novo userflow.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c76c75b4429054f92a1cfec592065c0caae5cc43
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734501"
---
# <a name="create-userflow"></a><span data-ttu-id="c5191-103">Criar userflow</span><span class="sxs-lookup"><span data-stu-id="c5191-103">Create userFlow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5191-104">Criar um novo objeto [userflow](../resources/identityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="c5191-104">Create a new [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5191-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c5191-105">Permissions</span></span>

<span data-ttu-id="c5191-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5191-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c5191-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5191-108">Permission type</span></span>                        | <span data-ttu-id="c5191-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c5191-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c5191-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5191-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c5191-111">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c5191-111">IdentityUserFlow.ReadWrite.All</span></span> |
| <span data-ttu-id="c5191-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5191-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5191-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5191-113">Not supported.</span></span> |
| <span data-ttu-id="c5191-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5191-114">Application</span></span>                            | <span data-ttu-id="c5191-115">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c5191-115">IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5191-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5191-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/userFlows
```

## <a name="request-headers"></a><span data-ttu-id="c5191-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5191-117">Request headers</span></span>

| <span data-ttu-id="c5191-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c5191-118">Name</span></span>          | <span data-ttu-id="c5191-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5191-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c5191-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5191-120">Authorization</span></span> | <span data-ttu-id="c5191-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5191-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="c5191-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="c5191-123">Content-type</span></span> | <span data-ttu-id="c5191-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5191-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5191-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5191-126">Request body</span></span>

<span data-ttu-id="c5191-127">No corpo da solicitação, forneça uma representação JSON do objeto [userflow](../resources/identityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="c5191-127">In the request body, supply a JSON representation of [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c5191-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5191-128">Response</span></span>

<span data-ttu-id="c5191-129">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [userflow](../resources/identityuserflow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5191-129">If successful, this method returns a `201 Created` response code and a new [userFlow](../resources/identityuserflow.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c5191-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c5191-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c5191-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5191-131">Request</span></span>

<span data-ttu-id="c5191-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5191-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_identityuserflow_from_identitycontainer"
}-->

```http
POST https://graph.microsoft.com/beta/identity/userFlows
Content-type: application/json

{
  "userFlowType": "signUpOrSignIn",
  "userFlowTypeVersion": 1
}
```

### <a name="response"></a><span data-ttu-id="c5191-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5191-133">Response</span></span>

<span data-ttu-id="c5191-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c5191-134">The following is an example of the response.</span></span>

> <span data-ttu-id="c5191-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c5191-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.UserFlow"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "B2C_1_Pol1",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create UserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: create_identityuserflow_from_identitycontainer/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
