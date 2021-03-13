---
title: Criar directReport
description: Use essa API para criar um novo directReport.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: bd228b01123fa893a320a8a273eca379432b4b7e
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761003"
---
# <a name="create-directreport"></a><span data-ttu-id="cea14-103">Criar directReport</span><span class="sxs-lookup"><span data-stu-id="cea14-103">Create directReport</span></span>

<span data-ttu-id="cea14-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cea14-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cea14-105">Use essa API para criar um novo directReport.</span><span class="sxs-lookup"><span data-stu-id="cea14-105">Use this API to create a new directReport.</span></span>
## <a name="permissions"></a><span data-ttu-id="cea14-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cea14-106">Permissions</span></span>
<span data-ttu-id="cea14-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cea14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cea14-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cea14-109">Permission type</span></span>      | <span data-ttu-id="cea14-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cea14-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cea14-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cea14-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cea14-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cea14-112">Not supported.</span></span>    |
|<span data-ttu-id="cea14-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cea14-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cea14-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cea14-114">Not supported.</span></span>    |
|<span data-ttu-id="cea14-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cea14-115">Application</span></span> | <span data-ttu-id="cea14-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cea14-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cea14-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cea14-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/directReports

```
## <a name="request-headers"></a><span data-ttu-id="cea14-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cea14-118">Request headers</span></span>
| <span data-ttu-id="cea14-119">Nome</span><span class="sxs-lookup"><span data-stu-id="cea14-119">Name</span></span>       | <span data-ttu-id="cea14-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="cea14-120">Type</span></span> | <span data-ttu-id="cea14-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="cea14-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cea14-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cea14-122">Authorization</span></span>  | <span data-ttu-id="cea14-123">string</span><span class="sxs-lookup"><span data-stu-id="cea14-123">string</span></span>  | <span data-ttu-id="cea14-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cea14-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cea14-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cea14-126">Request body</span></span>
<span data-ttu-id="cea14-127">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="cea14-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cea14-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="cea14-128">Response</span></span>

<span data-ttu-id="cea14-129">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cea14-129">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cea14-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cea14-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cea14-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cea14-131">Request</span></span>
<span data-ttu-id="cea14-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cea14-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cea14-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="cea14-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_orgcontact"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/directReports
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="cea14-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cea14-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="cea14-135">C#</span><span class="sxs-lookup"><span data-stu-id="cea14-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="cea14-136">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="cea14-136">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="cea14-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="cea14-137">Response</span></span>
<span data-ttu-id="cea14-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cea14-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create directReport",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


