---
title: Excluir contrato
description: Excluir um objeto agreement.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: e01cd007ae2fa0547211f79572db388174c525d8
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722523"
---
# <a name="delete-agreement"></a><span data-ttu-id="6518c-103">Excluir contrato</span><span class="sxs-lookup"><span data-stu-id="6518c-103">Delete agreement</span></span>

<span data-ttu-id="6518c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6518c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6518c-105">Excluir um [objeto agreement.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="6518c-105">Delete an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6518c-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="6518c-106">Permissions</span></span>
<span data-ttu-id="6518c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6518c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6518c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6518c-109">Permission type</span></span>                        | <span data-ttu-id="6518c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6518c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6518c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6518c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6518c-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6518c-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="6518c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6518c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6518c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6518c-114">Not supported.</span></span> |
|<span data-ttu-id="6518c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6518c-115">Application</span></span>                            | <span data-ttu-id="6518c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6518c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6518c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6518c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /identityGovernance/termsOfUse/agreements/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6518c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6518c-118">Request headers</span></span>
| <span data-ttu-id="6518c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6518c-119">Name</span></span>         | <span data-ttu-id="6518c-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="6518c-120">Type</span></span>        | <span data-ttu-id="6518c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6518c-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="6518c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6518c-122">Authorization</span></span> | <span data-ttu-id="6518c-123">string</span><span class="sxs-lookup"><span data-stu-id="6518c-123">string</span></span> | <span data-ttu-id="6518c-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6518c-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6518c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6518c-126">Request body</span></span>
<span data-ttu-id="6518c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6518c-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="6518c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6518c-128">Response</span></span>
<span data-ttu-id="6518c-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6518c-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6518c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6518c-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="6518c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6518c-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_agreement"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/identityGovernance/termsOfUse/agreements/093b947f-8363-4979-a47d-4c52b33ee1be
```

### <a name="response"></a><span data-ttu-id="6518c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6518c-133">Response</span></span>
><span data-ttu-id="6518c-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6518c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


