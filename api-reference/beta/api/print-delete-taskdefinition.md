---
title: Excluir taskDefinition
description: Excluir uma definição de tarefa.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 23d7438d573cb0ac8ff17c0a9c100bece71bb68c
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091561"
---
# <a name="delete-taskdefinition"></a><span data-ttu-id="d3e3f-103">Excluir taskDefinition</span><span class="sxs-lookup"><span data-stu-id="d3e3f-103">Delete taskDefinition</span></span>

<span data-ttu-id="d3e3f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3e3f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3e3f-105">Excluir um **taskDefinition**.</span><span class="sxs-lookup"><span data-stu-id="d3e3f-105">Delete a **taskDefinition**.</span></span>

<span data-ttu-id="d3e3f-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à impressão universal, consulte [Estendeing universal print to support pull Printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="d3e3f-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="d3e3f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d3e3f-107">Permissions</span></span>
<span data-ttu-id="d3e3f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3e3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d3e3f-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="d3e3f-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="d3e3f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3e3f-111">Permission type</span></span> | <span data-ttu-id="d3e3f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d3e3f-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="d3e3f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3e3f-113">Delegated (work or school account)</span></span>| <span data-ttu-id="d3e3f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3e3f-114">Not supported.</span></span> |
|<span data-ttu-id="d3e3f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3e3f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3e3f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3e3f-116">Not Supported.</span></span>|
|<span data-ttu-id="d3e3f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3e3f-117">Application</span></span>| <span data-ttu-id="d3e3f-118">PrintTaskDefinition. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d3e3f-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3e3f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3e3f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/taskDefinitions/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d3e3f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3e3f-120">Request headers</span></span>
| <span data-ttu-id="d3e3f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d3e3f-121">Name</span></span>          | <span data-ttu-id="d3e3f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3e3f-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d3e3f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3e3f-123">Authorization</span></span> | <span data-ttu-id="d3e3f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3e3f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d3e3f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3e3f-126">Request body</span></span>
<span data-ttu-id="d3e3f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d3e3f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3e3f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3e3f-128">Response</span></span>
<span data-ttu-id="d3e3f-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3e3f-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3e3f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3e3f-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="d3e3f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3e3f-132">Request</span></span>
<span data-ttu-id="d3e3f-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3e3f-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_taskdefinition"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/taskDefinitions/4c6a0f26-8e5d-4bf6-91e6-4a5731adec19
```

---

### <a name="response"></a><span data-ttu-id="d3e3f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3e3f-134">Response</span></span>
<span data-ttu-id="d3e3f-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d3e3f-135">The following is an example of the response.</span></span>
><span data-ttu-id="d3e3f-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3e3f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete taskDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
