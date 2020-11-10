---
title: 'impressora: restoreFactoryDefaults'
description: Redefinir as configurações padrão de uma impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 962e8df0d6afd29921ac60969c0585adb1035bef
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979785"
---
# <a name="printer-restorefactorydefaults"></a><span data-ttu-id="a8f8f-103">impressora: restoreFactoryDefaults</span><span class="sxs-lookup"><span data-stu-id="a8f8f-103">printer: restoreFactoryDefaults</span></span>

<span data-ttu-id="a8f8f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8f8f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8f8f-105">Restaurar as configurações padrão de uma [impressora](../resources/printer.md)para os valores especificados pelo fabricante.</span><span class="sxs-lookup"><span data-stu-id="a8f8f-105">Restore a [printer](../resources/printer.md)'s default settings to the values specified by the manufacturer.</span></span>

## <a name="permissions"></a><span data-ttu-id="a8f8f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a8f8f-106">Permissions</span></span>
<span data-ttu-id="a8f8f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8f8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a8f8f-109">Para usar o serviço de impressão universal, o usuário ou o locatário do aplicativo deve ter uma assinatura de impressão universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="a8f8f-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="a8f8f-110">O usuário conectado deve ser um [administrador da impressora](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="a8f8f-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="a8f8f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8f8f-111">Permission type</span></span> | <span data-ttu-id="a8f8f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a8f8f-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="a8f8f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8f8f-113">Delegated (work or school account)</span></span>| <span data-ttu-id="a8f8f-114">Printer. ReadWrite. All, Printer. FullControl. All</span><span class="sxs-lookup"><span data-stu-id="a8f8f-114">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="a8f8f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8f8f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8f8f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8f8f-116">Not Supported.</span></span>|
|<span data-ttu-id="a8f8f-117">Application</span><span class="sxs-lookup"><span data-stu-id="a8f8f-117">Application</span></span>| <span data-ttu-id="a8f8f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8f8f-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8f8f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8f8f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/restoreFactoryDefaults
```
## <a name="request-headers"></a><span data-ttu-id="a8f8f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8f8f-120">Request headers</span></span>
| <span data-ttu-id="a8f8f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a8f8f-121">Name</span></span>          | <span data-ttu-id="a8f8f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8f8f-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a8f8f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8f8f-123">Authorization</span></span> | <span data-ttu-id="a8f8f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8f8f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8f8f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8f8f-126">Request body</span></span>
<span data-ttu-id="a8f8f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a8f8f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8f8f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8f8f-128">Response</span></span>
<span data-ttu-id="a8f8f-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8f8f-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8f8f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a8f8f-131">Example</span></span>
<span data-ttu-id="a8f8f-132">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="a8f8f-132">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="a8f8f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8f8f-133">Request</span></span>
<span data-ttu-id="a8f8f-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8f8f-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a8f8f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8f8f-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printer-restorefactorydefaults"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/restoreFactoryDefaults
```
# <a name="c"></a>[<span data-ttu-id="a8f8f-136">C#</span><span class="sxs-lookup"><span data-stu-id="a8f8f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printer-restorefactorydefaults-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a8f8f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8f8f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printer-restorefactorydefaults-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a8f8f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a8f8f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printer-restorefactorydefaults-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a8f8f-139">Java</span><span class="sxs-lookup"><span data-stu-id="a8f8f-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printer-restorefactorydefaults-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a8f8f-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8f8f-140">Response</span></span>
<span data-ttu-id="a8f8f-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a8f8f-141">The following is an example of the response.</span></span> 
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
  "description": "printer: restoreFactoryDefaults",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
