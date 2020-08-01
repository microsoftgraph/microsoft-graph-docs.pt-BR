---
title: Criar conjunto
description: Criar um novo objeto Set.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 5db84c3fee015a856d43cff03c7f1d8bf356ce16
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539177"
---
# <a name="create-set"></a><span data-ttu-id="a2e7c-103">Criar conjunto</span><span class="sxs-lookup"><span data-stu-id="a2e7c-103">Create set</span></span>
<span data-ttu-id="a2e7c-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="a2e7c-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2e7c-105">Criar um novo objeto [set](../resources/termstore-set.md) .</span><span class="sxs-lookup"><span data-stu-id="a2e7c-105">Create a new [set](../resources/termstore-set.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2e7c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a2e7c-106">Permissions</span></span>
<span data-ttu-id="a2e7c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2e7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2e7c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2e7c-109">Permission type</span></span>|<span data-ttu-id="a2e7c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a2e7c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2e7c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2e7c-111">Delegated (work or school account)</span></span> |<span data-ttu-id="a2e7c-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2e7c-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="a2e7c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a2e7c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2e7c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2e7c-114">Not supported.</span></span>    |
|<span data-ttu-id="a2e7c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a2e7c-115">Application</span></span> | <span data-ttu-id="a2e7c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2e7c-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="a2e7c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2e7c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /termStore/sets
```

## <a name="request-headers"></a><span data-ttu-id="a2e7c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2e7c-118">Request headers</span></span>
|<span data-ttu-id="a2e7c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a2e7c-119">Name</span></span>|<span data-ttu-id="a2e7c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2e7c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a2e7c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2e7c-121">Authorization</span></span>|<span data-ttu-id="a2e7c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2e7c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a2e7c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a2e7c-124">Content-Type</span></span>|<span data-ttu-id="a2e7c-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2e7c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2e7c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2e7c-127">Request body</span></span>
<span data-ttu-id="a2e7c-128">No corpo da solicitação, forneça uma representação JSON do objeto [set](../resources/termstore-set.md) .</span><span class="sxs-lookup"><span data-stu-id="a2e7c-128">In the request body, supply a JSON representation of the [set](../resources/termstore-set.md) object.</span></span>

<span data-ttu-id="a2e7c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o [conjunto](../resources/termstore-set.md).</span><span class="sxs-lookup"><span data-stu-id="a2e7c-129">The following table shows the properties that are required when you create the [set](../resources/termstore-set.md).</span></span>

|<span data-ttu-id="a2e7c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2e7c-130">Property</span></span>|<span data-ttu-id="a2e7c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2e7c-131">Type</span></span>|<span data-ttu-id="a2e7c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2e7c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2e7c-133">localizadores</span><span class="sxs-lookup"><span data-stu-id="a2e7c-133">localizedNames</span></span>|<span data-ttu-id="a2e7c-134">coleção [Microsoft. Graph. termos.](../resources/termstore-localizedname.md) undeleble</span><span class="sxs-lookup"><span data-stu-id="a2e7c-134">[microsoft.graph.termstore.localizedName](../resources/termstore-localizedname.md) collection</span></span>|<span data-ttu-id="a2e7c-135">Nome do conjunto a ser criado</span><span class="sxs-lookup"><span data-stu-id="a2e7c-135">Name of the set to be created</span></span>|
|<span data-ttu-id="a2e7c-136">parentGroup</span><span class="sxs-lookup"><span data-stu-id="a2e7c-136">parentGroup</span></span>|[<span data-ttu-id="a2e7c-137">Microsoft. Graph. termos. Group</span><span class="sxs-lookup"><span data-stu-id="a2e7c-137">microsoft.graph.termstore.group</span></span>](../resources/termstore-group.md)|<span data-ttu-id="a2e7c-138">termos-grupo sob o qual o conjunto precisa ser criado</span><span class="sxs-lookup"><span data-stu-id="a2e7c-138">termstore-group under which the set needs to be created</span></span>|



## <a name="response"></a><span data-ttu-id="a2e7c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2e7c-139">Response</span></span>

<span data-ttu-id="a2e7c-140">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [set](../resources/termstore-set.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2e7c-140">If successful, this method returns a `201 Created` response code and a [set](../resources/termstore-set.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a2e7c-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a2e7c-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a2e7c-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2e7c-142">Request</span></span>
``` http
POST https://graph.microsoft.com/beta/termStore/sets
Content-Type: application/json
Content-length: 288

{
  "@odata.type": "#microsoft.graph.termStore.set",
  "parentGroup":{
      "id": "fc733b51-10f1-40fd-b784-dc6d1e42804b"
   },
   "localizedNames" : [
      {
        "languageTag" : "en-US",
        "name" : "Department"
      }
  ]
}
```


### <a name="response"></a><span data-ttu-id="a2e7c-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2e7c-143">Response</span></span>
<span data-ttu-id="a2e7c-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a2e7c-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termstore.set"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.termStore.set",
  "id": "3607e9f9-e9f9-3607-f9e9-0736f9e90736",
  "localizedNames" : [
      {
        "languageTag" : "en-US",
        "name" : "Department"
      }
  ]
}
```


[microsoft.graph.termStore.set]: ../resources/termstore-set.md
[microsoft.graph.termStore.group]: ../resources/termstore-group.md
[microsoft.graph.termStore.term]: ../resources/termstore-term.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a termSet entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Create termSet",
  "suppressions": [
  ]
}
-->
