---
title: Atualizar workforceintegration
description: Atualiza as propriedades de um objeto workforceintegration.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4c87031c5d8957e4014f491f671c05b7a10b4934
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451263"
---
# <a name="update-workforceintegration"></a><span data-ttu-id="095c5-103">Atualizar workforceintegration</span><span class="sxs-lookup"><span data-stu-id="095c5-103">Update workforceintegration</span></span>

<span data-ttu-id="095c5-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="095c5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="095c5-105">Atualiza as propriedades de um objeto [workforceintegration](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="095c5-105">Update the properties of a [workforceintegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="095c5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="095c5-106">Permissions</span></span>

<span data-ttu-id="095c5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="095c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="095c5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="095c5-109">Permission type</span></span>                        | <span data-ttu-id="095c5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="095c5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="095c5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="095c5-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="095c5-112">WorkforceIntegration. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="095c5-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="095c5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="095c5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="095c5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="095c5-114">Not supported.</span></span> |
| <span data-ttu-id="095c5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="095c5-115">Application</span></span>                            | <span data-ttu-id="095c5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="095c5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="095c5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="095c5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="095c5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="095c5-118">Request headers</span></span>

| <span data-ttu-id="095c5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="095c5-119">Name</span></span>       | <span data-ttu-id="095c5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="095c5-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="095c5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="095c5-121">Authorization</span></span> | <span data-ttu-id="095c5-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="095c5-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="095c5-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="095c5-123">Request body</span></span>

<span data-ttu-id="095c5-124">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="095c5-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="095c5-125">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="095c5-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="095c5-126">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="095c5-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="095c5-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="095c5-127">Property</span></span>     | <span data-ttu-id="095c5-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="095c5-128">Type</span></span>        | <span data-ttu-id="095c5-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="095c5-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="095c5-130">apiVersion</span><span class="sxs-lookup"><span data-stu-id="095c5-130">apiVersion</span></span>|<span data-ttu-id="095c5-131">Int32</span><span class="sxs-lookup"><span data-stu-id="095c5-131">Int32</span></span>|<span data-ttu-id="095c5-132">Versão da API para a URL de retorno de chamada.</span><span class="sxs-lookup"><span data-stu-id="095c5-132">API version for the call back url.</span></span> <span data-ttu-id="095c5-133">Comece com 1.</span><span class="sxs-lookup"><span data-stu-id="095c5-133">Start with 1.</span></span>|
|<span data-ttu-id="095c5-134">displayName</span><span class="sxs-lookup"><span data-stu-id="095c5-134">displayName</span></span>|<span data-ttu-id="095c5-135">String</span><span class="sxs-lookup"><span data-stu-id="095c5-135">String</span></span>|<span data-ttu-id="095c5-136">Nome da integração da força de funcionários.</span><span class="sxs-lookup"><span data-stu-id="095c5-136">Name of the workforce integration.</span></span>|
|<span data-ttu-id="095c5-137">encripta</span><span class="sxs-lookup"><span data-stu-id="095c5-137">encryption</span></span>|<span data-ttu-id="095c5-138">workforceIntegrationEncryption</span><span class="sxs-lookup"><span data-stu-id="095c5-138">workforceIntegrationEncryption</span></span>|<span data-ttu-id="095c5-139">O recurso de criptografia de integração da força de funcionários.</span><span class="sxs-lookup"><span data-stu-id="095c5-139">The workforce integration encryption resource.</span></span> |
|<span data-ttu-id="095c5-140">isActive</span><span class="sxs-lookup"><span data-stu-id="095c5-140">isActive</span></span>|<span data-ttu-id="095c5-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="095c5-141">Boolean</span></span>|<span data-ttu-id="095c5-142">Indica se a integração da força de trabalho está ativa e disponível atualmente.</span><span class="sxs-lookup"><span data-stu-id="095c5-142">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="095c5-143">compatível</span><span class="sxs-lookup"><span data-stu-id="095c5-143">supports</span></span>|<span data-ttu-id="095c5-144">string</span><span class="sxs-lookup"><span data-stu-id="095c5-144">string</span></span>| <span data-ttu-id="095c5-145">`none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span><span class="sxs-lookup"><span data-stu-id="095c5-145">`none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span></span> <span data-ttu-id="095c5-146">Se selecionar mais de um valor, todos os valores devem começar com a primeira letra em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="095c5-146">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="095c5-147">url</span><span class="sxs-lookup"><span data-stu-id="095c5-147">url</span></span>|<span data-ttu-id="095c5-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="095c5-148">String</span></span>| <span data-ttu-id="095c5-149">URL de integração de força de obra para retornos de chamada do serviço de turno.</span><span class="sxs-lookup"><span data-stu-id="095c5-149">Workforce Integration url for callbacks from the Shift service.</span></span> |

## <a name="response"></a><span data-ttu-id="095c5-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="095c5-150">Response</span></span>

<span data-ttu-id="095c5-151">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [workforceIntegration](../resources/workforceintegration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="095c5-151">If successful, this method returns a `200 OK` response code and an updated [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="095c5-152">Exemplos</span><span class="sxs-lookup"><span data-stu-id="095c5-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="095c5-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="095c5-153">Request</span></span>

<span data-ttu-id="095c5-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="095c5-154">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="095c5-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="095c5-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_workforceintegration"
}-->

```http
PATCH https://graph.microsoft.com/beta/teamwork/workforceIntegrations
Content-type: application/json

{
  "displayName": "displayName-value",
  "apiVersion": 99,
  "encryption": {
    "protocol": "protocol-value",
    "secret": "secret-value"
  },
  "isActive": true,
  "url": "url-value",
  "supports": "supports-value"
}
```
# <a name="c"></a>[<span data-ttu-id="095c5-156">C#</span><span class="sxs-lookup"><span data-stu-id="095c5-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="095c5-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="095c5-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="095c5-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="095c5-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="095c5-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="095c5-159">Response</span></span>

<span data-ttu-id="095c5-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="095c5-160">The following is an example of the response.</span></span>

> <span data-ttu-id="095c5-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="095c5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "displayName-value",
  "apiVersion": 99,
  "encryption": {
    "protocol": "protocol-value",
    "secret": "secret-value"
  },
  "isActive": true,
  "url": "url-value",
  "supports": "supports-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update workforceintegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
