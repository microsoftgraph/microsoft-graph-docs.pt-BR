---
title: Criar memberOf
description: Use esta API para criar um novo memberOf.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a4b0730a7ad65770f31a36d5be39a0cd841c8809
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657151"
---
# <a name="create-memberof"></a><span data-ttu-id="9afdc-103">Criar memberOf</span><span class="sxs-lookup"><span data-stu-id="9afdc-103">Create memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9afdc-104">Use esta API para criar um novo memberOf.</span><span class="sxs-lookup"><span data-stu-id="9afdc-104">Use this API to create a new memberOf.</span></span>
## <a name="permissions"></a><span data-ttu-id="9afdc-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9afdc-105">Permissions</span></span>
<span data-ttu-id="9afdc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9afdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9afdc-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9afdc-108">Permission type</span></span>      | <span data-ttu-id="9afdc-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9afdc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9afdc-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9afdc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9afdc-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9afdc-111">Not supported.</span></span>    |
|<span data-ttu-id="9afdc-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9afdc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9afdc-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9afdc-113">Not supported.</span></span>    |
|<span data-ttu-id="9afdc-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9afdc-114">Application</span></span> | <span data-ttu-id="9afdc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9afdc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9afdc-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9afdc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/memberOf

```
## <a name="request-headers"></a><span data-ttu-id="9afdc-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9afdc-117">Request headers</span></span>
| <span data-ttu-id="9afdc-118">Nome</span><span class="sxs-lookup"><span data-stu-id="9afdc-118">Name</span></span>       | <span data-ttu-id="9afdc-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="9afdc-119">Type</span></span> | <span data-ttu-id="9afdc-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9afdc-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9afdc-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9afdc-121">Authorization</span></span>  | <span data-ttu-id="9afdc-122">string</span><span class="sxs-lookup"><span data-stu-id="9afdc-122">string</span></span>  | <span data-ttu-id="9afdc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9afdc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9afdc-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9afdc-125">Request body</span></span>
<span data-ttu-id="9afdc-126">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="9afdc-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9afdc-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="9afdc-127">Response</span></span>

<span data-ttu-id="9afdc-128">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9afdc-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9afdc-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9afdc-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9afdc-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9afdc-130">Request</span></span>
<span data-ttu-id="9afdc-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9afdc-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_orgcontact"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/memberOf
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
<span data-ttu-id="9afdc-132">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="9afdc-132">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="9afdc-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9afdc-133">Response</span></span>
<span data-ttu-id="9afdc-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9afdc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "directoryObject": {
    "id": "id-value"
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9afdc-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="9afdc-137">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9afdc-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="9afdc-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_orgcontact-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/orgcontact-post-memberof.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
