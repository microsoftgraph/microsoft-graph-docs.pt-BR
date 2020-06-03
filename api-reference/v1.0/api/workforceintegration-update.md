---
title: Atualizar workforceIntegration
description: Atualiza as propriedades de um objeto workforceIntegration.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d6eee25246d0851bd442bbbb10b9f9c2bfc646cf
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44218081"
---
# <a name="update-workforceintegration"></a><span data-ttu-id="5f080-103">Atualizar workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="5f080-103">Update workforceIntegration</span></span>

<span data-ttu-id="5f080-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f080-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5f080-105">Atualiza as propriedades de um objeto [workforceIntegration](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="5f080-105">Update the properties of a [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f080-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5f080-106">Permissions</span></span>

<span data-ttu-id="5f080-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f080-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5f080-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f080-109">Permission type</span></span>                        | <span data-ttu-id="5f080-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5f080-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5f080-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f080-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="5f080-112">WorkforceIntegration. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="5f080-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="5f080-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f080-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f080-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f080-114">Not supported.</span></span> |
| <span data-ttu-id="5f080-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5f080-115">Application</span></span>                            | <span data-ttu-id="5f080-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f080-116">Not supported.</span></span> |

> <span data-ttu-id="5f080-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="5f080-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="5f080-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="5f080-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="5f080-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f080-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="5f080-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f080-120">Request headers</span></span>

| <span data-ttu-id="5f080-121">Nome</span><span class="sxs-lookup"><span data-stu-id="5f080-121">Name</span></span>       | <span data-ttu-id="5f080-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f080-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5f080-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f080-123">Authorization</span></span> | <span data-ttu-id="5f080-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="5f080-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5f080-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5f080-125">Request body</span></span>

<span data-ttu-id="5f080-126">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="5f080-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="5f080-127">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="5f080-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5f080-128">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="5f080-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5f080-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5f080-129">Property</span></span>     | <span data-ttu-id="5f080-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f080-130">Type</span></span>        | <span data-ttu-id="5f080-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f080-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5f080-132">apiVersion</span><span class="sxs-lookup"><span data-stu-id="5f080-132">apiVersion</span></span>|<span data-ttu-id="5f080-133">Int32</span><span class="sxs-lookup"><span data-stu-id="5f080-133">Int32</span></span>|<span data-ttu-id="5f080-134">Versão da API para a URL de retorno de chamada.</span><span class="sxs-lookup"><span data-stu-id="5f080-134">API version for the call back URL.</span></span> <span data-ttu-id="5f080-135">Comece com 1.</span><span class="sxs-lookup"><span data-stu-id="5f080-135">Start with 1.</span></span>|
|<span data-ttu-id="5f080-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5f080-136">displayName</span></span>|<span data-ttu-id="5f080-137">String</span><span class="sxs-lookup"><span data-stu-id="5f080-137">String</span></span>|<span data-ttu-id="5f080-138">Nome da integração da força de funcionários.</span><span class="sxs-lookup"><span data-stu-id="5f080-138">Name of the workforce integration.</span></span>|
|<span data-ttu-id="5f080-139">encripta</span><span class="sxs-lookup"><span data-stu-id="5f080-139">encryption</span></span>|<span data-ttu-id="5f080-140">workforceIntegrationEncryption</span><span class="sxs-lookup"><span data-stu-id="5f080-140">workforceIntegrationEncryption</span></span>|<span data-ttu-id="5f080-141">O recurso de criptografia de integração da força de funcionários.</span><span class="sxs-lookup"><span data-stu-id="5f080-141">The workforce integration encryption resource.</span></span> |
|<span data-ttu-id="5f080-142">isActive</span><span class="sxs-lookup"><span data-stu-id="5f080-142">isActive</span></span>|<span data-ttu-id="5f080-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="5f080-143">Boolean</span></span>|<span data-ttu-id="5f080-144">Indica se a integração da força de trabalho está ativa e disponível atualmente.</span><span class="sxs-lookup"><span data-stu-id="5f080-144">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="5f080-145">supportedEntities</span><span class="sxs-lookup"><span data-stu-id="5f080-145">supportedEntities</span></span>|<span data-ttu-id="5f080-146">string</span><span class="sxs-lookup"><span data-stu-id="5f080-146">string</span></span>| <span data-ttu-id="5f080-147">Os possíveis valores são: `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span><span class="sxs-lookup"><span data-stu-id="5f080-147">Possible values are: `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span></span> <span data-ttu-id="5f080-148">Se selecionar mais de um valor, todos os valores devem começar com a primeira letra em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="5f080-148">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="5f080-149">url</span><span class="sxs-lookup"><span data-stu-id="5f080-149">url</span></span>|<span data-ttu-id="5f080-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f080-150">String</span></span>| <span data-ttu-id="5f080-151">URL de integração de força de obra para retornos de chamada do serviço de turno.</span><span class="sxs-lookup"><span data-stu-id="5f080-151">Workforce integration URL for callbacks from the shift service.</span></span> |

## <a name="response"></a><span data-ttu-id="5f080-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f080-152">Response</span></span>

<span data-ttu-id="5f080-153">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [workforceIntegration](../resources/workforceintegration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5f080-153">If successful, this method returns a `200 OK` response code and an updated [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5f080-154">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5f080-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5f080-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f080-155">Request</span></span>

<span data-ttu-id="5f080-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f080-156">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5f080-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="5f080-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_workforceintegration"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations
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
# <a name="c"></a>[<span data-ttu-id="5f080-158">C#</span><span class="sxs-lookup"><span data-stu-id="5f080-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5f080-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f080-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5f080-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5f080-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5f080-161">Java</span><span class="sxs-lookup"><span data-stu-id="5f080-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-workforceintegration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="5f080-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f080-162">Response</span></span>

<span data-ttu-id="5f080-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5f080-163">The following is an example of the response.</span></span>

> <span data-ttu-id="5f080-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5f080-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

## <a name="examples-use-cases-of-workforceintegration-entity-for-filtering-by-wfm-rules-eligibility"></a><span data-ttu-id="5f080-166">Exemplos de uso da entidade WorkforceIntegration para filtragem pela elegibilidade de regras do WFM</span><span class="sxs-lookup"><span data-stu-id="5f080-166">Examples Use cases of WorkforceIntegration entity for Filtering by WFM rules eligibility</span></span>

### <a name="use-case-replace-an-existing-workforceintegration-to-enable-swaprequest-for-eligibility-filtering"></a><span data-ttu-id="5f080-167">Caso de uso: substitua um WorkforceIntegration existente para habilitar o SwapRequest para filtragem de qualificação</span><span class="sxs-lookup"><span data-stu-id="5f080-167">Use case: Replace an existing WorkforceIntegration to enable SwapRequest for eligibility filtering</span></span>

### <a name="request"></a><span data-ttu-id="5f080-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f080-168">Request</span></span>

<span data-ttu-id="5f080-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f080-169">The following is an example of the request.</span></span> 
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
### <a name="response"></a><span data-ttu-id="5f080-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f080-170">Response</span></span>

<span data-ttu-id="5f080-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5f080-171">The following is an example of the response.</span></span>
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
<span data-ttu-id="5f080-172">Para ver como criar um novo workforceintegration com o SwapRequest habilitado para filtragem de qualificação, consulte [Create](../api/workforceintegration-post.md).</span><span class="sxs-lookup"><span data-stu-id="5f080-172">To see how to create a new workforceintegration with SwapRequest enabled for eligibility filtering, see [Create](../api/workforceintegration-post.md).</span></span>

## <a name="example-of-fetching-eligible-shifts-when-swaprequest-is-included-in-eligibilityfilteringenabledentities"></a><span data-ttu-id="5f080-173">Exemplo de busca de turnos qualificados quando o SwapRequest está incluído no eligibilityFilteringEnabledEntities</span><span class="sxs-lookup"><span data-stu-id="5f080-173">Example of fetching eligible shifts when SwapRequest is included in eligibilityFilteringEnabledEntities</span></span>
<span data-ttu-id="5f080-174">A interação entre o aplicativo turnos e os pontos de extremidade de integração da força de força seguirá o padrão existente.</span><span class="sxs-lookup"><span data-stu-id="5f080-174">The interaction between Shifts app and workforce integration endpoints will follow the existing pattern.</span></span>

### <a name="request"></a><span data-ttu-id="5f080-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f080-175">Request</span></span>

<span data-ttu-id="5f080-176">Veja a seguir um exemplo da solicitação feita por turnos para o ponto de extremidade de integração de força de funcionários para buscar turnos qualificados para uma solicitação de troca.</span><span class="sxs-lookup"><span data-stu-id="5f080-176">The following is an example of the request made by Shifts to the workforce integration endpoint to fetch eligible shifts for a swap request.</span></span>

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
### <a name="response"></a><span data-ttu-id="5f080-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f080-177">Response</span></span>

<span data-ttu-id="5f080-178">Veja a seguir um exemplo da resposta do serviço de integração de força de funcionários.</span><span class="sxs-lookup"><span data-stu-id="5f080-178">The following is an example of the response from the workforce integration service.</span></span>
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
