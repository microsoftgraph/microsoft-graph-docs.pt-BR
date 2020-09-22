---
title: Criar relação
description: Criar um novo objeto relation.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 8008abbfa10bbc0c7267384c66afc7c7c1c1c328
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055716"
---
# <a name="create-relation"></a><span data-ttu-id="1d0cb-103">Criar relação</span><span class="sxs-lookup"><span data-stu-id="1d0cb-103">Create relation</span></span>
<span data-ttu-id="1d0cb-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="1d0cb-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d0cb-105">Criar um novo objeto [relation](../resources/termstore-relation.md) .</span><span class="sxs-lookup"><span data-stu-id="1d0cb-105">Create a new [relation](../resources/termstore-relation.md) object.</span></span> <span data-ttu-id="1d0cb-106">Eles são usados para criar relações fixas e resued entre os termos ou entre um termo e um conjunto.</span><span class="sxs-lookup"><span data-stu-id="1d0cb-106">These are used to create pinned and resued relations between terms or between a term and set.</span></span> <span data-ttu-id="1d0cb-107">Ao criar um termo fixado/reutilizado entre o termo e Set, fromTerm no corpo da postagem deve ser nulo.</span><span class="sxs-lookup"><span data-stu-id="1d0cb-107">When creating a pinned/reused term between term and set then fromTerm in the post body must be null.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d0cb-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="1d0cb-108">Permissions</span></span>
<span data-ttu-id="1d0cb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d0cb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d0cb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d0cb-111">Permission type</span></span>|<span data-ttu-id="1d0cb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1d0cb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d0cb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d0cb-113">Delegated (work or school account)</span></span> |<span data-ttu-id="1d0cb-114">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d0cb-114">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="1d0cb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d0cb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d0cb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d0cb-116">Not supported.</span></span>    |
|<span data-ttu-id="1d0cb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d0cb-117">Application</span></span> | <span data-ttu-id="1d0cb-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d0cb-118">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="1d0cb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d0cb-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /termStore/sets/{setId}/terms/{termId}/relations
```

## <a name="request-headers"></a><span data-ttu-id="1d0cb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d0cb-120">Request headers</span></span>
|<span data-ttu-id="1d0cb-121">Nome</span><span class="sxs-lookup"><span data-stu-id="1d0cb-121">Name</span></span>|<span data-ttu-id="1d0cb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d0cb-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1d0cb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d0cb-123">Authorization</span></span>|<span data-ttu-id="1d0cb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d0cb-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1d0cb-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1d0cb-126">Content-Type</span></span>|<span data-ttu-id="1d0cb-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d0cb-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d0cb-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d0cb-129">Request body</span></span>
<span data-ttu-id="1d0cb-130">No corpo da solicitação, forneça uma representação JSON do objeto [relation](../resources/termstore-relation.md) .</span><span class="sxs-lookup"><span data-stu-id="1d0cb-130">In the request body, supply a JSON representation of the [relation](../resources/termstore-relation.md) object.</span></span>

<span data-ttu-id="1d0cb-131">A tabela a seguir mostra as propriedades que são necessárias ao criar a [relação](../resources/termstore-relation.md).</span><span class="sxs-lookup"><span data-stu-id="1d0cb-131">The following table shows the properties that are required when you create the [relation](../resources/termstore-relation.md).</span></span>

|<span data-ttu-id="1d0cb-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d0cb-132">Property</span></span>|<span data-ttu-id="1d0cb-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d0cb-133">Type</span></span>|<span data-ttu-id="1d0cb-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d0cb-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d0cb-135">relação</span><span class="sxs-lookup"><span data-stu-id="1d0cb-135">relationship</span></span>|<span data-ttu-id="1d0cb-136">relationtype</span><span class="sxs-lookup"><span data-stu-id="1d0cb-136">relationType</span></span>|<span data-ttu-id="1d0cb-137">Tipo de relação a ser criada.</span><span class="sxs-lookup"><span data-stu-id="1d0cb-137">Type of relation to be created.</span></span> <span data-ttu-id="1d0cb-138">Os valores possíveis são: `pin` e `reuse`.</span><span class="sxs-lookup"><span data-stu-id="1d0cb-138">Possible values are: `pin`, `reuse`.</span></span>|
|<span data-ttu-id="1d0cb-139">set</span><span class="sxs-lookup"><span data-stu-id="1d0cb-139">set</span></span>| [<span data-ttu-id="1d0cb-140">Microsoft. Graph. termos. Set</span><span class="sxs-lookup"><span data-stu-id="1d0cb-140">microsoft.graph.termstore.set</span></span>](../resources/termstore-set.md)| <span data-ttu-id="1d0cb-141">O conjunto em que a relação precisa ser criada.</span><span class="sxs-lookup"><span data-stu-id="1d0cb-141">The set where the relationship needs to be created.</span></span>
|<span data-ttu-id="1d0cb-142">fromTerm</span><span class="sxs-lookup"><span data-stu-id="1d0cb-142">fromTerm</span></span>| [<span data-ttu-id="1d0cb-143">Microsoft. Graph. termos. Term</span><span class="sxs-lookup"><span data-stu-id="1d0cb-143">microsoft.graph.termstore.term</span></span>](../resources/termstore-term.md) | <span data-ttu-id="1d0cb-144">O termo com o qual a relação precisa ser criada.</span><span class="sxs-lookup"><span data-stu-id="1d0cb-144">The term with which the relationship needs to be created.</span></span>



## <a name="response"></a><span data-ttu-id="1d0cb-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d0cb-145">Response</span></span>

<span data-ttu-id="1d0cb-146">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [relation](../resources/termstore-relation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d0cb-146">If successful, this method returns a `201 Created` response code and a [relation](../resources/termstore-relation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1d0cb-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1d0cb-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1d0cb-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d0cb-148">Request</span></span>

``` http
POST https://graph.microsoft.com/beta/termStore/sets/{setId}/terms/{termId}/relations
Content-Type: application/json
Content-length: 89

{
  "@odata.type": "#microsoft.graph.termStore.relation",
  "relationship": "pin",
  "fromTerm" : {
    "id" : "b49f64b3-4722-4336-9a5c-56c326b344d4"
  },
  "set" : {
    "id": "95e553ae-a91a-4670-a139-67a6cea285b3"
  }
}
```


### <a name="response"></a><span data-ttu-id="1d0cb-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d0cb-149">Response</span></span>
<span data-ttu-id="1d0cb-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1d0cb-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termstore.relation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.termStore.relation",
  "id": "052c749c-749c-052c-9c74-2c059c742c05",
  "relationship": "pin",
  "fromTerm" : {
      "id" : "b49f64b3-4722-4336-9a5c-56c326b344d4"
  },
  "toTerm" : {
      "id" : "226e8ee3-f4b6-49d7-92d5-ec9d5475eec5"
  },
  "set" : {
      "id" : "95e553ae-a91a-4670-a139-67a6cea285b3"
  }
}
```

[microsoft.graph.termStore.set]: ../resources/termstore-set.md
[microsoft.graph.termStore.term]: ../resources/termstore-term.md
[microsoft.graph.termStore.relation]: ../resources/termstore-relation.md


<!--
{
  "type": "#page.annotation",
  "description": "Create a pinned term entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Pinned term",
  "suppressions": [
  ]
}
-->


