---
title: Excluir mailFolder
description: Exclua o mailFolder especificado ou mailSearchFolder.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: e993d4cb770db546a11e80aa9b9fe24501e2b281
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512994"
---
# <a name="delete-mailfolder"></a><span data-ttu-id="007de-103">Excluir mailFolder</span><span class="sxs-lookup"><span data-stu-id="007de-103">Delete mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="007de-104">Exclua o especificado [mailFolder](../resources/mailfolder.md) ou [mailSearchFolder](../resources/mailsearchfolder.md).</span><span class="sxs-lookup"><span data-stu-id="007de-104">Delete the specified [mailFolder](../resources/mailfolder.md) or [mailSearchFolder](../resources/mailsearchfolder.md).</span></span>

<span data-ttu-id="007de-105">Você pode especificar uma pasta de email por sua ID de pasta, ou por seu [nome da pasta conhecido](../resources/mailfolder.md), se houver uma.</span><span class="sxs-lookup"><span data-stu-id="007de-105">You can specify a mail folder by its folder ID, or by its [well-known folder name](../resources/mailfolder.md), if one exists.</span></span> 

><span data-ttu-id="007de-106">**Observação** Você não poderá excluir itens na pasta itens recuperáveis exclusões (representado pelo nome da pasta conhecido `recoverableitemsdeletions`).</span><span class="sxs-lookup"><span data-stu-id="007de-106">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the well-known folder name `recoverableitemsdeletions`).</span></span> <span data-ttu-id="007de-107">Para obter mais informações, consulte [retenção de itens excluídos](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) e [Limpar itens excluídos](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) .</span><span class="sxs-lookup"><span data-stu-id="007de-107">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="007de-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="007de-108">Permissions</span></span>
<span data-ttu-id="007de-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="007de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="007de-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="007de-111">Permission type</span></span>      | <span data-ttu-id="007de-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="007de-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="007de-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="007de-113">Delegated (work or school account)</span></span> | <span data-ttu-id="007de-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="007de-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="007de-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="007de-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="007de-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="007de-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="007de-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="007de-117">Application</span></span> | <span data-ttu-id="007de-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="007de-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="007de-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="007de-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="007de-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="007de-120">Request headers</span></span>
| <span data-ttu-id="007de-121">Nome</span><span class="sxs-lookup"><span data-stu-id="007de-121">Name</span></span>       | <span data-ttu-id="007de-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="007de-122">Type</span></span> | <span data-ttu-id="007de-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="007de-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="007de-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="007de-124">Authorization</span></span>  | <span data-ttu-id="007de-125">string</span><span class="sxs-lookup"><span data-stu-id="007de-125">string</span></span>  | <span data-ttu-id="007de-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="007de-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="007de-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="007de-128">Request body</span></span>
<span data-ttu-id="007de-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="007de-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="007de-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="007de-130">Response</span></span>
<span data-ttu-id="007de-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="007de-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="007de-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="007de-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="007de-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="007de-134">Request</span></span>
<span data-ttu-id="007de-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="007de-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/
```

#### <a name="response"></a><span data-ttu-id="007de-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="007de-136">Response</span></span>
<span data-ttu-id="007de-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="007de-137">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailfolder-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
