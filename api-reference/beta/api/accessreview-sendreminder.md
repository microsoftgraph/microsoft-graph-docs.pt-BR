---
title: SendReminder accessReview
description: 'No Windows Azure AD para acessar o recurso de revisões, envie um lembrete para os revisores de um accessReview ativa no momento.  O objeto de destino pode ser uma revisão de acesso de uma única vez, ou uma instância de uma análise mais acesso recorrente. '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: db394036a228f405a8cebb783a9279779054b04d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518545"
---
# <a name="sendreminder-accessreview"></a><span data-ttu-id="09197-104">SendReminder accessReview</span><span class="sxs-lookup"><span data-stu-id="09197-104">SendReminder accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09197-105">O recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, envie um lembrete para os revisores de um ativo no momento [accessReview](../resources/accessreview.md).</span><span class="sxs-lookup"><span data-stu-id="09197-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, send a reminder to the reviewers of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="09197-106">O objeto de destino pode ser uma revisão de acesso de uma única vez, ou uma instância de uma análise mais acesso recorrente.</span><span class="sxs-lookup"><span data-stu-id="09197-106">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span> 

## <a name="permissions"></a><span data-ttu-id="09197-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="09197-107">Permissions</span></span>
<span data-ttu-id="09197-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09197-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09197-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="09197-110">Permission type</span></span>                        | <span data-ttu-id="09197-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="09197-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="09197-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="09197-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="09197-113">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09197-113">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="09197-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="09197-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09197-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09197-115">Not supported.</span></span> |
|<span data-ttu-id="09197-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="09197-116">Application</span></span>                            | <span data-ttu-id="09197-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09197-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="09197-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="09197-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/sendReminder()
```
## <a name="request-headers"></a><span data-ttu-id="09197-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="09197-119">Request headers</span></span>
| <span data-ttu-id="09197-120">Nome</span><span class="sxs-lookup"><span data-stu-id="09197-120">Name</span></span>         | <span data-ttu-id="09197-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="09197-121">Type</span></span>        | <span data-ttu-id="09197-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="09197-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="09197-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="09197-123">Authorization</span></span> | <span data-ttu-id="09197-124">string</span><span class="sxs-lookup"><span data-stu-id="09197-124">string</span></span> | <span data-ttu-id="09197-125">Token de portador</span><span class="sxs-lookup"><span data-stu-id="09197-125">Bearer \{token\}.</span></span> <span data-ttu-id="09197-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09197-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="09197-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="09197-127">Request body</span></span>
<span data-ttu-id="09197-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="09197-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="09197-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="09197-129">Response</span></span>
<span data-ttu-id="09197-p105">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="09197-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09197-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="09197-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="09197-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09197-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/sendReminder()
```
##### <a name="response"></a><span data-ttu-id="09197-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="09197-134">Response</span></span>
><span data-ttu-id="09197-p106">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="09197-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-sendreminder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
