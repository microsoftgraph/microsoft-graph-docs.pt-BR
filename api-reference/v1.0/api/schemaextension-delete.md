---
title: Excluir schemaExtension
description: Exclui uma definição da extensão de esquema.
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: 5ae6f367d271db9dfb16a5cc490653ccb9db6784
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33603401"
---
# <a name="delete-schemaextension"></a><span data-ttu-id="70dfc-103">Excluir schemaExtension</span><span class="sxs-lookup"><span data-stu-id="70dfc-103">Delete schemaExtension</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70dfc-104">Exclui uma definição da [extensão de esquema](../resources/schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="70dfc-104">Delete the definition of a [schema extension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="70dfc-p101">Somente o aplicativo que criou a extensão de esquema (proprietário do aplicativo) pode excluir a definição da extensão de esquema e apenas quando a extensão estiver com o status **InDevelopment**. Excluir uma definição da extensão de esquema não afeta o acesso aos dados personalizados que foram adicionados às instâncias de recursos com base nessa definição.</span><span class="sxs-lookup"><span data-stu-id="70dfc-p101">Only the app that created the schema extension (owner app) can delete the schema extension definition, and only when the extension is in the **InDevelopment** state. Deleting a schema extension definition does not affect accessing custom data that has been added to resource instances based on that definition.</span></span>


## <a name="permissions"></a><span data-ttu-id="70dfc-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="70dfc-107">Permissions</span></span>
<span data-ttu-id="70dfc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70dfc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="70dfc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="70dfc-110">Permission type</span></span>      | <span data-ttu-id="70dfc-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="70dfc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70dfc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="70dfc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="70dfc-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="70dfc-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="70dfc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="70dfc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70dfc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70dfc-115">Not supported.</span></span>    |
|<span data-ttu-id="70dfc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="70dfc-116">Application</span></span> | <span data-ttu-id="70dfc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70dfc-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="70dfc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="70dfc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /schemaExtensions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="70dfc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="70dfc-119">Request headers</span></span>
| <span data-ttu-id="70dfc-120">Nome</span><span class="sxs-lookup"><span data-stu-id="70dfc-120">Name</span></span>      |<span data-ttu-id="70dfc-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="70dfc-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="70dfc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="70dfc-122">Authorization</span></span>  | <span data-ttu-id="70dfc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70dfc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="70dfc-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="70dfc-125">Request body</span></span>
<span data-ttu-id="70dfc-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="70dfc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70dfc-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="70dfc-127">Response</span></span>

<span data-ttu-id="70dfc-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70dfc-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70dfc-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="70dfc-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="70dfc-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70dfc-131">Request</span></span>
<span data-ttu-id="70dfc-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="70dfc-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/schemaExtensions/{id}
```
##### <a name="response"></a><span data-ttu-id="70dfc-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="70dfc-133">Response</span></span>
<span data-ttu-id="70dfc-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70dfc-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="70dfc-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="70dfc-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="70dfc-136">Basic</span><span class="sxs-lookup"><span data-stu-id="70dfc-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_schemaextension-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="70dfc-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70dfc-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_schemaextension-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="70dfc-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="70dfc-138">See also</span></span>

- [<span data-ttu-id="70dfc-139">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="70dfc-139">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="70dfc-140">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="70dfc-140">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

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
    "Error: /api-reference/beta/api/schemaextension-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/schemaextension-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
