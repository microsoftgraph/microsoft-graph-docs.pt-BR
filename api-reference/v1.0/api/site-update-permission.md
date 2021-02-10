---
title: Atualizar permissão
description: Atualize o objeto permission em um site.
author: BarrySh
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: c2942645dd2f4faa905f1ccfc87a6aa44132ecef
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162082"
---
# <a name="update-permission"></a><span data-ttu-id="8fdfb-103">Atualizar permissão</span><span class="sxs-lookup"><span data-stu-id="8fdfb-103">Update permission</span></span>
<span data-ttu-id="8fdfb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8fdfb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8fdfb-105">Atualize [o objeto](../resources/permission.md) permission em um site.</span><span class="sxs-lookup"><span data-stu-id="8fdfb-105">Update the [permission](../resources/permission.md) object on a site.</span></span>

## <a name="permissions"></a><span data-ttu-id="8fdfb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8fdfb-106">Permissions</span></span>
<span data-ttu-id="8fdfb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fdfb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fdfb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8fdfb-109">Permission type</span></span>                        | <span data-ttu-id="8fdfb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8fdfb-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="8fdfb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8fdfb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8fdfb-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8fdfb-112">Not supported.</span></span>
|<span data-ttu-id="8fdfb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8fdfb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8fdfb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8fdfb-114">Not supported.</span></span>
|<span data-ttu-id="8fdfb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8fdfb-115">Application</span></span>                            | <span data-ttu-id="8fdfb-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="8fdfb-116">Sites.FullControl.All</span></span>

## <a name="http-request"></a><span data-ttu-id="8fdfb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8fdfb-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /sites/{sitesId}/permissions/{permissionId}
```

## <a name="request-headers"></a><span data-ttu-id="8fdfb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8fdfb-118">Request headers</span></span>
|<span data-ttu-id="8fdfb-119">Nome</span><span class="sxs-lookup"><span data-stu-id="8fdfb-119">Name</span></span>|<span data-ttu-id="8fdfb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8fdfb-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8fdfb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8fdfb-121">Authorization</span></span>|<span data-ttu-id="8fdfb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8fdfb-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8fdfb-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8fdfb-124">Content-Type</span></span>|<span data-ttu-id="8fdfb-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8fdfb-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fdfb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8fdfb-127">Request body</span></span>
<span data-ttu-id="8fdfb-128">No corpo da solicitação, fornece uma representação JSON do [objeto permission.](../resources/permission.md)</span><span class="sxs-lookup"><span data-stu-id="8fdfb-128">In the request body, supply a JSON representation of the [permission](../resources/permission.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8fdfb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fdfb-129">Response</span></span>

<span data-ttu-id="8fdfb-130">Se bem-sucedido, este método retorna `200 OK` um código de resposta e um objeto [de](../resources/permission.md) permissão no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8fdfb-130">If successful, this method returns a `200 OK` response code and a [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8fdfb-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8fdfb-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8fdfb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8fdfb-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_permission_from_"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/sites/{sitesId}/permissions/{permissionId}
Content-Type: application/json

{
  "roles": ["read"]
}
```


### <a name="response"></a><span data-ttu-id="8fdfb-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fdfb-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "2",
    "roles": ["read"],
    "grantedToIdentities": [{
      "application": {
        "id": "89ea5c94-7736-4e25-95ad-3fa95f62b66e",
        "displayName": "Bar App"
      }
    }]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Permissions/Update site permission",
  "suppressions": [
  ]
} -->
