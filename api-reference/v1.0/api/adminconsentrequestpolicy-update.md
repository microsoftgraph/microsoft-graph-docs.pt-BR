---
title: Atualizar adminConsentRequestPolicy
description: Atualize as propriedades de um objeto adminConsentRequestPolicy.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 1eee4e0bf4ee57715953367ea2f0b43e9cc2e34f
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469521"
---
# <a name="update-adminconsentrequestpolicy"></a><span data-ttu-id="a7fdf-103">Atualizar adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="a7fdf-103">Update adminConsentRequestPolicy</span></span>

<span data-ttu-id="a7fdf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7fdf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a7fdf-105">Atualize as propriedades de [um objeto adminConsentRequestPolicy.](../resources/adminconsentrequestpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a7fdf-105">Update the properties of an [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7fdf-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a7fdf-106">Permissions</span></span>

<span data-ttu-id="a7fdf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7fdf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7fdf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7fdf-109">Permission type</span></span>|<span data-ttu-id="a7fdf-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a7fdf-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7fdf-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7fdf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a7fdf-112">Policy.ReadWrite.ConsentRequest, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7fdf-112">Policy.ReadWrite.ConsentRequest, Directory.ReadWrite.All</span></span>|
|<span data-ttu-id="a7fdf-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7fdf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7fdf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7fdf-114">Not supported.</span></span>|
|<span data-ttu-id="a7fdf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a7fdf-115">Application</span></span>|<span data-ttu-id="a7fdf-116">Policy.ReadWrite.ConsentRequest, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7fdf-116">Policy.ReadWrite.ConsentRequest, Directory.ReadWrite.All</span></span>|

<span data-ttu-id="a7fdf-117">Ao chamar em nome de um usuário, o usuário precisa pertencer à função de diretório [Administrador Global.](/azure/active-directory/roles/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="a7fdf-117">When calling on behalf of a user, the user needs to belong to the [Global Administrator](/azure/active-directory/roles/permissions-reference) directory role.</span></span>

## <a name="http-request"></a><span data-ttu-id="a7fdf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7fdf-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PUT /policies/adminConsentRequestPolicy
```

## <a name="request-headers"></a><span data-ttu-id="a7fdf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7fdf-119">Request headers</span></span>

|<span data-ttu-id="a7fdf-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a7fdf-120">Name</span></span>|<span data-ttu-id="a7fdf-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7fdf-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a7fdf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7fdf-122">Authorization</span></span>|<span data-ttu-id="a7fdf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7fdf-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a7fdf-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a7fdf-125">Content-Type</span></span>|<span data-ttu-id="a7fdf-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7fdf-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7fdf-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a7fdf-128">Request body</span></span>

<span data-ttu-id="a7fdf-129">No corpo da solicitação, fornece uma representação JSON do [objeto adminConsentRequestPolicy.](../resources/adminconsentrequestpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a7fdf-129">In the request body, supply a JSON representation of the [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object.</span></span>

<span data-ttu-id="a7fdf-130">A tabela a seguir mostra as propriedades que são necessárias ao atualizar [o adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a7fdf-130">The following table shows the properties that are required when you update the [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md).</span></span>

|<span data-ttu-id="a7fdf-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a7fdf-131">Property</span></span>|<span data-ttu-id="a7fdf-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7fdf-132">Type</span></span>|<span data-ttu-id="a7fdf-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7fdf-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7fdf-134">isEnabled</span><span class="sxs-lookup"><span data-stu-id="a7fdf-134">isEnabled</span></span>|<span data-ttu-id="a7fdf-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="a7fdf-135">Boolean</span></span>|<span data-ttu-id="a7fdf-136">Especifica se o recurso de solicitação de consentimento do administrador está habilitado ou desabilitado.</span><span class="sxs-lookup"><span data-stu-id="a7fdf-136">Specifies whether the admin consent request feature is enabled or disabled.</span></span>|
|<span data-ttu-id="a7fdf-137">notifyReviewers</span><span class="sxs-lookup"><span data-stu-id="a7fdf-137">notifyReviewers</span></span>|<span data-ttu-id="a7fdf-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="a7fdf-138">Boolean</span></span>|<span data-ttu-id="a7fdf-139">Especifica se os revisadores receberão notificações.</span><span class="sxs-lookup"><span data-stu-id="a7fdf-139">Specifies whether reviewers will receive notifications.</span></span>|
|<span data-ttu-id="a7fdf-140">remindersEnabled</span><span class="sxs-lookup"><span data-stu-id="a7fdf-140">remindersEnabled</span></span>|<span data-ttu-id="a7fdf-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="a7fdf-141">Boolean</span></span>|<span data-ttu-id="a7fdf-142">Especifica se os revisadores receberão emails de lembrete.</span><span class="sxs-lookup"><span data-stu-id="a7fdf-142">Specifies whether reviewers will receive reminder emails.</span></span>|
|<span data-ttu-id="a7fdf-143">requestDurationInDays</span><span class="sxs-lookup"><span data-stu-id="a7fdf-143">requestDurationInDays</span></span>|<span data-ttu-id="a7fdf-144">Int32</span><span class="sxs-lookup"><span data-stu-id="a7fdf-144">Int32</span></span>|<span data-ttu-id="a7fdf-145">Especifica a duração em que a solicitação está ativa antes de expirar automaticamente se nenhuma decisão for aplicada.</span><span class="sxs-lookup"><span data-stu-id="a7fdf-145">Specifies the duration the request is active before it automatically expires if no decision is applied.</span></span>|
|<span data-ttu-id="a7fdf-146">revisadores</span><span class="sxs-lookup"><span data-stu-id="a7fdf-146">reviewers</span></span>|<span data-ttu-id="a7fdf-147">[Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)</span><span class="sxs-lookup"><span data-stu-id="a7fdf-147">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|<span data-ttu-id="a7fdf-148">A lista de revisadores para o consentimento do administrador.</span><span class="sxs-lookup"><span data-stu-id="a7fdf-148">The list of reviewers for the admin consent.</span></span>|

## <a name="response"></a><span data-ttu-id="a7fdf-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7fdf-149">Response</span></span>

<span data-ttu-id="a7fdf-150">Se tiver êxito, este método retornará um código de resposta e um `204 No content` [objeto adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a7fdf-150">If successful, this method returns a `204 No content` response code and an updated [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a7fdf-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a7fdf-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a7fdf-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a7fdf-152">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_adminconsentrequestpolicy"
}
-->
``` http
PUT https://graph.microsoft.com/v1.0/policies/adminConsentRequestPolicy 
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

### <a name="response"></a><span data-ttu-id="a7fdf-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7fdf-153">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: text/plain
```
