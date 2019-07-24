---
title: Atualizar onPremisesPublishingProfile
description: Atualiza as propriedades de um objeto onPremisesPublishingProfile.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c2cdd2eafc51e5bd38aed41fcfcae259b5a9fe66
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841077"
---
# <a name="update-onpremisespublishingprofile"></a><span data-ttu-id="202a8-103">Atualizar onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="202a8-103">Update onPremisesPublishingProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="202a8-104">Atualiza as propriedades de um objeto [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="202a8-104">Update the properties of an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="202a8-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="202a8-105">Permissions</span></span>

<span data-ttu-id="202a8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="202a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="202a8-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="202a8-108">Permission type</span></span>                        | <span data-ttu-id="202a8-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="202a8-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="202a8-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="202a8-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="202a8-111">OnPremisesPublishingProfiles. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="202a8-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="202a8-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="202a8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="202a8-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="202a8-113">Not supported.</span></span> |
| <span data-ttu-id="202a8-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="202a8-114">Application</span></span>                            | <span data-ttu-id="202a8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="202a8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="202a8-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="202a8-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/hybridAgentUpdaterConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="202a8-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="202a8-117">Request headers</span></span>

| <span data-ttu-id="202a8-118">Nome</span><span class="sxs-lookup"><span data-stu-id="202a8-118">Name</span></span>       | <span data-ttu-id="202a8-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="202a8-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="202a8-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="202a8-120">Authorization</span></span> | <span data-ttu-id="202a8-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="202a8-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="202a8-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="202a8-122">Request body</span></span>

<span data-ttu-id="202a8-123">No corpo da solicitação, forneça os valores de campos relevantes a serem atualizados.</span><span class="sxs-lookup"><span data-stu-id="202a8-123">In the request body, supply the values for relevant fields to update.</span></span> <span data-ttu-id="202a8-124">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="202a8-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="202a8-125">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="202a8-125">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="202a8-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="202a8-126">Property</span></span>     | <span data-ttu-id="202a8-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="202a8-127">Type</span></span>        | <span data-ttu-id="202a8-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="202a8-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="202a8-129">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="202a8-129">hybridAgentUpdaterConfiguration</span></span>|<span data-ttu-id="202a8-130">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="202a8-130">hybridAgentUpdaterConfiguration</span></span>|<span data-ttu-id="202a8-131">Representa [hybridAgentUpdaterConfiguration](../resources/hybridagentupdaterconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="202a8-131">Represents [hybridAgentUpdaterConfiguration](../resources/hybridagentupdaterconfiguration.md).</span></span>|

## <a name="response"></a><span data-ttu-id="202a8-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="202a8-132">Response</span></span>

<span data-ttu-id="202a8-133">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="202a8-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="202a8-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="202a8-134">Examples</span></span>

### <a name="example-1-update-updatewindow-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="202a8-135">Exemplo 1: atualizar updateWindow no hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="202a8-135">Example 1: Update updateWindow in the hybridAgentUpdaterConfiguration</span></span>

<span data-ttu-id="202a8-136">O exemplo a seguir atualiza o **updateWindow** no **hybridAgentUpdaterConfiguration**.</span><span class="sxs-lookup"><span data-stu-id="202a8-136">The following example updates the **updateWindow** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="202a8-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="202a8-137">Request</span></span>

<span data-ttu-id="202a8-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="202a8-138">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="202a8-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="202a8-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-deferupdate-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="202a8-140">Exemplo 2: atualizar deferUpdate no hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="202a8-140">Example 2: Update deferUpdate in the hybridAgentUpdaterConfiguration</span></span> 

<span data-ttu-id="202a8-141">O exemplo a seguir atualiza o **deferUpdate** no **hybridAgentUpdaterConfiguration**.</span><span class="sxs-lookup"><span data-stu-id="202a8-141">The following example updates **deferUpdate** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="202a8-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="202a8-142">Request</span></span>

<span data-ttu-id="202a8-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="202a8-143">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="202a8-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="202a8-144">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-allowupdateconfigurationoverride-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="202a8-145">Exemplo 3: atualizar allowUpdateConfigurationOverride no hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="202a8-145">Example 3: Update allowUpdateConfigurationOverride in the hybridAgentUpdaterConfiguration</span></span>

<span data-ttu-id="202a8-146">O exemplo a seguir atualiza o **allowUpdateConfigurationOverride** no **hybridAgentUpdaterConfiguration**.</span><span class="sxs-lookup"><span data-stu-id="202a8-146">The following example updates **allowUpdateConfigurationOverride** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="202a8-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="202a8-147">Request</span></span>

<span data-ttu-id="202a8-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="202a8-148">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="202a8-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="202a8-149">Response</span></span>

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
