---
title: Atualizar workforceIntegration
description: Atualize as propriedades de um objeto workforceIntegration.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 97a902f38b983105a1815250071b3ef7f8b3d7bd
ms.sourcegitcommit: 6314172db76ba9f2c192d8c099d818c5e772d2b8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2021
ms.locfileid: "49910501"
---
# <a name="update-workforceintegration"></a><span data-ttu-id="18d3a-103">Atualizar workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="18d3a-103">Update workforceIntegration</span></span>

<span data-ttu-id="18d3a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18d3a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="18d3a-105">Atualize as propriedades de um [objeto workforceIntegration.](../resources/workforceintegration.md)</span><span class="sxs-lookup"><span data-stu-id="18d3a-105">Update the properties of a [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="18d3a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="18d3a-106">Permissions</span></span>

<span data-ttu-id="18d3a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18d3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="18d3a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18d3a-109">Permission type</span></span>                        | <span data-ttu-id="18d3a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="18d3a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="18d3a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18d3a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="18d3a-112">WorkforceIntegration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18d3a-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="18d3a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18d3a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18d3a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18d3a-114">Not supported.</span></span> |
| <span data-ttu-id="18d3a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18d3a-115">Application</span></span>                            | <span data-ttu-id="18d3a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18d3a-116">Not supported.</span></span> |

> <span data-ttu-id="18d3a-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="18d3a-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="18d3a-118">Os administradores globais podem acessar grupos dos que não são membros.</span><span class="sxs-lookup"><span data-stu-id="18d3a-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="18d3a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18d3a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teamwork/workforceIntegrations/{workforceIntegrationId}
```

## <a name="request-headers"></a><span data-ttu-id="18d3a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18d3a-120">Request headers</span></span>

| <span data-ttu-id="18d3a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="18d3a-121">Name</span></span>       | <span data-ttu-id="18d3a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="18d3a-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="18d3a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="18d3a-123">Authorization</span></span> | <span data-ttu-id="18d3a-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="18d3a-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="18d3a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18d3a-125">Request body</span></span>

<span data-ttu-id="18d3a-126">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="18d3a-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="18d3a-127">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="18d3a-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="18d3a-128">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="18d3a-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="18d3a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18d3a-129">Property</span></span>     | <span data-ttu-id="18d3a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="18d3a-130">Type</span></span>        | <span data-ttu-id="18d3a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="18d3a-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="18d3a-132">apiVersion</span><span class="sxs-lookup"><span data-stu-id="18d3a-132">apiVersion</span></span>|<span data-ttu-id="18d3a-133">Int32</span><span class="sxs-lookup"><span data-stu-id="18d3a-133">Int32</span></span>|<span data-ttu-id="18d3a-134">Versão da API para a URL de retorno de chamada.</span><span class="sxs-lookup"><span data-stu-id="18d3a-134">API version for the call back URL.</span></span> <span data-ttu-id="18d3a-135">Comece com 1.</span><span class="sxs-lookup"><span data-stu-id="18d3a-135">Start with 1.</span></span>|
|<span data-ttu-id="18d3a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="18d3a-136">displayName</span></span>|<span data-ttu-id="18d3a-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18d3a-137">String</span></span>|<span data-ttu-id="18d3a-138">Nome da integração da força de trabalho.</span><span class="sxs-lookup"><span data-stu-id="18d3a-138">Name of the workforce integration.</span></span>|
|<span data-ttu-id="18d3a-139">criptografia</span><span class="sxs-lookup"><span data-stu-id="18d3a-139">encryption</span></span>|<span data-ttu-id="18d3a-140">workforceIntegrationEncryption</span><span class="sxs-lookup"><span data-stu-id="18d3a-140">workforceIntegrationEncryption</span></span>|<span data-ttu-id="18d3a-141">O recurso de criptografia de integração da força de trabalho.</span><span class="sxs-lookup"><span data-stu-id="18d3a-141">The workforce integration encryption resource.</span></span> |
|<span data-ttu-id="18d3a-142">isActive</span><span class="sxs-lookup"><span data-stu-id="18d3a-142">isActive</span></span>|<span data-ttu-id="18d3a-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="18d3a-143">Boolean</span></span>|<span data-ttu-id="18d3a-144">Indica se essa integração de força de trabalho está ativa e disponível no momento.</span><span class="sxs-lookup"><span data-stu-id="18d3a-144">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="18d3a-145">supportedEntities</span><span class="sxs-lookup"><span data-stu-id="18d3a-145">supportedEntities</span></span>|<span data-ttu-id="18d3a-146">string</span><span class="sxs-lookup"><span data-stu-id="18d3a-146">string</span></span>| <span data-ttu-id="18d3a-147">Os possíveis valores são: `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span><span class="sxs-lookup"><span data-stu-id="18d3a-147">Possible values are: `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span></span> <span data-ttu-id="18d3a-148">Se você selecionar mais de um valor, todos os valores deverão começar com a primeira letra em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="18d3a-148">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="18d3a-149">url</span><span class="sxs-lookup"><span data-stu-id="18d3a-149">url</span></span>|<span data-ttu-id="18d3a-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18d3a-150">String</span></span>| <span data-ttu-id="18d3a-151">URL de integração da força de trabalho para retornos de chamada do serviço de turno.</span><span class="sxs-lookup"><span data-stu-id="18d3a-151">Workforce integration URL for callbacks from the shift service.</span></span> |

## <a name="response"></a><span data-ttu-id="18d3a-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="18d3a-152">Response</span></span>

<span data-ttu-id="18d3a-153">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` [workforceIntegration](../resources/workforceintegration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18d3a-153">If successful, this method returns a `200 OK` response code and an updated [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="18d3a-154">Exemplos</span><span class="sxs-lookup"><span data-stu-id="18d3a-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="18d3a-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18d3a-155">Request</span></span>

<span data-ttu-id="18d3a-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="18d3a-156">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="18d3a-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="18d3a-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_workforceintegration"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations/{workforceIntegrationId}
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
  "supportedEntities": "supportedEntities-value"
}
```
# <a name="c"></a>[<span data-ttu-id="18d3a-158">C#</span><span class="sxs-lookup"><span data-stu-id="18d3a-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="18d3a-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18d3a-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18d3a-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18d3a-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="18d3a-161">Java</span><span class="sxs-lookup"><span data-stu-id="18d3a-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-workforceintegration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="18d3a-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="18d3a-162">Response</span></span>

<span data-ttu-id="18d3a-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="18d3a-163">The following is an example of the response.</span></span>

> <span data-ttu-id="18d3a-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="18d3a-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "supportedEntities": "supportedEntities-value"
}
```

## <a name="examples-use-cases-of-workforceintegration-entity-for-filtering-by-wfm-rules-eligibility"></a><span data-ttu-id="18d3a-166">Exemplos Casos de uso da entidade WorkforceIntegration para filtragem por qualificação de regras WFM</span><span class="sxs-lookup"><span data-stu-id="18d3a-166">Examples Use cases of WorkforceIntegration entity for Filtering by WFM rules eligibility</span></span>

### <a name="use-case-replace-an-existing-workforceintegration-to-enable-swaprequest-for-eligibility-filtering"></a><span data-ttu-id="18d3a-167">Caso de uso: substitua uma WorkforceIntegration existente para habilitar SwapRequest para filtragem de qualificação</span><span class="sxs-lookup"><span data-stu-id="18d3a-167">Use case: Replace an existing WorkforceIntegration to enable SwapRequest for eligibility filtering</span></span>

### <a name="request"></a><span data-ttu-id="18d3a-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18d3a-168">Request</span></span>

<span data-ttu-id="18d3a-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="18d3a-169">The following is an example of the request.</span></span> 
```
PATCH https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations/{workforceIntegrationid}
{
  "displayName": "ABCWorkforceIntegration",
  "apiVersion": 1,
  "isActive": true,
  "encryption": {
    - "protocol": "sharedSecret",
    "secret": "My Secret"
  },
  "url": "https://abcWorkforceIntegration.com/Contoso/",
  "supports": "Shift,SwapRequest",
  "eligibilityFilteringEnabledEntities": "SwapRequest"
}
```
### <a name="response"></a><span data-ttu-id="18d3a-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="18d3a-170">Response</span></span>

<span data-ttu-id="18d3a-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="18d3a-171">The following is an example of the response.</span></span>
```
HTTP/1.1 200 OK
Content-type: application/json
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
<span data-ttu-id="18d3a-172">Para ver como criar uma nova força de trabalho com SwapRequest habilitado para filtragem de qualificação, consulte [Criar](../api/workforceintegration-post.md).</span><span class="sxs-lookup"><span data-stu-id="18d3a-172">To see how to create a new workforceintegration with SwapRequest enabled for eligibility filtering, see [Create](../api/workforceintegration-post.md).</span></span>

## <a name="example-of-fetching-eligible-shifts-when-swaprequest-is-included-in-eligibilityfilteringenabledentities"></a><span data-ttu-id="18d3a-173">Exemplo de busca de turnos qualificados quando SwapRequest é incluído em eligibilityFilteringEnabledEntities</span><span class="sxs-lookup"><span data-stu-id="18d3a-173">Example of fetching eligible shifts when SwapRequest is included in eligibilityFilteringEnabledEntities</span></span>
<span data-ttu-id="18d3a-174">A interação entre os pontos de extremidade de integração do aplicativo Shifts e da força de trabalho seguirá o padrão existente.</span><span class="sxs-lookup"><span data-stu-id="18d3a-174">The interaction between Shifts app and workforce integration endpoints will follow the existing pattern.</span></span>

### <a name="request"></a><span data-ttu-id="18d3a-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18d3a-175">Request</span></span>

<span data-ttu-id="18d3a-176">A seguir está um exemplo da solicitação feita por Shifts ao ponto de extremidade de integração da força de trabalho para buscar turnos qualificados para uma solicitação de troca.</span><span class="sxs-lookup"><span data-stu-id="18d3a-176">The following is an example of the request made by Shifts to the workforce integration endpoint to fetch eligible shifts for a swap request.</span></span>

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
### <a name="response"></a><span data-ttu-id="18d3a-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="18d3a-177">Response</span></span>

<span data-ttu-id="18d3a-178">A seguir está um exemplo da resposta do serviço de integração da força de trabalho.</span><span class="sxs-lookup"><span data-stu-id="18d3a-178">The following is an example of the response from the workforce integration service.</span></span>
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

