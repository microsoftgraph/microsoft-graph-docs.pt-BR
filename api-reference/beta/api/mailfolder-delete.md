---
title: Excluir mailFolder
description: Exclua o mailFolder especificado ou mailSearchFolder.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 46a47bc10560269ae78977fb6ada1d177c46e45e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851552"
---
# <a name="delete-mailfolder"></a><span data-ttu-id="eecb4-103">Excluir mailFolder</span><span class="sxs-lookup"><span data-stu-id="eecb4-103">Delete mailFolder</span></span>

> <span data-ttu-id="eecb4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="eecb4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eecb4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="eecb4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eecb4-106">Exclua o especificado [mailFolder](../resources/mailfolder.md) ou [mailSearchFolder](../resources/mailsearchfolder.md).</span><span class="sxs-lookup"><span data-stu-id="eecb4-106">Delete the specified [mailFolder](../resources/mailfolder.md) or [mailSearchFolder](../resources/mailsearchfolder.md).</span></span>

<span data-ttu-id="eecb4-107">Você pode especificar uma pasta de email por sua ID de pasta, ou por seu [nome da pasta conhecido](../resources/mailfolder.md), se houver uma.</span><span class="sxs-lookup"><span data-stu-id="eecb4-107">You can specify a mail folder by its folder ID, or by its [well-known folder name](../resources/mailfolder.md), if one exists.</span></span> 

><span data-ttu-id="eecb4-108">**Observação** Você não poderá excluir itens na pasta itens recuperáveis exclusões (representado pelo nome da pasta conhecido `recoverableitemsdeletions`).</span><span class="sxs-lookup"><span data-stu-id="eecb4-108">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the well-known folder name `recoverableitemsdeletions`).</span></span> <span data-ttu-id="eecb4-109">Para obter mais informações, consulte [retenção de itens excluídos](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) e [Limpar itens excluídos](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) .</span><span class="sxs-lookup"><span data-stu-id="eecb4-109">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="eecb4-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="eecb4-110">Permissions</span></span>
<span data-ttu-id="eecb4-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eecb4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eecb4-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eecb4-113">Permission type</span></span>      | <span data-ttu-id="eecb4-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eecb4-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eecb4-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eecb4-115">Delegated (work or school account)</span></span> | <span data-ttu-id="eecb4-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eecb4-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="eecb4-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eecb4-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eecb4-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eecb4-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="eecb4-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eecb4-119">Application</span></span> | <span data-ttu-id="eecb4-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eecb4-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="eecb4-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eecb4-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="eecb4-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eecb4-122">Request headers</span></span>
| <span data-ttu-id="eecb4-123">Nome</span><span class="sxs-lookup"><span data-stu-id="eecb4-123">Name</span></span>       | <span data-ttu-id="eecb4-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="eecb4-124">Type</span></span> | <span data-ttu-id="eecb4-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="eecb4-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="eecb4-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="eecb4-126">Authorization</span></span>  | <span data-ttu-id="eecb4-127">string</span><span class="sxs-lookup"><span data-stu-id="eecb4-127">string</span></span>  | <span data-ttu-id="eecb4-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eecb4-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eecb4-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eecb4-130">Request body</span></span>
<span data-ttu-id="eecb4-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eecb4-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eecb4-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="eecb4-132">Response</span></span>
<span data-ttu-id="eecb4-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eecb4-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eecb4-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eecb4-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="eecb4-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eecb4-136">Request</span></span>
<span data-ttu-id="eecb4-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="eecb4-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/
```

#### <a name="response"></a><span data-ttu-id="eecb4-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="eecb4-138">Response</span></span>
<span data-ttu-id="eecb4-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="eecb4-139">The following is an example of the response.</span></span> 
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
