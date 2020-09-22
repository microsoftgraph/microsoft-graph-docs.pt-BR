---
title: Atualizar continuousAccessEvaluationPolicy
description: Atualiza as propriedades de um objeto continuousAccessEvaluationPolicy.
author: jerrysai
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cb6a3cbffdb8058051442b85aeb6617639ce5dd5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023402"
---
# <a name="update-continuousaccessevaluationpolicy"></a><span data-ttu-id="96903-103">Atualizar continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="96903-103">Update continuousAccessEvaluationPolicy</span></span>
<span data-ttu-id="96903-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96903-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96903-105">Atualiza as propriedades de um objeto [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="96903-105">Update the properties of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="96903-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="96903-106">Permissions</span></span>
<span data-ttu-id="96903-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96903-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96903-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96903-109">Permission type</span></span>                        | <span data-ttu-id="96903-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="96903-110">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="96903-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96903-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="96903-112">Policy. Read. All, Policy. ReadWrite. ConditionalAccess e Application. Read. All</span><span class="sxs-lookup"><span data-stu-id="96903-112">Policy.Read.All, Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |
|<span data-ttu-id="96903-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96903-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96903-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96903-114">Not supported.</span></span> |
|<span data-ttu-id="96903-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96903-115">Application</span></span>                            | <span data-ttu-id="96903-116">Policy. Read. All, Policy. ReadWrite. ConditionalAccess e Application. Read. All</span><span class="sxs-lookup"><span data-stu-id="96903-116">Policy.Read.All, Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |

> [!NOTE]
> <span data-ttu-id="96903-117">Essa API tem um [problema conhecido](/graph/known-issues#permissions) relacionado às permissões.</span><span class="sxs-lookup"><span data-stu-id="96903-117">This API has a [known issue](/graph/known-issues#permissions) related to permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="96903-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96903-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identity/continuousAccessEvaluationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="96903-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96903-119">Request headers</span></span>
|<span data-ttu-id="96903-120">Nome</span><span class="sxs-lookup"><span data-stu-id="96903-120">Name</span></span>|<span data-ttu-id="96903-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="96903-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="96903-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="96903-122">Authorization</span></span>|<span data-ttu-id="96903-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96903-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="96903-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="96903-125">Content-Type</span></span>|<span data-ttu-id="96903-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96903-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="96903-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96903-128">Request body</span></span>
<span data-ttu-id="96903-129">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="96903-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="96903-130">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="96903-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="96903-131">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="96903-131">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="96903-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96903-132">Property</span></span>|<span data-ttu-id="96903-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="96903-133">Type</span></span>|<span data-ttu-id="96903-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="96903-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96903-135">grupos</span><span class="sxs-lookup"><span data-stu-id="96903-135">groups</span></span>|<span data-ttu-id="96903-136">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="96903-136">String collection</span></span>|<span data-ttu-id="96903-137">A coleção de identificadores de grupo no escopo para avaliação.</span><span class="sxs-lookup"><span data-stu-id="96903-137">The collection of group identifiers in scope for evaluation.</span></span> <span data-ttu-id="96903-138">Todos os grupos estão no escopo quando a coleção está vazia.</span><span class="sxs-lookup"><span data-stu-id="96903-138">All groups are in scope when the collection is empty.</span></span>|
|<span data-ttu-id="96903-139">isEnabled</span><span class="sxs-lookup"><span data-stu-id="96903-139">isEnabled</span></span>|<span data-ttu-id="96903-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="96903-140">Boolean</span></span>| <span data-ttu-id="96903-141">`true` para indicar se a avaliação de acesso contínuo deve ser executada; caso contrário `false` .</span><span class="sxs-lookup"><span data-stu-id="96903-141">`true` to indicate whether continuous access evaluation should be performed; otherwise `false`.</span></span> |
|<span data-ttu-id="96903-142">usuários</span><span class="sxs-lookup"><span data-stu-id="96903-142">users</span></span>|<span data-ttu-id="96903-143">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="96903-143">String collection</span></span>|<span data-ttu-id="96903-144">A coleção de identificadores de usuário no escopo para avaliação.</span><span class="sxs-lookup"><span data-stu-id="96903-144">The collection of user identifiers in scope for evaluation.</span></span> <span data-ttu-id="96903-145">Todos os usuários estão no escopo quando a coleção está vazia.</span><span class="sxs-lookup"><span data-stu-id="96903-145">All users are in scope when the collection is empty.</span></span>|


## <a name="response"></a><span data-ttu-id="96903-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="96903-146">Response</span></span>

<span data-ttu-id="96903-p107">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96903-p107">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="96903-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="96903-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="96903-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96903-150">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_continuousaccessevaluationpolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identity/continuousAccessEvaluationPolicy
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.continuousAccessEvaluationPolicy",
  "users": [ "88139f01-1f8d-4c06-ad74-a2544cee9aee" ],
  "groups": [ "9972fb3f-7a40-49f5-85f6-129d9dfbd47a", "ea178055-4713-4d9a-a06c-ff17466b7e77"]
}
```


### <a name="response"></a><span data-ttu-id="96903-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="96903-151">Response</span></span>

<span data-ttu-id="96903-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="96903-152">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```