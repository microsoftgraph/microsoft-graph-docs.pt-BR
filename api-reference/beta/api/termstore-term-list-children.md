---
title: Listar filhos
description: Obtenha os termos da propriedade de navegação Children.
author: mohitpcad
ms.prod: Sharepoint
localization_priority: Normal
doc_type: apiPageType
ms.openlocfilehash: b33b2ac40a489909d23183319b6c8f0fe2506c60
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539155"
---
# <a name="list-children"></a><span data-ttu-id="6f2c2-103">Listar filhos</span><span class="sxs-lookup"><span data-stu-id="6f2c2-103">List children</span></span>
<span data-ttu-id="6f2c2-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="6f2c2-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f2c2-105">Obter o primeiro nível filho de um recurso [set] ou [Term] usando a propriedade de navegação Children.</span><span class="sxs-lookup"><span data-stu-id="6f2c2-105">Get the first level children of a [set] or [term] resource using the children navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f2c2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6f2c2-106">Permissions</span></span>
<span data-ttu-id="6f2c2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f2c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f2c2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f2c2-109">Permission type</span></span>|<span data-ttu-id="6f2c2-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6f2c2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f2c2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f2c2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6f2c2-112">Termos. Read. All, termos. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6f2c2-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="6f2c2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f2c2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f2c2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f2c2-114">Not supported.</span></span>    |
|<span data-ttu-id="6f2c2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f2c2-115">Application</span></span> | <span data-ttu-id="6f2c2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f2c2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f2c2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f2c2-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /termStore/sets/{setId}/children
GET /termStore/sets/{setId}/terms/{termId}/children
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6f2c2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6f2c2-118">Optional query parameters</span></span>
<span data-ttu-id="6f2c2-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6f2c2-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6f2c2-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6f2c2-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6f2c2-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f2c2-121">Request headers</span></span>
|<span data-ttu-id="6f2c2-122">Nome</span><span class="sxs-lookup"><span data-stu-id="6f2c2-122">Name</span></span>|<span data-ttu-id="6f2c2-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f2c2-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6f2c2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f2c2-124">Authorization</span></span>|<span data-ttu-id="6f2c2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f2c2-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f2c2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f2c2-127">Request body</span></span>
<span data-ttu-id="6f2c2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6f2c2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f2c2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f2c2-129">Response</span></span>

<span data-ttu-id="6f2c2-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [Term](../resources/termstore-term.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f2c2-130">If successful, this method returns a `200 OK` response code and a collection of [term](../resources/termstore-term.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6f2c2-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6f2c2-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6f2c2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f2c2-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_term"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore/sets/{setId}/children
```


### <a name="response"></a><span data-ttu-id="6f2c2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f2c2-133">Response</span></span>
<span data-ttu-id="6f2c2-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6f2c2-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.termStore.term)"
}-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {      
      "id": "81be9856-9856-81be-5698-be815698be81",
      "labels" : [
        {
          "name" : "Car",
          "languageTag" : "en-US",
          "isDefault" : true
        }
      ],
      "lastModifiedDateTime": "2019-06-21T20:01:37Z"
   }  
 ]
}
```

[terminal]: ../resources/termstore-term.md
[term]: ../resources/termstore-term.md
[set]: ../resources/termstore-set.md

<!--
{
  "type": "#page.annotation",
  "description": "Get children of a term or termSet in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Get termchildren",
  "suppressions": []
}
-->
