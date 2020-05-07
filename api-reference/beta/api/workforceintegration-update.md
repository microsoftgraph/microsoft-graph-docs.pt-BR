---
title: Atualizar workforceintegration
description: Atualiza as propriedades de um objeto workforceintegration.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 80b688d700dff94d1a746e651b83a4b0236d1a39
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154399"
---
# <a name="update-workforceintegration"></a><span data-ttu-id="8810d-103">Atualizar workforceintegration</span><span class="sxs-lookup"><span data-stu-id="8810d-103">Update workforceintegration</span></span>

<span data-ttu-id="8810d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8810d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8810d-105">Atualiza as propriedades de um objeto [workforceintegration](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="8810d-105">Update the properties of a [workforceintegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8810d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8810d-106">Permissions</span></span>

<span data-ttu-id="8810d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8810d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8810d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8810d-109">Permission type</span></span>                        | <span data-ttu-id="8810d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8810d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8810d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8810d-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="8810d-112">WorkforceIntegration. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8810d-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="8810d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8810d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8810d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8810d-114">Not supported.</span></span> |
| <span data-ttu-id="8810d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8810d-115">Application</span></span>                            | <span data-ttu-id="8810d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8810d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8810d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8810d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="8810d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8810d-118">Request headers</span></span>

| <span data-ttu-id="8810d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="8810d-119">Name</span></span>       | <span data-ttu-id="8810d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8810d-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8810d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8810d-121">Authorization</span></span> | <span data-ttu-id="8810d-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="8810d-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8810d-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8810d-123">Request body</span></span>

<span data-ttu-id="8810d-124">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="8810d-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8810d-125">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="8810d-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8810d-126">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="8810d-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8810d-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8810d-127">Property</span></span>     | <span data-ttu-id="8810d-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="8810d-128">Type</span></span>        | <span data-ttu-id="8810d-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="8810d-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8810d-130">apiVersion</span><span class="sxs-lookup"><span data-stu-id="8810d-130">apiVersion</span></span>|<span data-ttu-id="8810d-131">Int32</span><span class="sxs-lookup"><span data-stu-id="8810d-131">Int32</span></span>|<span data-ttu-id="8810d-132">Versão da API para a URL de retorno de chamada.</span><span class="sxs-lookup"><span data-stu-id="8810d-132">API version for the call back url.</span></span> <span data-ttu-id="8810d-133">Comece com 1.</span><span class="sxs-lookup"><span data-stu-id="8810d-133">Start with 1.</span></span>|
|<span data-ttu-id="8810d-134">displayName</span><span class="sxs-lookup"><span data-stu-id="8810d-134">displayName</span></span>|<span data-ttu-id="8810d-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8810d-135">String</span></span>|<span data-ttu-id="8810d-136">Nome da integração da força de funcionários.</span><span class="sxs-lookup"><span data-stu-id="8810d-136">Name of the workforce integration.</span></span>|
|<span data-ttu-id="8810d-137">encripta</span><span class="sxs-lookup"><span data-stu-id="8810d-137">encryption</span></span>|<span data-ttu-id="8810d-138">workforceIntegrationEncryption</span><span class="sxs-lookup"><span data-stu-id="8810d-138">workforceIntegrationEncryption</span></span>|<span data-ttu-id="8810d-139">O recurso de criptografia de integração da força de funcionários.</span><span class="sxs-lookup"><span data-stu-id="8810d-139">The workforce integration encryption resource.</span></span> |
|<span data-ttu-id="8810d-140">isActive</span><span class="sxs-lookup"><span data-stu-id="8810d-140">isActive</span></span>|<span data-ttu-id="8810d-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="8810d-141">Boolean</span></span>|<span data-ttu-id="8810d-142">Indica se a integração da força de trabalho está ativa e disponível atualmente.</span><span class="sxs-lookup"><span data-stu-id="8810d-142">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="8810d-143">compatível</span><span class="sxs-lookup"><span data-stu-id="8810d-143">supports</span></span>|<span data-ttu-id="8810d-144">string</span><span class="sxs-lookup"><span data-stu-id="8810d-144">string</span></span>| <span data-ttu-id="8810d-145">Os valores possíveis `none`são `shift`: `swapRequest` `openshift` `openShiftRequest`,,, `userShiftPreferences`,.</span><span class="sxs-lookup"><span data-stu-id="8810d-145">Possible values are `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span></span> <span data-ttu-id="8810d-146">Se selecionar mais de um valor, todos os valores devem começar com a primeira letra em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="8810d-146">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="8810d-147">supportedEntities</span><span class="sxs-lookup"><span data-stu-id="8810d-147">supportedEntities</span></span>|<span data-ttu-id="8810d-148">string</span><span class="sxs-lookup"><span data-stu-id="8810d-148">string</span></span>| <span data-ttu-id="8810d-149">Essa propriedade substituirá **suporte** em v 1.0.</span><span class="sxs-lookup"><span data-stu-id="8810d-149">This property will replace **supports** in v1.0.</span></span> <span data-ttu-id="8810d-150">Recomendamos que você use essa propriedade em vez de **suportar**.</span><span class="sxs-lookup"><span data-stu-id="8810d-150">We recommend that you use this property instead of **supports**.</span></span> <span data-ttu-id="8810d-151">A **Propriedade** Supports ainda será suportada na versão beta para o momento.</span><span class="sxs-lookup"><span data-stu-id="8810d-151">The **supports** property will still be supported in beta for the time being.</span></span> <span data-ttu-id="8810d-152">Os valores possíveis `none`são `shift`: `swapRequest` `openshift` `openShiftRequest`,,, `userShiftPreferences`,.</span><span class="sxs-lookup"><span data-stu-id="8810d-152">Possible values are `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span></span> <span data-ttu-id="8810d-153">Se selecionar mais de um valor, todos os valores devem começar com a primeira letra em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="8810d-153">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="8810d-154">url</span><span class="sxs-lookup"><span data-stu-id="8810d-154">url</span></span>|<span data-ttu-id="8810d-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8810d-155">String</span></span>| <span data-ttu-id="8810d-156">URL de integração de força de obra para retornos de chamada do serviço de turno.</span><span class="sxs-lookup"><span data-stu-id="8810d-156">Workforce Integration url for callbacks from the Shift service.</span></span> |

## <a name="response"></a><span data-ttu-id="8810d-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="8810d-157">Response</span></span>

<span data-ttu-id="8810d-158">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [workforceIntegration](../resources/workforceintegration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8810d-158">If successful, this method returns a `200 OK` response code and an updated [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8810d-159">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8810d-159">Examples</span></span>

### <a name="example-1-update-a-workforceintegration-object"></a><span data-ttu-id="8810d-160">Exemplo 1: atualizar um objeto workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="8810d-160">Example 1: Update a workforceIntegration object</span></span>

<span data-ttu-id="8810d-161">O exemplo a seguir atualiza um objeto **workforceIntegration** .</span><span class="sxs-lookup"><span data-stu-id="8810d-161">The following example updates a **workforceIntegration** object.</span></span>

#### <a name="request"></a><span data-ttu-id="8810d-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8810d-162">Request</span></span>

<span data-ttu-id="8810d-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8810d-163">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8810d-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="8810d-164">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8810d-165">C#</span><span class="sxs-lookup"><span data-stu-id="8810d-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8810d-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8810d-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8810d-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8810d-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8810d-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="8810d-168">Response</span></span>

<span data-ttu-id="8810d-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8810d-169">The following is an example of the response.</span></span>

> <span data-ttu-id="8810d-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8810d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-create-a-new-workforceintegration-with-swaprequest-enabled-for-eligibility-filtering"></a><span data-ttu-id="8810d-172">Exemplo 2: criar um novo workforceIntegration com o SwapRequest habilitado para filtragem de qualificação</span><span class="sxs-lookup"><span data-stu-id="8810d-172">Example 2: Create a new workforceIntegration with SwapRequest enabled for eligibility filtering</span></span>

<span data-ttu-id="8810d-173">O exemplo a seguir cria um novo **workforceIntegration** com SwapRequest habilitado para filtragem de qualificação.</span><span class="sxs-lookup"><span data-stu-id="8810d-173">The following example creates a new **workforceIntegration** with SwapRequest enabled for eligibility filtering.</span></span>

#### <a name="request"></a><span data-ttu-id="8810d-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8810d-174">Request</span></span>

<span data-ttu-id="8810d-175">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8810d-175">The following is an example of the request.</span></span> 
```
POST https://graph.microsoft.com/beta/teamwork/workforceIntegrations/
Authorization: Bearer {token}
Content-type: application/json

{
  "displayName": "ABCWorkforceIntegration",
  "apiVersion": 1,
  "isActive": true,
  "encryption": {
    "protocol": "sharedSecret",
    "secret": "My Secret"
  },
  "url": "https://ABCWorkforceIntegration.com/Contoso/",
  "supports": "Shift,SwapRequest",
  "eligibilityFilteringEnabledEntities": "SwapRequest"
}

```
#### <a name="response"></a><span data-ttu-id="8810d-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="8810d-176">Response</span></span>

<span data-ttu-id="8810d-177">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8810d-177">The following is an example of the response.</span></span>
```
HTTP/1.1 200 OK
{
  "id": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "displayName": "ABCWorkforceIntegration",
  "apiVersion": 1,
  "isActive": true,
  "encryption": {
    "protocol": "sharedSecret",
    "secret": null
  },
  "url": "https://abcWorkforceIntegration.com/Contoso/",
  "supports": "Shift,SwapRequest",
  "eligibilityFilteringEnabledEntities": "SwapRequest"
}

```
<span data-ttu-id="8810d-178">Para criar um novo **workforceIntegration** com o SwapRequest habilitado para filtragem de qualificação, confira o método [Create](../api/workforceintegration-post.md) .</span><span class="sxs-lookup"><span data-stu-id="8810d-178">To create a new **workforceIntegration** with SwapRequest enabled for eligibility filtering, see the [Create](../api/workforceintegration-post.md) method.</span></span>

### <a name="example-3-fetching-eligible-shifts-when-swaprequest-is-included-in-eligibilityfilteringenabledentities"></a><span data-ttu-id="8810d-179">Exemplo 3: buscando turnos qualificados quando o SwapRequest está incluído no eligibilityFilteringEnabledEntities</span><span class="sxs-lookup"><span data-stu-id="8810d-179">Example 3: Fetching eligible shifts when SwapRequest is included in eligibilityFilteringEnabledEntities</span></span>

<span data-ttu-id="8810d-180">A interação entre o aplicativo turnos e os pontos de extremidade de integração da força de força seguirá o padrão existente.</span><span class="sxs-lookup"><span data-stu-id="8810d-180">The interaction between Shifts app and workforce integration endpoints will follow the existing pattern.</span></span>

#### <a name="request"></a><span data-ttu-id="8810d-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8810d-181">Request</span></span>

<span data-ttu-id="8810d-182">Veja a seguir um exemplo da solicitação feita por turnos para o ponto de extremidade de integração de força de funcionários para buscar turnos qualificados para uma solicitação de troca.</span><span class="sxs-lookup"><span data-stu-id="8810d-182">The following is an example of the request made by Shifts to the workforce integration endpoint to fetch eligible shifts for a swap request.</span></span>

```
POST https://abcWorkforceIntegration.com/Contoso/{apiVersion}/team/{teamId}/read
Accept-Language: en-us

{
  "requests": [
  {
     "id": "{shiftId}",
     "method": "GET”,
     "url": “/shifts/{shiftId}/requestableShifts?requestType={requestType}&startDateTime={startDateTime}&endDateTime={endDateTime}”
   }]
}
```
#### <a name="response"></a><span data-ttu-id="8810d-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="8810d-183">Response</span></span>

<span data-ttu-id="8810d-184">Veja a seguir um exemplo da resposta do serviço de integração de força de funcionários.</span><span class="sxs-lookup"><span data-stu-id="8810d-184">The following is an example of the response from the workforce integration service.</span></span>
```
HTTP/1.1 200 OK
{
  "responses": [
  {
    "body": {
      "SHFT_6548f642-cbc1-4228-8621-054327576457",
      "SHFT_6548f642-cbc1-4228-8621-054327571234"
  }
    "id": "{shiftId}",
    "status: 200,
    "body": {
       "data": [{ShiftId}, {ShiftId}...]
       "error": null
    }
  ]
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
