---
title: Excluir inferenceClassificationOverride
description: Excluir uma substituição de caixa de entrada destaques especificada por sua ID.
localization_priority: Normal
ms.openlocfilehash: 8c9213f48a0d7cc430b0177d6c3d3ff30819202e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328603"
---
# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="67f52-103">Excluir inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="67f52-103">Delete inferenceClassificationOverride</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67f52-104">Excluir uma substituição de [caixa de entrada destaques](../resources/manage-focused-inbox.md) especificada por sua ID.</span><span class="sxs-lookup"><span data-stu-id="67f52-104">Delete a [Focused Inbox](../resources/manage-focused-inbox.md) override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="67f52-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="67f52-105">Permissions</span></span>
<span data-ttu-id="67f52-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67f52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67f52-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67f52-108">Permission type</span></span>      | <span data-ttu-id="67f52-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="67f52-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67f52-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67f52-110">Delegated (work or school account)</span></span> | <span data-ttu-id="67f52-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67f52-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="67f52-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67f52-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67f52-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67f52-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="67f52-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67f52-114">Application</span></span> | <span data-ttu-id="67f52-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67f52-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="67f52-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67f52-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="67f52-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67f52-117">Request headers</span></span>
| <span data-ttu-id="67f52-118">Nome</span><span class="sxs-lookup"><span data-stu-id="67f52-118">Name</span></span>       | <span data-ttu-id="67f52-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="67f52-119">Type</span></span> | <span data-ttu-id="67f52-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="67f52-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="67f52-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="67f52-121">Authorization</span></span>  | <span data-ttu-id="67f52-122">string</span><span class="sxs-lookup"><span data-stu-id="67f52-122">string</span></span>  | <span data-ttu-id="67f52-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67f52-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="67f52-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67f52-125">Request body</span></span>
<span data-ttu-id="67f52-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="67f52-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67f52-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="67f52-127">Response</span></span>

<span data-ttu-id="67f52-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67f52-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67f52-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67f52-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="67f52-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67f52-131">Request</span></span>
<span data-ttu-id="67f52-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="67f52-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
##### <a name="response"></a><span data-ttu-id="67f52-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="67f52-133">Response</span></span>
<span data-ttu-id="67f52-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="67f52-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
