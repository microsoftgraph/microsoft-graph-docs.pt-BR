---
title: Excluir schemaExtension
description: Exclui uma definição da extensão de esquema.
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: e6f62b570a9befa762ac0f4f05db70cbb13f6c7e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975292"
---
# <a name="delete-schemaextension"></a><span data-ttu-id="4abcd-103">Excluir schemaExtension</span><span class="sxs-lookup"><span data-stu-id="4abcd-103">Delete schemaExtension</span></span>

<span data-ttu-id="4abcd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4abcd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4abcd-105">Exclui uma definição da [extensão de esquema](../resources/schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="4abcd-105">Delete the definition of a [schema extension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="4abcd-p101">Somente o aplicativo que criou a extensão de esquema (proprietário do aplicativo) pode excluir a definição da extensão de esquema e apenas quando a extensão estiver com o status **InDevelopment**. Excluir uma definição da extensão de esquema não afeta o acesso aos dados personalizados que foram adicionados às instâncias de recursos com base nessa definição.</span><span class="sxs-lookup"><span data-stu-id="4abcd-p101">Only the app that created the schema extension (owner app) can delete the schema extension definition, and only when the extension is in the **InDevelopment** state. Deleting a schema extension definition does not affect accessing custom data that has been added to resource instances based on that definition.</span></span>


## <a name="permissions"></a><span data-ttu-id="4abcd-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="4abcd-108">Permissions</span></span>
<span data-ttu-id="4abcd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4abcd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4abcd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4abcd-111">Permission type</span></span>      | <span data-ttu-id="4abcd-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4abcd-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4abcd-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4abcd-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4abcd-114">Application.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4abcd-114">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4abcd-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4abcd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4abcd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4abcd-116">Not supported.</span></span>    |
|<span data-ttu-id="4abcd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4abcd-117">Application</span></span> | <span data-ttu-id="4abcd-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4abcd-118">Not supported.</span></span> |

> [!NOTE]
> <span data-ttu-id="4abcd-119">Além disso, para o fluxo delegado, o usuário conectado só pode excluir schemaExtensionss próprios (onde a propriedade **Owner** do schemaExtension é o `appId` de um aplicativo que o usuário conectado possui).</span><span class="sxs-lookup"><span data-stu-id="4abcd-119">Additionally for the delegated flow, the signed-in user can only delete schemaExtensions they own (where the **owner** property of the schemaExtension is the `appId` of an application the signed-in user owns).</span></span>

## <a name="http-request"></a><span data-ttu-id="4abcd-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4abcd-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /schemaExtensions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4abcd-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4abcd-121">Request headers</span></span>
| <span data-ttu-id="4abcd-122">Nome</span><span class="sxs-lookup"><span data-stu-id="4abcd-122">Name</span></span>      |<span data-ttu-id="4abcd-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="4abcd-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4abcd-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4abcd-124">Authorization</span></span>  | <span data-ttu-id="4abcd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4abcd-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4abcd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4abcd-127">Request body</span></span>
<span data-ttu-id="4abcd-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4abcd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4abcd-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4abcd-129">Response</span></span>

<span data-ttu-id="4abcd-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4abcd-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4abcd-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4abcd-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4abcd-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4abcd-133">Request</span></span>
<span data-ttu-id="4abcd-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4abcd-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4abcd-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="4abcd-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/schemaExtensions/{id}
```
# <a name="c"></a>[<span data-ttu-id="4abcd-136">C#</span><span class="sxs-lookup"><span data-stu-id="4abcd-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4abcd-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4abcd-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4abcd-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4abcd-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4abcd-139">Java</span><span class="sxs-lookup"><span data-stu-id="4abcd-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-schemaextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4abcd-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="4abcd-140">Response</span></span>
<span data-ttu-id="4abcd-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4abcd-141">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="4abcd-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="4abcd-142">See also</span></span>

- [<span data-ttu-id="4abcd-143">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="4abcd-143">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="4abcd-144">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="4abcd-144">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

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


