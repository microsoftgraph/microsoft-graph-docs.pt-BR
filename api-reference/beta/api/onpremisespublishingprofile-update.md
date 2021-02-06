---
title: Atualizar onPremisesPublishingProfile
description: Atualizar as propriedades de um objeto onPremisesPublishingProfile.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: e1200e66da53b564e21396bbf347959a3223fd3a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132787"
---
# <a name="update-onpremisespublishingprofile"></a><span data-ttu-id="26d81-103">Atualizar onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="26d81-103">Update onPremisesPublishingProfile</span></span>

<span data-ttu-id="26d81-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26d81-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26d81-105">Atualizar as propriedades de um [objeto onPremisesPublishingProfile.](../resources/onpremisespublishingprofile.md)</span><span class="sxs-lookup"><span data-stu-id="26d81-105">Update the properties of an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="26d81-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="26d81-106">Permissions</span></span>

<span data-ttu-id="26d81-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26d81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="26d81-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26d81-109">Permission type</span></span>                        | <span data-ttu-id="26d81-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="26d81-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="26d81-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26d81-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="26d81-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26d81-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="26d81-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26d81-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26d81-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26d81-114">Not supported.</span></span> |
| <span data-ttu-id="26d81-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26d81-115">Application</span></span>                            | <span data-ttu-id="26d81-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26d81-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="26d81-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26d81-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/hybridAgentUpdaterConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="26d81-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26d81-118">Request headers</span></span>

| <span data-ttu-id="26d81-119">Nome</span><span class="sxs-lookup"><span data-stu-id="26d81-119">Name</span></span>       | <span data-ttu-id="26d81-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="26d81-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="26d81-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="26d81-121">Authorization</span></span> | <span data-ttu-id="26d81-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="26d81-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="26d81-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26d81-123">Request body</span></span>

<span data-ttu-id="26d81-124">No corpo da solicitação, fornece os valores dos campos relevantes a atualizar.</span><span class="sxs-lookup"><span data-stu-id="26d81-124">In the request body, supply the values for relevant fields to update.</span></span> <span data-ttu-id="26d81-125">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="26d81-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="26d81-126">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="26d81-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="26d81-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26d81-127">Property</span></span>     | <span data-ttu-id="26d81-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="26d81-128">Type</span></span>        | <span data-ttu-id="26d81-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="26d81-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="26d81-130">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="26d81-130">hybridAgentUpdaterConfiguration</span></span>|<span data-ttu-id="26d81-131">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="26d81-131">hybridAgentUpdaterConfiguration</span></span>|<span data-ttu-id="26d81-132">Representa [hybridAgentUpdaterConfiguration](../resources/hybridagentupdaterconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="26d81-132">Represents [hybridAgentUpdaterConfiguration](../resources/hybridagentupdaterconfiguration.md).</span></span>|

## <a name="response"></a><span data-ttu-id="26d81-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="26d81-133">Response</span></span>

<span data-ttu-id="26d81-134">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="26d81-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="26d81-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="26d81-135">Examples</span></span>

### <a name="example-1-update-updatewindow-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="26d81-136">Exemplo 1: Atualizar UpdateWindow no hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="26d81-136">Example 1: Update updateWindow in the hybridAgentUpdaterConfiguration</span></span>

<span data-ttu-id="26d81-137">O exemplo a seguir atualiza **a updateWindow** no **hybridAgentUpdaterConfiguration**.</span><span class="sxs-lookup"><span data-stu-id="26d81-137">The following example updates the **updateWindow** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="26d81-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26d81-138">Request</span></span>

<span data-ttu-id="26d81-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="26d81-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="26d81-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="26d81-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_onpremisespublishingprofile"
}-->

```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration
Content-Type: application/json

{
   "updateWindow" :
{
      "updateWindowStartTime" : "0:00:00",
      "updateWindowEndTime" : "23:59:00"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="26d81-141">C#</span><span class="sxs-lookup"><span data-stu-id="26d81-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-onpremisespublishingprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26d81-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26d81-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-onpremisespublishingprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26d81-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26d81-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-onpremisespublishingprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="26d81-144">Java</span><span class="sxs-lookup"><span data-stu-id="26d81-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-onpremisespublishingprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="26d81-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="26d81-145">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-deferupdate-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="26d81-146">Exemplo 2: Atualizar deferUpdate no hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="26d81-146">Example 2: Update deferUpdate in the hybridAgentUpdaterConfiguration</span></span> 

<span data-ttu-id="26d81-147">O exemplo a seguir **atualiza deferUpdate** no **hybridAgentUpdaterConfiguration**.</span><span class="sxs-lookup"><span data-stu-id="26d81-147">The following example updates **deferUpdate** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="26d81-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26d81-148">Request</span></span>

<span data-ttu-id="26d81-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="26d81-149">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_onpremisespublishingprofile"
}-->

```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration
Content-Type: application/json

{
    "deferUpdate" : "2018-08-20T12:00"
}
```

#### <a name="response"></a><span data-ttu-id="26d81-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="26d81-150">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-allowupdateconfigurationoverride-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="26d81-151">Exemplo 3: Atualizar allowUpdateConfigurationOverride no hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="26d81-151">Example 3: Update allowUpdateConfigurationOverride in the hybridAgentUpdaterConfiguration</span></span>

<span data-ttu-id="26d81-152">O exemplo a seguir atualiza **allowUpdateConfigurationOverride** no **hybridAgentUpdaterConfiguration**.</span><span class="sxs-lookup"><span data-stu-id="26d81-152">The following example updates **allowUpdateConfigurationOverride** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="26d81-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26d81-153">Request</span></span>

<span data-ttu-id="26d81-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="26d81-154">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_onpremisespublishingprofile"
}-->

```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration
Content-Type: application/json

{
    "allowUpdateConfigurationOverride" : false
}
```

#### <a name="response"></a><span data-ttu-id="26d81-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="26d81-155">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update onpremisespublishingprofile",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



