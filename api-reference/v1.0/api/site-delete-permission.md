---
title: Permissão de exclusão
description: Exclua um objeto de permissão em um site.
author: BarrySh
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: d38b92b9d49863810e6aff0bf7eed0d93643f13f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162085"
---
# <a name="delete-permission"></a><span data-ttu-id="9c6c3-103">Permissão de exclusão</span><span class="sxs-lookup"><span data-stu-id="9c6c3-103">Delete permission</span></span>
<span data-ttu-id="9c6c3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c6c3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9c6c3-105">[Exclua um](../resources/permission.md) objeto de permissão em um site.</span><span class="sxs-lookup"><span data-stu-id="9c6c3-105">Delete a [permission](../resources/permission.md) object on a site.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c6c3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9c6c3-106">Permissions</span></span>
<span data-ttu-id="9c6c3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c6c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c6c3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c6c3-109">Permission type</span></span>                        | <span data-ttu-id="9c6c3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9c6c3-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="9c6c3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c6c3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9c6c3-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c6c3-112">Not supported.</span></span>
|<span data-ttu-id="9c6c3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c6c3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c6c3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c6c3-114">Not supported.</span></span>
|<span data-ttu-id="9c6c3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c6c3-115">Application</span></span>                            | <span data-ttu-id="9c6c3-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="9c6c3-116">Sites.FullControl.All</span></span>

## <a name="http-request"></a><span data-ttu-id="9c6c3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c6c3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /sites/{sitesId}/permissions/{permissionId}
```

## <a name="request-headers"></a><span data-ttu-id="9c6c3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c6c3-118">Request headers</span></span>
|<span data-ttu-id="9c6c3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9c6c3-119">Name</span></span>|<span data-ttu-id="9c6c3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c6c3-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9c6c3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c6c3-121">Authorization</span></span>|<span data-ttu-id="9c6c3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c6c3-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c6c3-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c6c3-124">Request body</span></span>
<span data-ttu-id="9c6c3-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9c6c3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c6c3-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c6c3-126">Response</span></span>

<span data-ttu-id="9c6c3-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c6c3-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9c6c3-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9c6c3-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9c6c3-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c6c3-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_permission"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/sites/{sitesId}/permissions/{permissionId}
```


### <a name="response"></a><span data-ttu-id="9c6c3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c6c3-131">Response</span></span>
<span data-ttu-id="9c6c3-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c6c3-132">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Sites/Permissions/Delete site permission"
} -->
