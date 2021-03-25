---
title: Atualizar adminConsentRequestPolicy
description: Atualize as propriedades de um objeto adminConsentRequestPolicy.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 3fcd6bb895a4f1cb36f099269c8414669dc98620
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201446"
---
# <a name="update-adminconsentrequestpolicy"></a><span data-ttu-id="7f45f-103">Atualizar adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="7f45f-103">Update adminConsentRequestPolicy</span></span>
<span data-ttu-id="7f45f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f45f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f45f-105">Atualize as propriedades de [um objeto adminConsentRequestPolicy.](../resources/adminconsentrequestpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7f45f-105">Update the properties of an [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f45f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7f45f-106">Permissions</span></span>
<span data-ttu-id="7f45f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f45f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f45f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f45f-109">Permission type</span></span>|<span data-ttu-id="7f45f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7f45f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f45f-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f45f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7f45f-112">Policy.ReadWrite.ConsentRequest</span><span class="sxs-lookup"><span data-stu-id="7f45f-112">Policy.ReadWrite.ConsentRequest</span></span>|
|<span data-ttu-id="7f45f-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f45f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f45f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f45f-114">Not supported.</span></span>|
|<span data-ttu-id="7f45f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f45f-115">Application</span></span>|<span data-ttu-id="7f45f-116">Policy.ReadWrite.ConsentRequest</span><span class="sxs-lookup"><span data-stu-id="7f45f-116">Policy.ReadWrite.ConsentRequest</span></span>|

<span data-ttu-id="7f45f-117">Ao chamar em nome de um usuário, o usuário precisa pertencer à função de diretório [Administrador Global.](/azure/active-directory/roles/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="7f45f-117">When calling on behalf of a user, the user needs to belong to the [Global Administrator](/azure/active-directory/roles/permissions-reference) directory role.</span></span>

## <a name="http-request"></a><span data-ttu-id="7f45f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f45f-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PUT /policies/adminConsentRequestPolicy 
```

## <a name="request-headers"></a><span data-ttu-id="7f45f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f45f-119">Request headers</span></span>
|<span data-ttu-id="7f45f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="7f45f-120">Name</span></span>|<span data-ttu-id="7f45f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f45f-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7f45f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f45f-122">Authorization</span></span>|<span data-ttu-id="7f45f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f45f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7f45f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7f45f-125">Content-Type</span></span>|<span data-ttu-id="7f45f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f45f-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f45f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f45f-128">Request body</span></span>
<span data-ttu-id="7f45f-129">No corpo da solicitação, fornece uma representação JSON do [objeto adminConsentRequestPolicy.](../resources/adminconsentrequestpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7f45f-129">In the request body, supply a JSON representation of the [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object.</span></span>

<span data-ttu-id="7f45f-130">A tabela a seguir mostra as propriedades que são necessárias ao atualizar [o adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7f45f-130">The following table shows the properties that are required when you update the [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md).</span></span>

|<span data-ttu-id="7f45f-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f45f-131">Property</span></span>|<span data-ttu-id="7f45f-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f45f-132">Type</span></span>|<span data-ttu-id="7f45f-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f45f-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f45f-134">isEnabled</span><span class="sxs-lookup"><span data-stu-id="7f45f-134">isEnabled</span></span>|<span data-ttu-id="7f45f-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="7f45f-135">Boolean</span></span>|<span data-ttu-id="7f45f-136">Especifica se o recurso de solicitação de consentimento do administrador está habilitado ou desabilitado.</span><span class="sxs-lookup"><span data-stu-id="7f45f-136">Specifies whether the admin consent request feature is enabled or disabled.</span></span>|
|<span data-ttu-id="7f45f-137">notifyReviewers</span><span class="sxs-lookup"><span data-stu-id="7f45f-137">notifyReviewers</span></span>|<span data-ttu-id="7f45f-138">Booleano</span><span class="sxs-lookup"><span data-stu-id="7f45f-138">Boolean</span></span>|<span data-ttu-id="7f45f-139">Especifica se os revisadores receberão notificações.</span><span class="sxs-lookup"><span data-stu-id="7f45f-139">Specifies whether reviewers will receive notifications.</span></span>|
|<span data-ttu-id="7f45f-140">remindersEnabled</span><span class="sxs-lookup"><span data-stu-id="7f45f-140">remindersEnabled</span></span>|<span data-ttu-id="7f45f-141">Booleano</span><span class="sxs-lookup"><span data-stu-id="7f45f-141">Boolean</span></span>|<span data-ttu-id="7f45f-142">Especifica se os revisadores receberão emails de lembrete.</span><span class="sxs-lookup"><span data-stu-id="7f45f-142">Specifies whether reviewers will receive reminder emails.</span></span>|
|<span data-ttu-id="7f45f-143">requestDurationInDays</span><span class="sxs-lookup"><span data-stu-id="7f45f-143">requestDurationInDays</span></span>|<span data-ttu-id="7f45f-144">Int32</span><span class="sxs-lookup"><span data-stu-id="7f45f-144">Int32</span></span>|<span data-ttu-id="7f45f-145">Especifica a duração em que a solicitação está ativa antes de expirar automaticamente se nenhuma decisão for aplicada.</span><span class="sxs-lookup"><span data-stu-id="7f45f-145">Specifies the duration the request is active before it automatically expires if no decision is applied.</span></span>|
|<span data-ttu-id="7f45f-146">revisadores</span><span class="sxs-lookup"><span data-stu-id="7f45f-146">reviewers</span></span>|<span data-ttu-id="7f45f-147">[Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)</span><span class="sxs-lookup"><span data-stu-id="7f45f-147">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|<span data-ttu-id="7f45f-148">A lista de revisadores para o consentimento do administrador.</span><span class="sxs-lookup"><span data-stu-id="7f45f-148">The list of reviewers for the admin consent.</span></span>|



## <a name="response"></a><span data-ttu-id="7f45f-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f45f-149">Response</span></span>

<span data-ttu-id="7f45f-150">Se tiver êxito, este método retornará um código de resposta `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="7f45f-150">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7f45f-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7f45f-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7f45f-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f45f-152">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7f45f-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f45f-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_adminconsentrequestpolicy"
}
-->
``` http
PUT https://graph.microsoft.com/beta/policies/adminConsentRequestPolicy 
Content-Type: application/json

{
  "isEnabled": true,
  "notifyReviewers": true,
  "remindersEnabled": true,
  "requestDurationInDays": 5,
  "reviewers": [
    {
      "query": "/users/b6879be8-fb87-4482-a72e-18445d2b5c54",
      "queryType": "MicrosoftGraph"
    },
    {
      "query": "/users/b3427cc5-bf69-4dcd-95f7-ed1eb432f5e9",
      "queryType": "MicrosoftGraph"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="7f45f-154">C#</span><span class="sxs-lookup"><span data-stu-id="7f45f-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-adminconsentrequestpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f45f-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f45f-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-adminconsentrequestpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f45f-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f45f-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-adminconsentrequestpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7f45f-157">Java</span><span class="sxs-lookup"><span data-stu-id="7f45f-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-adminconsentrequestpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="7f45f-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f45f-158">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: text/plain
```
