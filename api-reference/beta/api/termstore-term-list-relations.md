---
title: Listar relações
description: Obtenha as relações da propriedade de navegação Relations.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 4389d2522bf394cdc9a871c37f661b1bdcadb016
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539154"
---
# <a name="list-relations"></a><span data-ttu-id="ce874-103">Listar relações</span><span class="sxs-lookup"><span data-stu-id="ce874-103">List relations</span></span>
<span data-ttu-id="ce874-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="ce874-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce874-105">Obtenha a relação diferente de um [termo] ou [conjunto] na propriedade de navegação de relações.</span><span class="sxs-lookup"><span data-stu-id="ce874-105">Get the different relation of a [term] or [set] from the relations navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce874-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ce874-106">Permissions</span></span>
<span data-ttu-id="ce874-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce874-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce874-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce874-109">Permission type</span></span>|<span data-ttu-id="ce874-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ce874-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce874-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce874-111">Delegated (work or school account)</span></span> |<span data-ttu-id="ce874-112">Termos. Read. All, termos. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ce874-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="ce874-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce874-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce874-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce874-114">Not supported.</span></span>    |
|<span data-ttu-id="ce874-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce874-115">Application</span></span> | <span data-ttu-id="ce874-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce874-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="ce874-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce874-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /termStore/sets/{setId}/relations
GET /termStore/sets/{setId}/terms/{termId}/relations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ce874-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ce874-118">Optional query parameters</span></span>
<span data-ttu-id="ce874-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ce874-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ce874-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ce874-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ce874-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce874-121">Request headers</span></span>
|<span data-ttu-id="ce874-122">Nome</span><span class="sxs-lookup"><span data-stu-id="ce874-122">Name</span></span>|<span data-ttu-id="ce874-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce874-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ce874-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce874-124">Authorization</span></span>|<span data-ttu-id="ce874-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce874-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce874-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce874-127">Request body</span></span>
<span data-ttu-id="ce874-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ce874-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce874-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce874-129">Response</span></span>

<span data-ttu-id="ce874-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [relation](../resources/termstore-relation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce874-130">If successful, this method returns a `200 OK` response code and a collection of [relation](../resources/termstore-relation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ce874-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ce874-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ce874-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce874-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_relation"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore/sets/{setId}/relations
```


### <a name="response"></a><span data-ttu-id="ce874-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce874-133">Response</span></span>
<span data-ttu-id="ce874-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ce874-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.termStore.relation)"
}-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "052c749c-749c-052c-9c74-2c059c742c05",
      "relationship": "pin"
    }
  ]
}
```


[set]: ../resources/termstore-set.md
[terminal]: ../resources/termstore-term.md
[term]: ../resources/termstore-term.md
[microsoft.graph.termStore.relation]: ../resources/termstore-relation.md


<!--
{
  "type": "#page.annotation",
  "description": "Create a pinned term entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/term list relations",
  "suppressions": [
  ]
}
-->
