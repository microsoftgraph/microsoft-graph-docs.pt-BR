---
title: Criar permissão
description: Criar um novo objeto de permissão.
author: BarrySh
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 64a62e8a0904cc2be0c3cffde0ff3f1c42ef86db
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162083"
---
# <a name="create-permission"></a><span data-ttu-id="d8f4c-103">Criar permissão</span><span class="sxs-lookup"><span data-stu-id="d8f4c-103">Create permission</span></span>
<span data-ttu-id="d8f4c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8f4c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d8f4c-105">Criar um novo [objeto de](../resources/permission.md) permissão em um site.</span><span class="sxs-lookup"><span data-stu-id="d8f4c-105">Create a new [permission](../resources/permission.md) object on a site.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8f4c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d8f4c-106">Permissions</span></span>
<span data-ttu-id="d8f4c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8f4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8f4c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8f4c-109">Permission type</span></span>                        | <span data-ttu-id="d8f4c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d8f4c-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="d8f4c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8f4c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d8f4c-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8f4c-112">Not supported.</span></span>
|<span data-ttu-id="d8f4c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8f4c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8f4c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8f4c-114">Not supported.</span></span>
|<span data-ttu-id="d8f4c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8f4c-115">Application</span></span>                            | <span data-ttu-id="d8f4c-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="d8f4c-116">Sites.FullControl.All</span></span>

## <a name="http-request"></a><span data-ttu-id="d8f4c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8f4c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /sites/{sitesId}/permissions
```

## <a name="request-headers"></a><span data-ttu-id="d8f4c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8f4c-118">Request headers</span></span>
|<span data-ttu-id="d8f4c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d8f4c-119">Name</span></span>|<span data-ttu-id="d8f4c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8f4c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d8f4c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8f4c-121">Authorization</span></span>|<span data-ttu-id="d8f4c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8f4c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d8f4c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d8f4c-124">Content-Type</span></span>|<span data-ttu-id="d8f4c-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8f4c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8f4c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8f4c-127">Request body</span></span>
<span data-ttu-id="d8f4c-128">No corpo da solicitação, fornece uma representação JSON do [objeto permission.](../resources/permission.md)</span><span class="sxs-lookup"><span data-stu-id="d8f4c-128">In the request body, supply a JSON representation of the [permission](../resources/permission.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d8f4c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8f4c-129">Response</span></span>

<span data-ttu-id="d8f4c-130">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um objeto [de](../resources/permission.md) permissão no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8f4c-130">If successful, this method returns a `201 Created` response code and a [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d8f4c-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d8f4c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d8f4c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8f4c-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_permission_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/sites/{sitesId}/permissions
Content-Type: application/json

{
  "roles": ["write"],
  "grantedToIdentities": [{
    "application": {
      "id": "89ea5c94-7736-4e25-95ad-3fa95f62b66e",
      "displayName": "Foo App"
    }
  }]
}
```


### <a name="response"></a><span data-ttu-id="d8f4c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8f4c-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "id": "1",
    "roles": ["write"],
    "grantedToIdentities": [{
      "application": {
        "id": "89ea5c94-7736-4e25-95ad-3fa95f62b66e",
        "displayName": "Foo App"
      }
    }]
}
```

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Sites/Permissions/Create site permissions"
} -->
