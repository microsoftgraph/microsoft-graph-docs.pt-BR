---
title: Parar accessReview
description: No Windows Azure AD para acessar o recurso de revisões, parar uma accessReview ativa no momento.  O objeto de destino pode ser uma revisão de acesso de uma única vez, ou uma instância de uma análise mais acesso recorrente.  (Para impedir que uma análise mais acesso recorrente iniciando a instâncias futuras, atualizá-lo para alterar sua data de término agendada).  Após o acesso revisar paradas, revisores não podem dar entrada e as decisões de revisão de acesso podem ser aplicadas.
localization_priority: Normal
ms.openlocfilehash: 57c0473b58b8ca4bbbb4e9f182b7da4582af4c38
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860113"
---
# <a name="stop-accessreview"></a><span data-ttu-id="a942e-106">Parar accessReview</span><span class="sxs-lookup"><span data-stu-id="a942e-106">Stop accessReview</span></span>

> <span data-ttu-id="a942e-107">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a942e-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a942e-108">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a942e-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a942e-109">O recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, pare de um ativo no momento [accessReview](../resources/accessreview.md).</span><span class="sxs-lookup"><span data-stu-id="a942e-109">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, stop a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="a942e-110">O objeto de destino pode ser uma revisão de acesso de uma única vez, ou uma instância de uma análise mais acesso recorrente.</span><span class="sxs-lookup"><span data-stu-id="a942e-110">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="a942e-111">(Para impedir que uma análise mais acesso recorrente iniciando a instâncias futuras, [atualizá-la](accessreview-update.md) para alterar sua data de término agendada).</span><span class="sxs-lookup"><span data-stu-id="a942e-111">(To prevent a recurring access review from starting future instances, [update it](accessreview-update.md) to change its scheduled end date).</span></span>  <span data-ttu-id="a942e-112">Após o acesso revisar paradas, revisores não podem dar entrada e as decisões de revisão de acesso podem ser aplicadas.</span><span class="sxs-lookup"><span data-stu-id="a942e-112">After the access review stops, reviewers can no longer give input, and the access review decisions can be applied.</span></span>
## <a name="permissions"></a><span data-ttu-id="a942e-113">Permissions</span><span class="sxs-lookup"><span data-stu-id="a942e-113">Permissions</span></span>
<span data-ttu-id="a942e-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a942e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a942e-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a942e-116">Permission type</span></span>                        | <span data-ttu-id="a942e-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a942e-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a942e-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a942e-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="a942e-119">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a942e-119">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="a942e-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a942e-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a942e-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a942e-121">Not supported.</span></span> |
|<span data-ttu-id="a942e-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a942e-122">Application</span></span>                            | <span data-ttu-id="a942e-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a942e-123">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a942e-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a942e-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/stop()
```
## <a name="request-headers"></a><span data-ttu-id="a942e-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a942e-125">Request headers</span></span>
| <span data-ttu-id="a942e-126">Nome</span><span class="sxs-lookup"><span data-stu-id="a942e-126">Name</span></span>         | <span data-ttu-id="a942e-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="a942e-127">Type</span></span>        | <span data-ttu-id="a942e-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="a942e-128">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a942e-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="a942e-129">Authorization</span></span> | <span data-ttu-id="a942e-130">string</span><span class="sxs-lookup"><span data-stu-id="a942e-130">string</span></span> | <span data-ttu-id="a942e-131">Portador \{token\}.</span><span class="sxs-lookup"><span data-stu-id="a942e-131">Bearer \{token\}.</span></span> <span data-ttu-id="a942e-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a942e-132">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a942e-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a942e-133">Request body</span></span>
<span data-ttu-id="a942e-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a942e-134">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="a942e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a942e-135">Response</span></span>
<span data-ttu-id="a942e-p106">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a942e-p106">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a942e-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a942e-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a942e-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a942e-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "stop_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/stop()
```
##### <a name="response"></a><span data-ttu-id="a942e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a942e-140">Response</span></span>
><span data-ttu-id="a942e-p107">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a942e-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Stop accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
