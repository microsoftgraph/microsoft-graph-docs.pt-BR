---
title: Atualizar workforceintegration
description: Atualiza as propriedades de um objeto workforceintegration.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a3e73cf0b0dbe0b54b9ac3af5a5378503f336e6a
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870446"
---
# <a name="update-workforceintegration"></a><span data-ttu-id="76092-103">Atualizar workforceintegration</span><span class="sxs-lookup"><span data-stu-id="76092-103">Update workforceintegration</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76092-104">Atualiza as propriedades de um objeto [workforceintegration](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="76092-104">Update the properties of a [workforceintegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="76092-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="76092-105">Permissions</span></span>

<span data-ttu-id="76092-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76092-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="76092-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76092-108">Permission type</span></span>                        | <span data-ttu-id="76092-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="76092-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="76092-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76092-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="76092-111">WorkforceIntegration. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="76092-111">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="76092-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76092-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76092-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76092-113">Not supported.</span></span> |
| <span data-ttu-id="76092-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76092-114">Application</span></span>                            | <span data-ttu-id="76092-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76092-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="76092-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76092-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="76092-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76092-117">Request headers</span></span>

| <span data-ttu-id="76092-118">Nome</span><span class="sxs-lookup"><span data-stu-id="76092-118">Name</span></span>       | <span data-ttu-id="76092-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="76092-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="76092-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="76092-120">Authorization</span></span> | <span data-ttu-id="76092-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="76092-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="76092-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76092-122">Request body</span></span>

<span data-ttu-id="76092-123">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="76092-123">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="76092-124">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="76092-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="76092-125">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="76092-125">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="76092-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="76092-126">Property</span></span>     | <span data-ttu-id="76092-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="76092-127">Type</span></span>        | <span data-ttu-id="76092-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="76092-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="76092-129">apiVersion</span><span class="sxs-lookup"><span data-stu-id="76092-129">apiVersion</span></span>|<span data-ttu-id="76092-130">Int32</span><span class="sxs-lookup"><span data-stu-id="76092-130">Int32</span></span>|<span data-ttu-id="76092-131">Versão da API para a URL de retorno de chamada.</span><span class="sxs-lookup"><span data-stu-id="76092-131">API version for the call back url.</span></span> <span data-ttu-id="76092-132">Comece com 1.</span><span class="sxs-lookup"><span data-stu-id="76092-132">Start with 1.</span></span>|
|<span data-ttu-id="76092-133">displayName</span><span class="sxs-lookup"><span data-stu-id="76092-133">displayName</span></span>|<span data-ttu-id="76092-134">String</span><span class="sxs-lookup"><span data-stu-id="76092-134">String</span></span>|<span data-ttu-id="76092-135">Nome da integração da força de funcionários.</span><span class="sxs-lookup"><span data-stu-id="76092-135">Name of the workforce integration.</span></span>|
|<span data-ttu-id="76092-136">encripta</span><span class="sxs-lookup"><span data-stu-id="76092-136">encryption</span></span>|<span data-ttu-id="76092-137">workforceIntegrationEncryption</span><span class="sxs-lookup"><span data-stu-id="76092-137">workforceIntegrationEncryption</span></span>|<span data-ttu-id="76092-138">O recurso de criptografia de integração da força de funcionários.</span><span class="sxs-lookup"><span data-stu-id="76092-138">The workforce integration encryption resource.</span></span> |
|<span data-ttu-id="76092-139">isActive</span><span class="sxs-lookup"><span data-stu-id="76092-139">isActive</span></span>|<span data-ttu-id="76092-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="76092-140">Boolean</span></span>|<span data-ttu-id="76092-141">Indica se a integração da força de trabalho está ativa e disponível atualmente.</span><span class="sxs-lookup"><span data-stu-id="76092-141">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="76092-142">compatível</span><span class="sxs-lookup"><span data-stu-id="76092-142">supports</span></span>|<span data-ttu-id="76092-143">string</span><span class="sxs-lookup"><span data-stu-id="76092-143">string</span></span>| <span data-ttu-id="76092-144">`none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span><span class="sxs-lookup"><span data-stu-id="76092-144"></span></span> <span data-ttu-id="76092-145">Se selecionar mais de um valor, todos os valores devem começar com a primeira letra em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="76092-145">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="76092-146">url</span><span class="sxs-lookup"><span data-stu-id="76092-146">url</span></span>|<span data-ttu-id="76092-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76092-147">String</span></span>| <span data-ttu-id="76092-148">URL de integração de força de obra para retornos de chamada do serviço de turno.</span><span class="sxs-lookup"><span data-stu-id="76092-148">Workforce Integration url for callbacks from the Shift service.</span></span> |

## <a name="response"></a><span data-ttu-id="76092-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="76092-149">Response</span></span>

<span data-ttu-id="76092-150">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [workforceIntegration](../resources/workforceintegration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="76092-150">If successful, this method returns a `200 OK` response code and an updated [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="76092-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="76092-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="76092-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76092-152">Request</span></span>

<span data-ttu-id="76092-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="76092-153">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="76092-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="76092-154">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="76092-155">C#</span><span class="sxs-lookup"><span data-stu-id="76092-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="76092-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="76092-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="76092-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="76092-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="76092-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="76092-158">Response</span></span>

<span data-ttu-id="76092-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="76092-159">The following is an example of the response.</span></span>

> <span data-ttu-id="76092-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="76092-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
