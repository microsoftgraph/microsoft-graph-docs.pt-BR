---
title: Atualizar synchronizationtemplate
description: Atualizar (substituir) o modelo de sincronização associado a um determinado aplicativo.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 67892e838d4d4ebad1d0caa282a3c85467185c4f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869033"
---
# <a name="update-synchronizationtemplate"></a><span data-ttu-id="0382a-103">Atualizar synchronizationtemplate</span><span class="sxs-lookup"><span data-stu-id="0382a-103">Update synchronizationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0382a-104">Atualizar (substituir) o modelo de sincronização associado a um determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0382a-104">Update (override) the synchronization template associated with a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="0382a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0382a-105">Permissions</span></span>
<span data-ttu-id="0382a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0382a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0382a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0382a-108">Permission type</span></span>                        | <span data-ttu-id="0382a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0382a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0382a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0382a-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="0382a-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0382a-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="0382a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0382a-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="0382a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0382a-113">Not supported.</span></span>|
|<span data-ttu-id="0382a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0382a-114">Application</span></span>                            |<span data-ttu-id="0382a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0382a-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="0382a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0382a-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT application/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="0382a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0382a-117">Request headers</span></span>

| <span data-ttu-id="0382a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="0382a-118">Name</span></span>           | <span data-ttu-id="0382a-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="0382a-119">Type</span></span>    | <span data-ttu-id="0382a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0382a-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="0382a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0382a-121">Authorization</span></span>  | <span data-ttu-id="0382a-122">string</span><span class="sxs-lookup"><span data-stu-id="0382a-122">string</span></span>  | <span data-ttu-id="0382a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0382a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0382a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0382a-125">Request body</span></span>

<span data-ttu-id="0382a-126">No corpo da solicitação, forneça o [](../resources/synchronization-synchronizationtemplate.md) objeto synchronizationtemplate para substituir o modelo existente.</span><span class="sxs-lookup"><span data-stu-id="0382a-126">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to replace the existing template.</span></span> <span data-ttu-id="0382a-127">Certifique-se de que todas as propriedades sejam fornecidas.</span><span class="sxs-lookup"><span data-stu-id="0382a-127">Make sure all properties are provided.</span></span> <span data-ttu-id="0382a-128">As propriedades ausentes serão apagadas.</span><span class="sxs-lookup"><span data-stu-id="0382a-128">Missing properties will be erased.</span></span>

### <a name="response"></a><span data-ttu-id="0382a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0382a-129">Response</span></span>

<span data-ttu-id="0382a-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0382a-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="examples"></a><span data-ttu-id="0382a-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0382a-132">Examples</span></span>

##### <a name="request"></a><span data-ttu-id="0382a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0382a-133">Request</span></span>
<span data-ttu-id="0382a-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="0382a-134">The following is an example of a request.</span></span> 

><span data-ttu-id="0382a-135">**Observação:** O objeto Request mostrado aqui é reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0382a-135">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="0382a-136">Incluir todas as propriedades em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0382a-136">Include all the properties in an actual call.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0382a-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="0382a-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_synchronizationtemplate"
}-->
```http
PUT https://graph.microsoft.com/beta/applications/{id}/synchronization/templates/{templateId}
Authorization: Bearer <token>
Content-type: application/json

{
    "id": "Slack",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0382a-138">C#</span><span class="sxs-lookup"><span data-stu-id="0382a-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-synchronizationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0382a-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="0382a-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-synchronizationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0382a-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0382a-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-synchronizationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0382a-141">Java</span><span class="sxs-lookup"><span data-stu-id="0382a-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-synchronizationtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0382a-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="0382a-142">Response</span></span>
<span data-ttu-id="0382a-143">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="0382a-143">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update synchronizationtemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
