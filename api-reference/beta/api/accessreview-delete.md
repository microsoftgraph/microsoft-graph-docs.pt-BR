---
title: Excluir accessReview
description: No Windows Azure AD para acessar o recurso de revisões, excluir um objeto accessReview.
localization_priority: Normal
ms.openlocfilehash: b062931e58834e1b6a62c83791ec663865fb5c9c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829453"
---
# <a name="delete-accessreview"></a><span data-ttu-id="91126-103">Excluir accessReview</span><span class="sxs-lookup"><span data-stu-id="91126-103">Delete accessReview</span></span>

> <span data-ttu-id="91126-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="91126-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91126-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="91126-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="91126-106">No recurso de [acesso analisa](../resources/accessreviews-root.md) Azure AD, exclua um objeto de [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="91126-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="91126-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="91126-107">Permissions</span></span>
<span data-ttu-id="91126-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91126-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91126-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91126-110">Permission type</span></span>                        | <span data-ttu-id="91126-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="91126-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="91126-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91126-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="91126-113">AccessReview.ReadWrite.All e também devem ter ProgramControl.ReadWrite.All ao cenário completo com uma chamada para excluir um programControl</span><span class="sxs-lookup"><span data-stu-id="91126-113">AccessReview.ReadWrite.All, and should also have ProgramControl.ReadWrite.All to complete scenario with a call to delete a programControl</span></span> |
|<span data-ttu-id="91126-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91126-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91126-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91126-115">Not supported.</span></span> |
|<span data-ttu-id="91126-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91126-116">Application</span></span>                            | <span data-ttu-id="91126-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91126-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="91126-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91126-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="91126-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91126-119">Request headers</span></span>
| <span data-ttu-id="91126-120">Nome</span><span class="sxs-lookup"><span data-stu-id="91126-120">Name</span></span>         | <span data-ttu-id="91126-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="91126-121">Type</span></span>        | <span data-ttu-id="91126-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="91126-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="91126-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="91126-123">Authorization</span></span> | <span data-ttu-id="91126-124">string</span><span class="sxs-lookup"><span data-stu-id="91126-124">string</span></span> | <span data-ttu-id="91126-125">Portador \{token\}.</span><span class="sxs-lookup"><span data-stu-id="91126-125">Bearer \{token\}.</span></span> <span data-ttu-id="91126-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91126-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91126-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91126-127">Request body</span></span>
<span data-ttu-id="91126-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="91126-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="91126-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="91126-129">Response</span></span>
<span data-ttu-id="91126-p104">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91126-p104">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91126-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91126-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91126-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91126-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_accessReview"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')
```
##### <a name="response"></a><span data-ttu-id="91126-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="91126-134">Response</span></span>
><span data-ttu-id="91126-p105">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91126-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
