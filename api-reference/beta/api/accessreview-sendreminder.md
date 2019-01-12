---
title: SendReminder accessReview
description: 'No Windows Azure AD para acessar o recurso de revisões, envie um lembrete para os revisores de um accessReview ativa no momento.  O objeto de destino pode ser uma revisão de acesso de uma única vez, ou uma instância de uma análise mais acesso recorrente. '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cf5b78d2c67993fbf2da9be7c55a07fb752985c7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917276"
---
# <a name="sendreminder-accessreview"></a><span data-ttu-id="91d0f-104">SendReminder accessReview</span><span class="sxs-lookup"><span data-stu-id="91d0f-104">SendReminder accessReview</span></span>

> <span data-ttu-id="91d0f-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="91d0f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91d0f-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="91d0f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="91d0f-107">O recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, envie um lembrete para os revisores de um ativo no momento [accessReview](../resources/accessreview.md).</span><span class="sxs-lookup"><span data-stu-id="91d0f-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, send a reminder to the reviewers of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="91d0f-108">O objeto de destino pode ser uma revisão de acesso de uma única vez, ou uma instância de uma análise mais acesso recorrente.</span><span class="sxs-lookup"><span data-stu-id="91d0f-108">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span> 

## <a name="permissions"></a><span data-ttu-id="91d0f-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="91d0f-109">Permissions</span></span>
<span data-ttu-id="91d0f-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91d0f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91d0f-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91d0f-112">Permission type</span></span>                        | <span data-ttu-id="91d0f-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="91d0f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="91d0f-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91d0f-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="91d0f-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91d0f-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="91d0f-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91d0f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91d0f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91d0f-117">Not supported.</span></span> |
|<span data-ttu-id="91d0f-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91d0f-118">Application</span></span>                            | <span data-ttu-id="91d0f-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91d0f-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="91d0f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91d0f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/sendReminder()
```
## <a name="request-headers"></a><span data-ttu-id="91d0f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91d0f-121">Request headers</span></span>
| <span data-ttu-id="91d0f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="91d0f-122">Name</span></span>         | <span data-ttu-id="91d0f-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="91d0f-123">Type</span></span>        | <span data-ttu-id="91d0f-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="91d0f-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="91d0f-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="91d0f-125">Authorization</span></span> | <span data-ttu-id="91d0f-126">string</span><span class="sxs-lookup"><span data-stu-id="91d0f-126">string</span></span> | <span data-ttu-id="91d0f-127">Portador \{token\}.</span><span class="sxs-lookup"><span data-stu-id="91d0f-127">Bearer \{token\}.</span></span> <span data-ttu-id="91d0f-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91d0f-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91d0f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91d0f-129">Request body</span></span>
<span data-ttu-id="91d0f-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="91d0f-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="91d0f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="91d0f-131">Response</span></span>
<span data-ttu-id="91d0f-p106">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91d0f-p106">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91d0f-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91d0f-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91d0f-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91d0f-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/sendReminder()
```
##### <a name="response"></a><span data-ttu-id="91d0f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="91d0f-136">Response</span></span>
><span data-ttu-id="91d0f-p107">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91d0f-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "SendReminder accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
