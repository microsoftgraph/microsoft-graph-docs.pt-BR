---
title: Criar termo
description: Criar um novo objeto Term.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 2d2c18f802d9dfe68aa17b46c4dc196a31e3f93c
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539143"
---
# <a name="create-term"></a><span data-ttu-id="d5091-103">Criar termo</span><span class="sxs-lookup"><span data-stu-id="d5091-103">Create term</span></span>
<span data-ttu-id="d5091-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="d5091-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5091-105">Criar um novo objeto [Term](../resources/termstore-term.md) .</span><span class="sxs-lookup"><span data-stu-id="d5091-105">Create a new [term](../resources/termstore-term.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5091-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d5091-106">Permissions</span></span>
<span data-ttu-id="d5091-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5091-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5091-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5091-109">Permission type</span></span>|<span data-ttu-id="d5091-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d5091-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5091-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5091-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d5091-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5091-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="d5091-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5091-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5091-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5091-114">Not supported.</span></span>    |
|<span data-ttu-id="d5091-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5091-115">Application</span></span> | <span data-ttu-id="d5091-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5091-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="d5091-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5091-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
} -->

``` http
POST /termStore/sets/{setId}/children
POST /termStore/sets/{setId}/terms/{termId}/children
```

## <a name="request-headers"></a><span data-ttu-id="d5091-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5091-118">Request headers</span></span>
|<span data-ttu-id="d5091-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d5091-119">Name</span></span>|<span data-ttu-id="d5091-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5091-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d5091-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5091-121">Authorization</span></span>|<span data-ttu-id="d5091-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5091-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d5091-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d5091-124">Content-Type</span></span>|<span data-ttu-id="d5091-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5091-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5091-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5091-127">Request body</span></span>
<span data-ttu-id="d5091-128">No corpo da solicitação, forneça uma representação JSON do objeto [Term](../resources/termstore-term.md) .</span><span class="sxs-lookup"><span data-stu-id="d5091-128">In the request body, supply a JSON representation of the [term](../resources/termstore-term.md) object.</span></span>

<span data-ttu-id="d5091-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o [termo](../resources/termstore-term.md).</span><span class="sxs-lookup"><span data-stu-id="d5091-129">The following table shows the properties that are required when you create the [term](../resources/termstore-term.md).</span></span>

|<span data-ttu-id="d5091-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5091-130">Property</span></span>|<span data-ttu-id="d5091-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5091-131">Type</span></span>|<span data-ttu-id="d5091-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5091-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5091-133">Legendas</span><span class="sxs-lookup"><span data-stu-id="d5091-133">labels</span></span>|<span data-ttu-id="d5091-134">coleção [Microsoft. Graph. termos. localizedLabel](../resources/termstore-localizedlabel.md)</span><span class="sxs-lookup"><span data-stu-id="d5091-134">[microsoft.graph.termStore.localizedLabel](../resources/termstore-localizedlabel.md) collection</span></span>|<span data-ttu-id="d5091-135">Rótulo do termo a ser criado</span><span class="sxs-lookup"><span data-stu-id="d5091-135">Label for the term to be created</span></span>|



## <a name="response"></a><span data-ttu-id="d5091-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5091-136">Response</span></span>

<span data-ttu-id="d5091-137">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [Term](../resources/termstore-term.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5091-137">If successful, this method returns a `201 Created` response code and a [term](../resources/termstore-term.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d5091-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d5091-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d5091-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5091-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_term_from_"
} -->

``` http
POST https://graph.microsoft.com/beta/termStore/sets/{setId}/terms
Content-Type: application/json
Content-length: 366

{
  "labels": [
    {
      "languageTag" : "en-US",
      "name" : "Car",
      "isDefault" : true
    }
  ]
}
```


### <a name="response"></a><span data-ttu-id="d5091-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5091-140">Response</span></span>
<span data-ttu-id="d5091-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d5091-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.term"
}-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "createdDateTime": "2019-06-21T20:01:37Z",
  "id": "8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f",
  "labels" : [
      {
          "name" : "Car",
          "languageTag" : "en-US",
          "isDefault" : true
      }
  ],
  "lastModifiedDateTime": "2019-06-21T20:01:37Z"
}
```

[microsoft.graph.termStore.set]: ../resources/termstore-set.md
[microsoft.graph.termStore.term]: ../resources/termstore-term.md

<!--
{
  "type": "#page.annotation",
  "description": "Post term entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Post term",
  "suppressions": [
  ]
}
-->
