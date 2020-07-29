---
title: Atualizar reviewSetQuery
description: Atualiza as propriedades de um objeto reviewSetQuery.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 9ba2a3f51bee694001fde5f7f62f0f452aa0bcff
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509947"
---
# <a name="update-reviewsetquery"></a><span data-ttu-id="b8775-103">Atualizar reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="b8775-103">Update reviewSetQuery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8775-104">Atualizar as propriedades de um [reviewSetQuery](../resources/reviewsetquery.md)de descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="b8775-104">Update the properties of an eDiscovery [reviewSetQuery](../resources/reviewsetquery.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b8775-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8775-105">Permissions</span></span>

<span data-ttu-id="b8775-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8775-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b8775-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8775-108">Permission type</span></span>                        | <span data-ttu-id="b8775-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8775-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b8775-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8775-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b8775-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="b8775-111">User.Read</span></span> |
| <span data-ttu-id="b8775-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8775-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8775-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8775-113">Not supported.</span></span> |
| <span data-ttu-id="b8775-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8775-114">Application</span></span>                            | <span data-ttu-id="b8775-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8775-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8775-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8775-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /compliance/ediscovery/cases/{id}/reviewSets/{id}/queries/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b8775-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8775-117">Request headers</span></span>

| <span data-ttu-id="b8775-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b8775-118">Name</span></span>       | <span data-ttu-id="b8775-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8775-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b8775-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8775-120">Authorization</span></span> | <span data-ttu-id="b8775-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8775-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8775-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8775-123">Request body</span></span>

<span data-ttu-id="b8775-124">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="b8775-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b8775-125">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="b8775-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b8775-126">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b8775-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b8775-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b8775-127">Property</span></span>     | <span data-ttu-id="b8775-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8775-128">Type</span></span>        | <span data-ttu-id="b8775-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8775-129">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b8775-130">displayName</span><span class="sxs-lookup"><span data-stu-id="b8775-130">displayName</span></span> | <span data-ttu-id="b8775-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8775-131">String</span></span> | <span data-ttu-id="b8775-132">Nome para exibição para a consulta de conjunto de análise.</span><span class="sxs-lookup"><span data-stu-id="b8775-132">Display name for they review set query.</span></span> |
| <span data-ttu-id="b8775-133">consulta</span><span class="sxs-lookup"><span data-stu-id="b8775-133">query</span></span> | <span data-ttu-id="b8775-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8775-134">String</span></span> | <span data-ttu-id="b8775-135">A cadeia de caracteres de consulta na consulta KQL (linguagem de consulta de palavra-chave).</span><span class="sxs-lookup"><span data-stu-id="b8775-135">The query string in KQL (Keyword Query Language) query.</span></span> <span data-ttu-id="b8775-136">Para obter detalhes, consulte [Document Metadata Fields](https://docs.microsoft.com/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery).</span><span class="sxs-lookup"><span data-stu-id="b8775-136">For details, see [Document metadata fields](https://docs.microsoft.com/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery).</span></span> |

## <a name="response"></a><span data-ttu-id="b8775-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8775-137">Response</span></span>

<span data-ttu-id="b8775-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8775-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b8775-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b8775-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b8775-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8775-141">Request</span></span>

<span data-ttu-id="b8775-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8775-142">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_reviewsetquery"
}-->

```http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets('b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries/6b5358b0-2ce2-4369-b9cf-65392fe56807
Content-type: application/json

{
  "displayName": "My Query 1 - Renamed"
}
```

### <a name="response"></a><span data-ttu-id="b8775-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8775-143">Response</span></span>

<span data-ttu-id="b8775-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b8775-144">The following is an example of the response.</span></span>

> <span data-ttu-id="b8775-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8775-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reviewSetQuery"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update reviewsetquery",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
