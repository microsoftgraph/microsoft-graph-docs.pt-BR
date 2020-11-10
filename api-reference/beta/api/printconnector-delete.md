---
title: Excluir conector
description: Excluir (cancelar o registro) de um conector.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 61a3497f552777928d7454ac717ed1b066835ee0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966899"
---
# <a name="delete-connector"></a><span data-ttu-id="fc6ed-103">Excluir conector</span><span class="sxs-lookup"><span data-stu-id="fc6ed-103">Delete connector</span></span>

<span data-ttu-id="fc6ed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc6ed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc6ed-105">Excluir (cancelar o registro) de um **Reconectador**.</span><span class="sxs-lookup"><span data-stu-id="fc6ed-105">Delete (unregister) a **printConnector**.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc6ed-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fc6ed-106">Permissions</span></span>
<span data-ttu-id="fc6ed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc6ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="fc6ed-109">Para usar o serviço de impressão universal, o usuário ou o locatário do aplicativo deve ter uma assinatura de impressão universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="fc6ed-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="fc6ed-110">O usuário conectado deve ser um [administrador da impressora](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="fc6ed-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="fc6ed-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc6ed-111">Permission type</span></span> | <span data-ttu-id="fc6ed-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fc6ed-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="fc6ed-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc6ed-113">Delegated (work or school account)</span></span>| <span data-ttu-id="fc6ed-114">User.Read</span><span class="sxs-lookup"><span data-stu-id="fc6ed-114">User.Read</span></span> |
|<span data-ttu-id="fc6ed-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc6ed-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc6ed-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc6ed-116">Not Supported.</span></span>|
|<span data-ttu-id="fc6ed-117">Application</span><span class="sxs-lookup"><span data-stu-id="fc6ed-117">Application</span></span>|<span data-ttu-id="fc6ed-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc6ed-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc6ed-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc6ed-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/connectors/{id}
```
## <a name="request-headers"></a><span data-ttu-id="fc6ed-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc6ed-120">Request headers</span></span>
| <span data-ttu-id="fc6ed-121">Nome</span><span class="sxs-lookup"><span data-stu-id="fc6ed-121">Name</span></span>          | <span data-ttu-id="fc6ed-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc6ed-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="fc6ed-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc6ed-123">Authorization</span></span> | <span data-ttu-id="fc6ed-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc6ed-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc6ed-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc6ed-126">Request body</span></span>
<span data-ttu-id="fc6ed-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fc6ed-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc6ed-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc6ed-128">Response</span></span>
<span data-ttu-id="fc6ed-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc6ed-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="error-conditions-and-messages"></a><span data-ttu-id="fc6ed-131">Condições e mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="fc6ed-131">Error conditions and messages</span></span>

|<span data-ttu-id="fc6ed-132">Cenário</span><span class="sxs-lookup"><span data-stu-id="fc6ed-132">Scenario</span></span>|<span data-ttu-id="fc6ed-133">Método</span><span class="sxs-lookup"><span data-stu-id="fc6ed-133">Method</span></span>|<span data-ttu-id="fc6ed-134">Código</span><span class="sxs-lookup"><span data-stu-id="fc6ed-134">Code</span></span>|<span data-ttu-id="fc6ed-135">Mensagem</span><span class="sxs-lookup"><span data-stu-id="fc6ed-135">Message</span></span>|
|--------|------|----|-------|
|<span data-ttu-id="fc6ed-136">O usuário tenta excluir um conector que tem uma ou mais impressoras registradas</span><span class="sxs-lookup"><span data-stu-id="fc6ed-136">User attempts to delete a connector that has one or more printers registered</span></span>|<span data-ttu-id="fc6ed-137">EXCLUIR</span><span class="sxs-lookup"><span data-stu-id="fc6ed-137">DELETE</span></span>|<span data-ttu-id="fc6ed-138">409</span><span class="sxs-lookup"><span data-stu-id="fc6ed-138">409</span></span>|<span data-ttu-id="fc6ed-139">Antes de excluir o conector, cancele o registro das impressoras associadas.</span><span class="sxs-lookup"><span data-stu-id="fc6ed-139">Before deleting the connector, please unregister the associated printers.</span></span>|

## <a name="example"></a><span data-ttu-id="fc6ed-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fc6ed-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fc6ed-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc6ed-141">Request</span></span>
<span data-ttu-id="fc6ed-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc6ed-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fc6ed-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc6ed-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connector"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/connectors/{id}
```
# <a name="c"></a>[<span data-ttu-id="fc6ed-144">C#</span><span class="sxs-lookup"><span data-stu-id="fc6ed-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fc6ed-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc6ed-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fc6ed-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc6ed-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fc6ed-147">Java</span><span class="sxs-lookup"><span data-stu-id="fc6ed-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-connector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fc6ed-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc6ed-148">Response</span></span>
<span data-ttu-id="fc6ed-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fc6ed-149">The following is an example of the response.</span></span>
><span data-ttu-id="fc6ed-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fc6ed-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete connector",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
