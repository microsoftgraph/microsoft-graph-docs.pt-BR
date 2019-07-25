---
title: Excluir schemaExtension
description: Exclui uma definição da extensão de esquema.
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: c3ce95154319519e7dd6b4353389e392f169de35
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870678"
---
# <a name="delete-schemaextension"></a><span data-ttu-id="cca27-103">Excluir schemaExtension</span><span class="sxs-lookup"><span data-stu-id="cca27-103">Delete schemaExtension</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cca27-104">Exclui uma definição da [extensão de esquema](../resources/schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="cca27-104">Delete the definition of a [schema extension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="cca27-p101">Somente o aplicativo que criou a extensão de esquema (proprietário do aplicativo) pode excluir a definição da extensão de esquema e apenas quando a extensão estiver com o status **InDevelopment**. Excluir uma definição da extensão de esquema não afeta o acesso aos dados personalizados que foram adicionados às instâncias de recursos com base nessa definição.</span><span class="sxs-lookup"><span data-stu-id="cca27-p101">Only the app that created the schema extension (owner app) can delete the schema extension definition, and only when the extension is in the **InDevelopment** state. Deleting a schema extension definition does not affect accessing custom data that has been added to resource instances based on that definition.</span></span>


## <a name="permissions"></a><span data-ttu-id="cca27-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="cca27-107">Permissions</span></span>
<span data-ttu-id="cca27-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cca27-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cca27-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cca27-110">Permission type</span></span>      | <span data-ttu-id="cca27-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cca27-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cca27-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cca27-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cca27-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cca27-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cca27-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cca27-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cca27-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cca27-115">Not supported.</span></span>    |
|<span data-ttu-id="cca27-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cca27-116">Application</span></span> | <span data-ttu-id="cca27-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cca27-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cca27-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cca27-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /schemaExtensions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cca27-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cca27-119">Request headers</span></span>
| <span data-ttu-id="cca27-120">Nome</span><span class="sxs-lookup"><span data-stu-id="cca27-120">Name</span></span>      |<span data-ttu-id="cca27-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="cca27-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cca27-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cca27-122">Authorization</span></span>  | <span data-ttu-id="cca27-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cca27-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cca27-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cca27-125">Request body</span></span>
<span data-ttu-id="cca27-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cca27-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cca27-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="cca27-127">Response</span></span>

<span data-ttu-id="cca27-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cca27-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cca27-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cca27-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cca27-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cca27-131">Request</span></span>
<span data-ttu-id="cca27-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cca27-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cca27-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="cca27-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/schemaExtensions/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cca27-134">C#</span><span class="sxs-lookup"><span data-stu-id="cca27-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cca27-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="cca27-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cca27-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="cca27-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cca27-137">Java</span><span class="sxs-lookup"><span data-stu-id="cca27-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-schemaextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cca27-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="cca27-138">Response</span></span>
<span data-ttu-id="cca27-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cca27-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="cca27-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="cca27-140">See also</span></span>

- [<span data-ttu-id="cca27-141">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="cca27-141">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="cca27-142">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="cca27-142">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
