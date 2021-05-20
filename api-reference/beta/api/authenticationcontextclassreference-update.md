---
title: Atualizar authenticationContextClassReference
description: Atualize as propriedades de um objeto authenticationContextClassReference.
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: dcc0a20ac8b10fc1b7fad3fa3472832036f70024
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547297"
---
# <a name="update-authenticationcontextclassreference"></a><span data-ttu-id="b8dc6-103">Atualizar authenticationContextClassReference</span><span class="sxs-lookup"><span data-stu-id="b8dc6-103">Update authenticationContextClassReference</span></span>

<span data-ttu-id="b8dc6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8dc6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8dc6-105">Atualize as propriedades de [um objeto authenticationContextClassReference.](../resources/authenticationcontextclassreference.md)</span><span class="sxs-lookup"><span data-stu-id="b8dc6-105">Update the properties of an [authenticationContextClassReference](../resources/authenticationcontextclassreference.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8dc6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8dc6-106">Permissions</span></span>

<span data-ttu-id="b8dc6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8dc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8dc6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8dc6-109">Permission type</span></span>                        | <span data-ttu-id="b8dc6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8dc6-110">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="b8dc6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8dc6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b8dc6-112">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="b8dc6-112">Policy.ReadWrite.ConditionalAccess</span></span> |
|<span data-ttu-id="b8dc6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8dc6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8dc6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8dc6-114">Not supported.</span></span> |
|<span data-ttu-id="b8dc6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8dc6-115">Application</span></span>                            | <span data-ttu-id="b8dc6-116">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="b8dc6-116">Policy.ReadWrite.ConditionalAccess</span></span> |

> [!NOTE]
> <span data-ttu-id="b8dc6-117">Essa API tem um [problema conhecido relacionado](/graph/known-issues#permissions) a permissões.</span><span class="sxs-lookup"><span data-stu-id="b8dc6-117">This API has a [known issue](/graph/known-issues#permissions) related to permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="b8dc6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8dc6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/conditionalAccess/authenticationContextClassReferences/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b8dc6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8dc6-119">Request headers</span></span>

| <span data-ttu-id="b8dc6-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b8dc6-120">Name</span></span>          | <span data-ttu-id="b8dc6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8dc6-121">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="b8dc6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8dc6-122">Authorization</span></span> | <span data-ttu-id="b8dc6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8dc6-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="b8dc6-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b8dc6-125">Content-Type</span></span>  | <span data-ttu-id="b8dc6-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8dc6-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8dc6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8dc6-128">Request body</span></span>

<span data-ttu-id="b8dc6-129">No corpo da solicitação, fornece os valores para propriedades relevantes que devem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="b8dc6-129">In the request body, supply the values for relevant properties that should be updated.</span></span> <span data-ttu-id="b8dc6-130">As propriedades existentes que não estão incluídas no corpo da solicitação mantêm os valores anteriores ou recalcula-os com base nas alterações feitas em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="b8dc6-130">Existing properties that are not included in the request body maintain their previous values or are recalculated based on changes to other property values.</span></span> <span data-ttu-id="b8dc6-131">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b8dc6-131">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="b8dc6-132">Para ver a lista de propriedades, consulte [authenticationContextClassReference](../resources/authenticationContextClassReference.md).</span><span class="sxs-lookup"><span data-stu-id="b8dc6-132">For the list of properties, see [authenticationContextClassReference](../resources/authenticationContextClassReference.md).</span></span>

## <a name="response"></a><span data-ttu-id="b8dc6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8dc6-133">Response</span></span>

<span data-ttu-id="b8dc6-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8dc6-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b8dc6-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b8dc6-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b8dc6-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8dc6-137">Request</span></span>

<span data-ttu-id="b8dc6-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8dc6-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_authenticationcontextclassreference"
}-->

```http
PATCH https://graph.microsoft.com/beta/identity/conditionalAccess/authenticationContextClassReferences/c1
Content-type: application/json

{
   "value": 
    [
      {
         "displayName": "Contoso trusted locations",
        "description": "Access is only allowed from trusted locations",
        "isAvailable": true
      }
    ]
}
```



### <a name="response"></a><span data-ttu-id="b8dc6-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8dc6-139">Response</span></span>

<span data-ttu-id="b8dc6-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b8dc6-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update authenticationContextClassReference",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
