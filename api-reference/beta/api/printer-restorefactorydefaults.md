---
title: 'printer: restoreFactoryDefaults'
description: Redefinir as configurações padrão de uma impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 87e31568dcbe17ec4bd5e3017e852fb17c6f9989
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786450"
---
# <a name="printer-restorefactorydefaults"></a><span data-ttu-id="44aff-103">printer: restoreFactoryDefaults</span><span class="sxs-lookup"><span data-stu-id="44aff-103">printer: restoreFactoryDefaults</span></span>

<span data-ttu-id="44aff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44aff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44aff-105">Restaure [as configurações](../resources/printer.md)padrão de uma impressora para os valores especificados pelo fabricante.</span><span class="sxs-lookup"><span data-stu-id="44aff-105">Restore a [printer](../resources/printer.md)'s default settings to the values specified by the manufacturer.</span></span>

## <a name="permissions"></a><span data-ttu-id="44aff-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="44aff-106">Permissions</span></span>
<span data-ttu-id="44aff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44aff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="44aff-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="44aff-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="44aff-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="44aff-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="44aff-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="44aff-111">Permission type</span></span> | <span data-ttu-id="44aff-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="44aff-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="44aff-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="44aff-113">Delegated (work or school account)</span></span>| <span data-ttu-id="44aff-114">Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="44aff-114">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="44aff-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="44aff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44aff-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44aff-116">Not Supported.</span></span>|
|<span data-ttu-id="44aff-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="44aff-117">Application</span></span>| <span data-ttu-id="44aff-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44aff-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="44aff-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="44aff-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/restoreFactoryDefaults
```
## <a name="request-headers"></a><span data-ttu-id="44aff-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="44aff-120">Request headers</span></span>
| <span data-ttu-id="44aff-121">Nome</span><span class="sxs-lookup"><span data-stu-id="44aff-121">Name</span></span>          | <span data-ttu-id="44aff-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="44aff-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="44aff-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="44aff-123">Authorization</span></span> | <span data-ttu-id="44aff-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="44aff-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="44aff-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="44aff-126">Request body</span></span>
<span data-ttu-id="44aff-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="44aff-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44aff-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="44aff-128">Response</span></span>
<span data-ttu-id="44aff-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="44aff-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44aff-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="44aff-131">Example</span></span>
<span data-ttu-id="44aff-132">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="44aff-132">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="44aff-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="44aff-133">Request</span></span>
<span data-ttu-id="44aff-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="44aff-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="44aff-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="44aff-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printer-restorefactorydefaults"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/restoreFactoryDefaults
```
# <a name="c"></a>[<span data-ttu-id="44aff-136">C#</span><span class="sxs-lookup"><span data-stu-id="44aff-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printer-restorefactorydefaults-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44aff-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44aff-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printer-restorefactorydefaults-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44aff-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44aff-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printer-restorefactorydefaults-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="44aff-139">Java</span><span class="sxs-lookup"><span data-stu-id="44aff-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printer-restorefactorydefaults-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="44aff-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="44aff-140">Response</span></span>
<span data-ttu-id="44aff-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="44aff-141">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printer: restoreFactoryDefaults",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
