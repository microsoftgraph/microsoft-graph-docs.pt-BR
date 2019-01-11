---
title: Excluir inferenceClassificationOverride
description: Excluir uma substituição de caixa de entrada com foco especificada por sua identificação.
localization_priority: Normal
ms.openlocfilehash: 7db351e11ccfa8e88fe97ff1ee22173a87242d57
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870137"
---
# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="42e28-103">Excluir inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="42e28-103">Delete inferenceClassificationOverride</span></span>

> <span data-ttu-id="42e28-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="42e28-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="42e28-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="42e28-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="42e28-106">Excluir uma substituição de [Caixa de entrada com foco](../resources/manage-focused-inbox.md) especificada por sua identificação.</span><span class="sxs-lookup"><span data-stu-id="42e28-106">Delete a [Focused Inbox](../resources/manage-focused-inbox.md) override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="42e28-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="42e28-107">Permissions</span></span>
<span data-ttu-id="42e28-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42e28-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42e28-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42e28-110">Permission type</span></span>      | <span data-ttu-id="42e28-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="42e28-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42e28-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42e28-112">Delegated (work or school account)</span></span> | <span data-ttu-id="42e28-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42e28-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="42e28-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42e28-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42e28-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42e28-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="42e28-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42e28-116">Application</span></span> | <span data-ttu-id="42e28-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42e28-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="42e28-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42e28-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="42e28-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42e28-119">Request headers</span></span>
| <span data-ttu-id="42e28-120">Nome</span><span class="sxs-lookup"><span data-stu-id="42e28-120">Name</span></span>       | <span data-ttu-id="42e28-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="42e28-121">Type</span></span> | <span data-ttu-id="42e28-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="42e28-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="42e28-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="42e28-123">Authorization</span></span>  | <span data-ttu-id="42e28-124">string</span><span class="sxs-lookup"><span data-stu-id="42e28-124">string</span></span>  | <span data-ttu-id="42e28-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42e28-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42e28-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42e28-127">Request body</span></span>
<span data-ttu-id="42e28-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="42e28-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42e28-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="42e28-129">Response</span></span>

<span data-ttu-id="42e28-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42e28-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42e28-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42e28-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="42e28-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42e28-133">Request</span></span>
<span data-ttu-id="42e28-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42e28-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
##### <a name="response"></a><span data-ttu-id="42e28-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="42e28-135">Response</span></span>
<span data-ttu-id="42e28-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42e28-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
