---
title: Atualizar onPremisesPublishingProfile
description: Atualize as propriedades de um objeto onPremisesPublishingProfile.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 9ca1c8237f5869c8545482eaf3f561489a48e11c
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547229"
---
# <a name="update-onpremisespublishingprofile"></a><span data-ttu-id="cab33-103">Atualizar onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="cab33-103">Update onPremisesPublishingProfile</span></span>

<span data-ttu-id="cab33-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cab33-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cab33-105">Atualize as propriedades de um [objeto onPremisesPublishingProfile.](../resources/onpremisespublishingprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cab33-105">Update the properties of an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cab33-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cab33-106">Permissions</span></span>

<span data-ttu-id="cab33-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cab33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cab33-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cab33-109">Permission type</span></span>                        | <span data-ttu-id="cab33-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cab33-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="cab33-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cab33-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cab33-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cab33-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="cab33-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cab33-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cab33-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cab33-114">Not supported.</span></span> |
| <span data-ttu-id="cab33-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cab33-115">Application</span></span>                            | <span data-ttu-id="cab33-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cab33-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cab33-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cab33-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/hybridAgentUpdaterConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="cab33-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cab33-118">Request headers</span></span>

| <span data-ttu-id="cab33-119">Nome</span><span class="sxs-lookup"><span data-stu-id="cab33-119">Name</span></span>       | <span data-ttu-id="cab33-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="cab33-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="cab33-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cab33-121">Authorization</span></span> | <span data-ttu-id="cab33-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="cab33-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="cab33-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cab33-123">Request body</span></span>

<span data-ttu-id="cab33-124">No corpo da solicitação, fornece os valores dos campos relevantes a ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="cab33-124">In the request body, supply the values for relevant fields to update.</span></span> <span data-ttu-id="cab33-125">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="cab33-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="cab33-126">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="cab33-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cab33-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cab33-127">Property</span></span>     | <span data-ttu-id="cab33-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="cab33-128">Type</span></span>        | <span data-ttu-id="cab33-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="cab33-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cab33-130">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="cab33-130">hybridAgentUpdaterConfiguration</span></span>|<span data-ttu-id="cab33-131">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="cab33-131">hybridAgentUpdaterConfiguration</span></span>|<span data-ttu-id="cab33-132">Representa [hybridAgentUpdaterConfiguration](../resources/hybridagentupdaterconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cab33-132">Represents [hybridAgentUpdaterConfiguration](../resources/hybridagentupdaterconfiguration.md).</span></span>|

## <a name="response"></a><span data-ttu-id="cab33-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="cab33-133">Response</span></span>

<span data-ttu-id="cab33-134">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cab33-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="cab33-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cab33-135">Examples</span></span>

### <a name="example-1-update-updatewindow-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="cab33-136">Exemplo 1: atualizar updateWindow no hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="cab33-136">Example 1: Update updateWindow in the hybridAgentUpdaterConfiguration</span></span>

<span data-ttu-id="cab33-137">O exemplo a seguir atualiza **o updateWindow** no **hybridAgentUpdaterConfiguration**.</span><span class="sxs-lookup"><span data-stu-id="cab33-137">The following example updates the **updateWindow** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="cab33-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cab33-138">Request</span></span>

<span data-ttu-id="cab33-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cab33-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cab33-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="cab33-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_onpremisespublishingprofile_1"
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
# <a name="c"></a>[<span data-ttu-id="cab33-141">C#</span><span class="sxs-lookup"><span data-stu-id="cab33-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-onpremisespublishingprofile-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cab33-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cab33-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-onpremisespublishingprofile-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cab33-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cab33-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-onpremisespublishingprofile-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cab33-144">Java</span><span class="sxs-lookup"><span data-stu-id="cab33-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-onpremisespublishingprofile-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cab33-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="cab33-145">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-deferupdate-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="cab33-146">Exemplo 2: Atualizar adiamentoUpdate no hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="cab33-146">Example 2: Update deferUpdate in the hybridAgentUpdaterConfiguration</span></span> 

<span data-ttu-id="cab33-147">O exemplo a seguir atualiza **deferUpdate** no **hybridAgentUpdaterConfiguration**.</span><span class="sxs-lookup"><span data-stu-id="cab33-147">The following example updates **deferUpdate** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="cab33-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cab33-148">Request</span></span>

<span data-ttu-id="cab33-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cab33-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_onpremisespublishingprofile_2"
}-->

```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration
Content-Type: application/json

{
    "deferUpdate" : "2018-08-20T12:00"
}
```

#### <a name="response"></a><span data-ttu-id="cab33-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="cab33-150">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-allowupdateconfigurationoverride-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="cab33-151">Exemplo 3: Update allowUpdateConfigurationOverride in the hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="cab33-151">Example 3: Update allowUpdateConfigurationOverride in the hybridAgentUpdaterConfiguration</span></span>

<span data-ttu-id="cab33-152">O exemplo a seguir atualiza **allowUpdateConfigurationOverride** no **hybridAgentUpdaterConfiguration**.</span><span class="sxs-lookup"><span data-stu-id="cab33-152">The following example updates **allowUpdateConfigurationOverride** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="cab33-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cab33-153">Request</span></span>

<span data-ttu-id="cab33-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cab33-154">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cab33-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="cab33-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_onpremisespublishingprofile_3"
}-->

```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration
Content-Type: application/json

{
    "allowUpdateConfigurationOverride" : false
}
```
# <a name="c"></a>[<span data-ttu-id="cab33-156">C#</span><span class="sxs-lookup"><span data-stu-id="cab33-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-onpremisespublishingprofile-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cab33-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cab33-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-onpremisespublishingprofile-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cab33-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cab33-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-onpremisespublishingprofile-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cab33-159">Java</span><span class="sxs-lookup"><span data-stu-id="cab33-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-onpremisespublishingprofile-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cab33-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="cab33-160">Response</span></span>

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



