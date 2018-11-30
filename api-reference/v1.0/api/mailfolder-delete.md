---
title: Excluir mailFolder
description: Exclua o mailFolder especificado.
ms.openlocfilehash: e01f631141147373d1c2010d4313ad833c057df2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007315"
---
# <a name="delete-mailfolder"></a><span data-ttu-id="a9919-103">Excluir mailFolder</span><span class="sxs-lookup"><span data-stu-id="a9919-103">Delete mailFolder</span></span>

<span data-ttu-id="a9919-104">Exclua o especificado [mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="a9919-104">Delete the specified [mailFolder](../resources/mailfolder.md).</span></span>

<span data-ttu-id="a9919-105">Você pode especificar uma pasta de email por sua ID de pasta, ou por seu [nome da pasta conhecido](../resources/mailfolder.md), se houver uma.</span><span class="sxs-lookup"><span data-stu-id="a9919-105">You can specify a mail folder by its folder ID, or by its [well-known folder name](../resources/mailfolder.md), if one exists.</span></span> 

><span data-ttu-id="a9919-106">**Observação** Você não poderá excluir itens na pasta itens recuperáveis exclusões (representado pelo nome da pasta conhecido `recoverableitemsdeletions`).</span><span class="sxs-lookup"><span data-stu-id="a9919-106">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the well-known folder name `recoverableitemsdeletions`).</span></span> <span data-ttu-id="a9919-107">Para obter mais informações, consulte [retenção de itens excluídos](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) e [Limpar itens excluídos](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) .</span><span class="sxs-lookup"><span data-stu-id="a9919-107">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9919-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="a9919-108">Permissions</span></span>
<span data-ttu-id="a9919-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9919-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9919-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9919-111">Permission type</span></span>      | <span data-ttu-id="a9919-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a9919-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9919-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9919-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a9919-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a9919-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a9919-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9919-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9919-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a9919-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a9919-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9919-117">Application</span></span> | <span data-ttu-id="a9919-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a9919-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9919-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9919-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a9919-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9919-120">Request headers</span></span>
| <span data-ttu-id="a9919-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a9919-121">Name</span></span>       | <span data-ttu-id="a9919-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9919-122">Type</span></span> | <span data-ttu-id="a9919-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9919-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a9919-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9919-124">Authorization</span></span>  | <span data-ttu-id="a9919-125">string</span><span class="sxs-lookup"><span data-stu-id="a9919-125">string</span></span>  | <span data-ttu-id="a9919-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9919-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9919-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9919-128">Request body</span></span>
<span data-ttu-id="a9919-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a9919-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9919-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9919-130">Response</span></span>

<span data-ttu-id="a9919-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9919-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9919-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9919-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a9919-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9919-134">Request</span></span>
<span data-ttu-id="a9919-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9919-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="a9919-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9919-136">Response</span></span>
<span data-ttu-id="a9919-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9919-137">Here is an example of the response.</span></span> 
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
  "description": "Delete mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->