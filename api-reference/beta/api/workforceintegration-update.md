---
title: Atualizar workforceintegration
description: Atualize as propriedades de um objeto workforceintegration.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c62a27e7c0a019023bea7549523dc8b9de7582c1
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787993"
---
# <a name="update-workforceintegration"></a><span data-ttu-id="0506e-103">Atualizar workforceintegration</span><span class="sxs-lookup"><span data-stu-id="0506e-103">Update workforceintegration</span></span>

<span data-ttu-id="0506e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0506e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0506e-105">Atualize as propriedades de um [objeto workforceintegration.](../resources/workforceintegration.md)</span><span class="sxs-lookup"><span data-stu-id="0506e-105">Update the properties of a [workforceintegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0506e-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="0506e-106">Permissions</span></span>

<span data-ttu-id="0506e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0506e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0506e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0506e-109">Permission type</span></span>                        | <span data-ttu-id="0506e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0506e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0506e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0506e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0506e-112">WorkforceIntegration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0506e-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="0506e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0506e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0506e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0506e-114">Not supported.</span></span> |
| <span data-ttu-id="0506e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0506e-115">Application</span></span>                            | <span data-ttu-id="0506e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0506e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0506e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0506e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teamwork/workforceIntegrations/{workforceIntegrationId}
```

## <a name="request-headers"></a><span data-ttu-id="0506e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0506e-118">Request headers</span></span>

| <span data-ttu-id="0506e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0506e-119">Name</span></span>       | <span data-ttu-id="0506e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0506e-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0506e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0506e-121">Authorization</span></span> | <span data-ttu-id="0506e-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="0506e-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0506e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0506e-123">Request body</span></span>

<span data-ttu-id="0506e-124">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="0506e-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0506e-125">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="0506e-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0506e-126">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="0506e-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0506e-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0506e-127">Property</span></span>     | <span data-ttu-id="0506e-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="0506e-128">Type</span></span>        | <span data-ttu-id="0506e-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="0506e-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0506e-130">apiVersion</span><span class="sxs-lookup"><span data-stu-id="0506e-130">apiVersion</span></span>|<span data-ttu-id="0506e-131">Int32</span><span class="sxs-lookup"><span data-stu-id="0506e-131">Int32</span></span>|<span data-ttu-id="0506e-132">Versão da API para a URL de retorno de chamada.</span><span class="sxs-lookup"><span data-stu-id="0506e-132">API version for the call back url.</span></span> <span data-ttu-id="0506e-133">Comece com 1.</span><span class="sxs-lookup"><span data-stu-id="0506e-133">Start with 1.</span></span>|
|<span data-ttu-id="0506e-134">displayName</span><span class="sxs-lookup"><span data-stu-id="0506e-134">displayName</span></span>|<span data-ttu-id="0506e-135">String</span><span class="sxs-lookup"><span data-stu-id="0506e-135">String</span></span>|<span data-ttu-id="0506e-136">Nome da integração da força de trabalho.</span><span class="sxs-lookup"><span data-stu-id="0506e-136">Name of the workforce integration.</span></span>|
|<span data-ttu-id="0506e-137">encryption</span><span class="sxs-lookup"><span data-stu-id="0506e-137">encryption</span></span>|<span data-ttu-id="0506e-138">workforceIntegrationEncryption</span><span class="sxs-lookup"><span data-stu-id="0506e-138">workforceIntegrationEncryption</span></span>|<span data-ttu-id="0506e-139">O recurso de criptografia de integração de força de trabalho.</span><span class="sxs-lookup"><span data-stu-id="0506e-139">The workforce integration encryption resource.</span></span> |
|<span data-ttu-id="0506e-140">isActive</span><span class="sxs-lookup"><span data-stu-id="0506e-140">isActive</span></span>|<span data-ttu-id="0506e-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="0506e-141">Boolean</span></span>|<span data-ttu-id="0506e-142">Indica se essa integração de força de trabalho está ativa e disponível no momento.</span><span class="sxs-lookup"><span data-stu-id="0506e-142">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="0506e-143">suporta</span><span class="sxs-lookup"><span data-stu-id="0506e-143">supports</span></span>|<span data-ttu-id="0506e-144">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0506e-144">string</span></span>| <span data-ttu-id="0506e-145">Os valores possíveis `none` são , , , , , `shift` `swapRequest` `openshift` `openShiftRequest` `userShiftPreferences` .</span><span class="sxs-lookup"><span data-stu-id="0506e-145">Possible values are `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span></span> <span data-ttu-id="0506e-146">Se selecionar mais de um valor, todos os valores devem começar com a primeira letra em maiúscula.</span><span class="sxs-lookup"><span data-stu-id="0506e-146">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="0506e-147">supportedEntities</span><span class="sxs-lookup"><span data-stu-id="0506e-147">supportedEntities</span></span>|<span data-ttu-id="0506e-148">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0506e-148">string</span></span>| <span data-ttu-id="0506e-149">Essa propriedade substituirá **os suportes** em v1.0.</span><span class="sxs-lookup"><span data-stu-id="0506e-149">This property will replace **supports** in v1.0.</span></span> <span data-ttu-id="0506e-150">Recomendamos que você use essa propriedade em vez de **suporte**.</span><span class="sxs-lookup"><span data-stu-id="0506e-150">We recommend that you use this property instead of **supports**.</span></span> <span data-ttu-id="0506e-151">A **propriedade supports** ainda terá suporte na versão beta por enquanto.</span><span class="sxs-lookup"><span data-stu-id="0506e-151">The **supports** property will still be supported in beta for the time being.</span></span> <span data-ttu-id="0506e-152">Os valores possíveis `none` são , , , , , `shift` `swapRequest` `openshift` `openShiftRequest` `userShiftPreferences` .</span><span class="sxs-lookup"><span data-stu-id="0506e-152">Possible values are `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span></span> <span data-ttu-id="0506e-153">Se selecionar mais de um valor, todos os valores devem começar com a primeira letra em maiúscula.</span><span class="sxs-lookup"><span data-stu-id="0506e-153">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="0506e-154">url</span><span class="sxs-lookup"><span data-stu-id="0506e-154">url</span></span>|<span data-ttu-id="0506e-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0506e-155">String</span></span>| <span data-ttu-id="0506e-156">Url de Integração de Força de Trabalho para retornos de chamada do serviço Shift.</span><span class="sxs-lookup"><span data-stu-id="0506e-156">Workforce Integration url for callbacks from the Shift service.</span></span> |

## <a name="response"></a><span data-ttu-id="0506e-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="0506e-157">Response</span></span>

<span data-ttu-id="0506e-158">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [workforceIntegration](../resources/workforceintegration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0506e-158">If successful, this method returns a `200 OK` response code and an updated [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0506e-159">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0506e-159">Examples</span></span>

### <a name="example-1-update-a-workforceintegration-object"></a><span data-ttu-id="0506e-160">Exemplo 1: Atualizar um objeto workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="0506e-160">Example 1: Update a workforceIntegration object</span></span>

<span data-ttu-id="0506e-161">O exemplo a seguir atualiza um **objeto workforceIntegration.**</span><span class="sxs-lookup"><span data-stu-id="0506e-161">The following example updates a **workforceIntegration** object.</span></span>

#### <a name="request"></a><span data-ttu-id="0506e-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0506e-162">Request</span></span>

<span data-ttu-id="0506e-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0506e-163">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0506e-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="0506e-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_workforceintegration"
}-->

```http
PATCH https://graph.microsoft.com/beta/teamwork/workforceIntegrations/{workforceIntegrationId}
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
# <a name="c"></a>[<span data-ttu-id="0506e-165">C#</span><span class="sxs-lookup"><span data-stu-id="0506e-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0506e-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0506e-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0506e-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0506e-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0506e-168">Java</span><span class="sxs-lookup"><span data-stu-id="0506e-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-workforceintegration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0506e-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="0506e-169">Response</span></span>

<span data-ttu-id="0506e-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0506e-170">The following is an example of the response.</span></span>

> <span data-ttu-id="0506e-171">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0506e-171">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-a-new-workforceintegration-with-swaprequest-enabled-for-eligibility-filtering"></a><span data-ttu-id="0506e-172">Exemplo 2: Criar uma nova workforceIntegration com SwapRequest habilitada para filtragem de qualificação</span><span class="sxs-lookup"><span data-stu-id="0506e-172">Example 2: Create a new workforceIntegration with SwapRequest enabled for eligibility filtering</span></span>

<span data-ttu-id="0506e-173">O exemplo a seguir cria uma nova **workforceIntegration** com SwapRequest habilitada para filtragem de qualificação.</span><span class="sxs-lookup"><span data-stu-id="0506e-173">The following example creates a new **workforceIntegration** with SwapRequest enabled for eligibility filtering.</span></span>

#### <a name="request"></a><span data-ttu-id="0506e-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0506e-174">Request</span></span>

<span data-ttu-id="0506e-175">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0506e-175">The following is an example of the request.</span></span> 
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
#### <a name="response"></a><span data-ttu-id="0506e-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="0506e-176">Response</span></span>

<span data-ttu-id="0506e-177">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0506e-177">The following is an example of the response.</span></span>
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
<span data-ttu-id="0506e-178">Para criar uma nova **workforceIntegration** com SwapRequest habilitado para filtragem de qualificação, consulte o [método Create.](../api/workforceintegration-post.md)</span><span class="sxs-lookup"><span data-stu-id="0506e-178">To create a new **workforceIntegration** with SwapRequest enabled for eligibility filtering, see the [Create](../api/workforceintegration-post.md) method.</span></span>

### <a name="example-3-fetching-eligible-shifts-when-swaprequest-is-included-in-eligibilityfilteringenabledentities"></a><span data-ttu-id="0506e-179">Exemplo 3: buscar turnos qualificados quando SwapRequest está incluído em eligibilityFilteringEnabledEntities</span><span class="sxs-lookup"><span data-stu-id="0506e-179">Example 3: Fetching eligible shifts when SwapRequest is included in eligibilityFilteringEnabledEntities</span></span>

<span data-ttu-id="0506e-180">A interação entre o aplicativo Shifts e os pontos de extremidade de integração da força de trabalho seguirá o padrão existente.</span><span class="sxs-lookup"><span data-stu-id="0506e-180">The interaction between Shifts app and workforce integration endpoints will follow the existing pattern.</span></span>

#### <a name="request"></a><span data-ttu-id="0506e-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0506e-181">Request</span></span>

<span data-ttu-id="0506e-182">A seguir, um exemplo da solicitação feita por Shifts para o ponto de extremidade de integração da força de trabalho para buscar turnos qualificados para uma solicitação de troca.</span><span class="sxs-lookup"><span data-stu-id="0506e-182">The following is an example of the request made by Shifts to the workforce integration endpoint to fetch eligible shifts for a swap request.</span></span>

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
#### <a name="response"></a><span data-ttu-id="0506e-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="0506e-183">Response</span></span>

<span data-ttu-id="0506e-184">A seguir, um exemplo da resposta do serviço de integração da força de trabalho.</span><span class="sxs-lookup"><span data-stu-id="0506e-184">The following is an example of the response from the workforce integration service.</span></span>
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

### <a name="example-4-shifts-synchronous-call-back-to-the-workforce-integration-endpoint-when-enabled-for-real-time-notifications-on-timecard-changes"></a><span data-ttu-id="0506e-185">Exemplo 4: altera a chamada síncrona de volta para o ponto de extremidade de integração da força de trabalho quando habilitada para notificações em tempo real em alterações do timeCard.</span><span class="sxs-lookup"><span data-stu-id="0506e-185">Example 4: Shifts synchronous call back to the workforce integration endpoint when enabled for real time notifications on timeCard changes.</span></span>

#### <a name="request"></a><span data-ttu-id="0506e-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0506e-186">Request</span></span>

<span data-ttu-id="0506e-187">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0506e-187">The following is an example of the request.</span></span> 
```
POST https://foobarWorkforceIntegration.com/foobar/v1/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/update
Accept-Language: en-us
X-MS-WFMPassthrough: foobarvalue
Content-type: application/json
{
   "requests":[
      {
         "id":"1",
         "method":"POST",
         "url":"/timecards",
         "headers":{
            "X-MS-Transaction-ID":"1"
         },
         "body":{
            "id":"3895809b-a618-4c0d-86a0-d42b25b7d74f",
            "userId":"a3601044-a1b5-438e-b742-f78d01d68a67",
            "createdDateTime":"2019-03-18T00:00:00.000Z",
            "createdBy":{
               "user":{
                  "id":"a3601044-a1b5-438e-b742-f78d01d68a67",
                  "displayName":"Dwight Schrute"
               }
            },
            "lastModifiedDateTime":"2019-03-18T00:00:00.000Z",
            "lastModifiedBy":{
               "user":{
                  "id":"a3601044-a1b5-438e-b742-f78d01d68a67",
                  "displayName":"Dwight Schrute"
               }
            },
            "state":"onBreak",
            "clockIn":{
               "dateTime":"2019-03-18T00:00:00.000Z",
               "atApprovedLocation":true,
               "notes":null
            },
            "clockOut":null,
            "breaks":[
               {
                  "id":"string",
                  "notes":{
                     "content":"Lunch break",
                     "contentType":"text"
                  },
                  "start":{
                     "dateTime":"2019-03-18T00:00:00.000Z",
                     "atApprovedLocation":true,
                     "notes":{
                        "content":"Started my break 5 minutes early",
                        "contentType":"text"
                     }
                  },
                  "end":null
               }
            ],
            "notes":null,
            "originalEntry":{
               "clockIn":{
                  "dateTime":"2019-03-18T00:00:00.000Z",
                  "atApprovedLocation":true,
                  "notes":null
               },
               "clockOut":null,
               "breaks":[
                  {
                     "id":"4591109b-a618-3e0d-e6a0-d42b25b7231f",
                     "notes":{
                        "content":"Lunch break",
                        "contentType":"text"
                     },
                     "start":{
                        "dateTime":"2019-03-18T00:00:00.000Z",
                        "atApprovedLocation":true,
                        "notes":{
                           "content":"Started my break 5 minutes early",
                           "contentType":"text"
                        }
                     },
                     "end":null
                  }
               ]
            }
         }
      }
   ]
}

```
#### <a name="response"></a><span data-ttu-id="0506e-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="0506e-188">Response</span></span>

<span data-ttu-id="0506e-189">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0506e-189">The following is an example of the response.</span></span>
```
HTTP/1.1 200 OK
Content-type: application/json
{
  "responses":[
    {
      "id": "1",
      "status": 200,
      "body":{
        "eTag": "4000ee23-0000-0700-0000-5d1415f60000",
        "error": null
      }
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


