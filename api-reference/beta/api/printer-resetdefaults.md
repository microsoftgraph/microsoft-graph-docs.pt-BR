---
title: 'impressora: resetDefaults'
description: Redefinir as configurações padrão de uma impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: fab03a23e05b0077a8556f8f546f8ba83c4889d7
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48315252"
---
# <a name="printer-resetdefaults"></a><span data-ttu-id="a99be-103">impressora: resetDefaults</span><span class="sxs-lookup"><span data-stu-id="a99be-103">printer: resetDefaults</span></span>

<span data-ttu-id="a99be-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a99be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a99be-105">Redefinir as configurações padrão de uma [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="a99be-105">Reset a [printer](../resources/printer.md)'s default settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="a99be-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a99be-106">Permissions</span></span>
<span data-ttu-id="a99be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a99be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a99be-109">Para usar o serviço de impressão universal, o usuário ou o locatário do aplicativo deve ter uma assinatura de impressão universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="a99be-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="a99be-110">O usuário conectado deve ser um [administrador da impressora](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="a99be-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="a99be-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a99be-111">Permission type</span></span> | <span data-ttu-id="a99be-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a99be-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="a99be-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a99be-113">Delegated (work or school account)</span></span>| <span data-ttu-id="a99be-114">Printer. ReadWrite. All, Printer. FullControl. All</span><span class="sxs-lookup"><span data-stu-id="a99be-114">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="a99be-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a99be-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a99be-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a99be-116">Not Supported.</span></span>|
|<span data-ttu-id="a99be-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a99be-117">Application</span></span>| <span data-ttu-id="a99be-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a99be-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a99be-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a99be-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/resetDefaults
```
## <a name="request-headers"></a><span data-ttu-id="a99be-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a99be-120">Request headers</span></span>
| <span data-ttu-id="a99be-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a99be-121">Name</span></span>          | <span data-ttu-id="a99be-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a99be-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a99be-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a99be-123">Authorization</span></span> | <span data-ttu-id="a99be-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a99be-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a99be-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a99be-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="a99be-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a99be-127">Response</span></span>
<span data-ttu-id="a99be-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a99be-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a99be-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a99be-130">Example</span></span>
<span data-ttu-id="a99be-131">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="a99be-131">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a99be-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a99be-132">Request</span></span>
<span data-ttu-id="a99be-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a99be-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a99be-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a99be-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printer-resetdefaults"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/resetDefaults
```
# <a name="c"></a>[<span data-ttu-id="a99be-135">C#</span><span class="sxs-lookup"><span data-stu-id="a99be-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printer-resetdefaults-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a99be-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a99be-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printer-resetdefaults-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a99be-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a99be-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printer-resetdefaults-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a99be-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a99be-138">Response</span></span>
<span data-ttu-id="a99be-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a99be-139">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printer: resetDefaults",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->