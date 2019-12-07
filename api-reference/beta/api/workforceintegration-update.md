---
title: Atualizar workforceintegration
description: Atualiza as propriedades de um objeto workforceintegration.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1aa2afb19f380a07d147e82fe37a10304dc097be
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895526"
---
# <a name="update-workforceintegration"></a><span data-ttu-id="96322-103">Atualizar workforceintegration</span><span class="sxs-lookup"><span data-stu-id="96322-103">Update workforceintegration</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96322-104">Atualiza as propriedades de um objeto [workforceintegration](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="96322-104">Update the properties of a [workforceintegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="96322-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="96322-105">Permissions</span></span>

<span data-ttu-id="96322-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96322-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="96322-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96322-108">Permission type</span></span>                        | <span data-ttu-id="96322-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="96322-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="96322-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96322-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="96322-111">WorkforceIntegration. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="96322-111">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="96322-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96322-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96322-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96322-113">Not supported.</span></span> |
| <span data-ttu-id="96322-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96322-114">Application</span></span>                            | <span data-ttu-id="96322-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96322-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="96322-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96322-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="96322-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96322-117">Request headers</span></span>

| <span data-ttu-id="96322-118">Nome</span><span class="sxs-lookup"><span data-stu-id="96322-118">Name</span></span>       | <span data-ttu-id="96322-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="96322-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="96322-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="96322-120">Authorization</span></span> | <span data-ttu-id="96322-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="96322-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="96322-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96322-122">Request body</span></span>

<span data-ttu-id="96322-123">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="96322-123">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="96322-124">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="96322-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="96322-125">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="96322-125">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="96322-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96322-126">Property</span></span>     | <span data-ttu-id="96322-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="96322-127">Type</span></span>        | <span data-ttu-id="96322-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="96322-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="96322-129">apiVersion</span><span class="sxs-lookup"><span data-stu-id="96322-129">apiVersion</span></span>|<span data-ttu-id="96322-130">Int32</span><span class="sxs-lookup"><span data-stu-id="96322-130">Int32</span></span>|<span data-ttu-id="96322-131">Versão da API para a URL de retorno de chamada.</span><span class="sxs-lookup"><span data-stu-id="96322-131">API version for the call back url.</span></span> <span data-ttu-id="96322-132">Comece com 1.</span><span class="sxs-lookup"><span data-stu-id="96322-132">Start with 1.</span></span>|
|<span data-ttu-id="96322-133">displayName</span><span class="sxs-lookup"><span data-stu-id="96322-133">displayName</span></span>|<span data-ttu-id="96322-134">String</span><span class="sxs-lookup"><span data-stu-id="96322-134">String</span></span>|<span data-ttu-id="96322-135">Nome da integração da força de funcionários.</span><span class="sxs-lookup"><span data-stu-id="96322-135">Name of the workforce integration.</span></span>|
|<span data-ttu-id="96322-136">encripta</span><span class="sxs-lookup"><span data-stu-id="96322-136">encryption</span></span>|<span data-ttu-id="96322-137">workforceIntegrationEncryption</span><span class="sxs-lookup"><span data-stu-id="96322-137">workforceIntegrationEncryption</span></span>|<span data-ttu-id="96322-138">O recurso de criptografia de integração da força de funcionários.</span><span class="sxs-lookup"><span data-stu-id="96322-138">The workforce integration encryption resource.</span></span> |
|<span data-ttu-id="96322-139">isActive</span><span class="sxs-lookup"><span data-stu-id="96322-139">isActive</span></span>|<span data-ttu-id="96322-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="96322-140">Boolean</span></span>|<span data-ttu-id="96322-141">Indica se a integração da força de trabalho está ativa e disponível atualmente.</span><span class="sxs-lookup"><span data-stu-id="96322-141">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="96322-142">compatível</span><span class="sxs-lookup"><span data-stu-id="96322-142">supports</span></span>|<span data-ttu-id="96322-143">string</span><span class="sxs-lookup"><span data-stu-id="96322-143">string</span></span>| <span data-ttu-id="96322-144">`none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span><span class="sxs-lookup"><span data-stu-id="96322-144"></span></span> <span data-ttu-id="96322-145">Se selecionar mais de um valor, todos os valores devem começar com a primeira letra em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="96322-145">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="96322-146">url</span><span class="sxs-lookup"><span data-stu-id="96322-146">url</span></span>|<span data-ttu-id="96322-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96322-147">String</span></span>| <span data-ttu-id="96322-148">URL de integração de força de obra para retornos de chamada do serviço de turno.</span><span class="sxs-lookup"><span data-stu-id="96322-148">Workforce Integration url for callbacks from the Shift service.</span></span> |

## <a name="response"></a><span data-ttu-id="96322-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="96322-149">Response</span></span>

<span data-ttu-id="96322-150">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [workforceIntegration](../resources/workforceintegration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96322-150">If successful, this method returns a `200 OK` response code and an updated [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="96322-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="96322-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="96322-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96322-152">Request</span></span>

<span data-ttu-id="96322-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="96322-153">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="96322-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="96322-154">Response</span></span>

<span data-ttu-id="96322-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="96322-155">The following is an example of the response.</span></span>

> <span data-ttu-id="96322-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="96322-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
