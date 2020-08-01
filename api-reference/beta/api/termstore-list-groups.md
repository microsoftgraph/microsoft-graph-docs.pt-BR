---
title: Listar grupos
description: Obtenha os grupos da propriedade de navegação grupos.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 477fda55761220d61afc480ab1a8f8304bf879dc
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539178"
---
# <a name="list-groups"></a><span data-ttu-id="074e0-103">Listar grupos</span><span class="sxs-lookup"><span data-stu-id="074e0-103">List groups</span></span>
<span data-ttu-id="074e0-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="074e0-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="074e0-105">Obter a lista de objetos de [grupo](../resources/termstore-group.md) de um [repositório](../resources/termstore-store.md)</span><span class="sxs-lookup"><span data-stu-id="074e0-105">Get the list of [group](../resources/termstore-group.md) objects of a [store](../resources/termstore-store.md)</span></span>

## <a name="permissions"></a><span data-ttu-id="074e0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="074e0-106">Permissions</span></span>
<span data-ttu-id="074e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="074e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="074e0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="074e0-109">Permission type</span></span>|<span data-ttu-id="074e0-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="074e0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="074e0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="074e0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="074e0-112">Termos. Read. All, termos. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="074e0-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="074e0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="074e0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="074e0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="074e0-114">Not supported.</span></span>    |
|<span data-ttu-id="074e0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="074e0-115">Application</span></span> | <span data-ttu-id="074e0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="074e0-116">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="074e0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="074e0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore/groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="074e0-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="074e0-118">Optional query parameters</span></span>
<span data-ttu-id="074e0-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="074e0-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="074e0-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="074e0-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="074e0-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="074e0-121">Request headers</span></span>
|<span data-ttu-id="074e0-122">Nome</span><span class="sxs-lookup"><span data-stu-id="074e0-122">Name</span></span>|<span data-ttu-id="074e0-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="074e0-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="074e0-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="074e0-124">Authorization</span></span>|<span data-ttu-id="074e0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="074e0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="074e0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="074e0-127">Request body</span></span>
<span data-ttu-id="074e0-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="074e0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="074e0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="074e0-129">Response</span></span>

<span data-ttu-id="074e0-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [Group](../resources/termstore-group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="074e0-130">If successful, this method returns a `200 OK` response code and a collection of [group](../resources/termstore-group.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="074e0-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="074e0-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="074e0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="074e0-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}
-->

``` http
GET https://graph.microsoft.com/beta/termStore/groups
```


### <a name="response"></a><span data-ttu-id="074e0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="074e0-133">Response</span></span>
<span data-ttu-id="074e0-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="074e0-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.termStore.group)"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "85825593-5593-8582-9355-828593558285",
      "createdDateTime": "2019-06-21T20:01:37Z",
      "description": "My term group",
      "scope" : "global",
      "displayName": "myGroup"  
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Get termGroup entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/List termGroups",
  "suppressions": [
  ]
}
-->

