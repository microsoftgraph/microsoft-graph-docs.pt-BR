---
title: SendReminder accessReview
description: 'No recurso de revisões do Azure AD Access, envie um lembrete para os revisores de um accessReview ativo no momento.  O objeto de destino pode ser uma revisão de acesso única ou uma instância de uma revisão de acesso recorrente. '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ed98f096d1bca4ff3ba9ee3626b457c11c392829
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33323031"
---
# <a name="sendreminder-accessreview"></a><span data-ttu-id="804b3-104">SendReminder accessReview</span><span class="sxs-lookup"><span data-stu-id="804b3-104">SendReminder accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="804b3-105">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , envie um lembrete para os revisores de um [accessReview](../resources/accessreview.md)ativo no momento.</span><span class="sxs-lookup"><span data-stu-id="804b3-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, send a reminder to the reviewers of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="804b3-106">O objeto de destino pode ser uma revisão de acesso única ou uma instância de uma revisão de acesso recorrente.</span><span class="sxs-lookup"><span data-stu-id="804b3-106">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span> 

## <a name="permissions"></a><span data-ttu-id="804b3-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="804b3-107">Permissions</span></span>
<span data-ttu-id="804b3-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="804b3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="804b3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="804b3-110">Permission type</span></span>                        | <span data-ttu-id="804b3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="804b3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="804b3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="804b3-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="804b3-113">AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="804b3-113">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="804b3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="804b3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="804b3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="804b3-115">Not supported.</span></span> |
|<span data-ttu-id="804b3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="804b3-116">Application</span></span>                            | <span data-ttu-id="804b3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="804b3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="804b3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="804b3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/sendReminder()
```
## <a name="request-headers"></a><span data-ttu-id="804b3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="804b3-119">Request headers</span></span>
| <span data-ttu-id="804b3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="804b3-120">Name</span></span>         | <span data-ttu-id="804b3-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="804b3-121">Type</span></span>        | <span data-ttu-id="804b3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="804b3-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="804b3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="804b3-123">Authorization</span></span> | <span data-ttu-id="804b3-124">string</span><span class="sxs-lookup"><span data-stu-id="804b3-124">string</span></span> | <span data-ttu-id="804b3-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="804b3-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="804b3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="804b3-127">Request body</span></span>
<span data-ttu-id="804b3-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="804b3-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="804b3-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="804b3-129">Response</span></span>
<span data-ttu-id="804b3-p105">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="804b3-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="804b3-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="804b3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="804b3-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="804b3-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/sendReminder
```
##### <a name="response"></a><span data-ttu-id="804b3-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="804b3-134">Response</span></span>
><span data-ttu-id="804b3-p106">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="804b3-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "SendReminder accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
