---
title: Criar workforceIntegration
description: Crie um novo objeto workforceIntegration.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2eee6b620bcd22e571a2b526d4a43e70fe91416a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055642"
---
# <a name="create-workforceintegration"></a><span data-ttu-id="9f748-103">Criar workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="9f748-103">Create workforceIntegration</span></span>

<span data-ttu-id="9f748-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f748-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9f748-105">Crie um novo [objeto workforceIntegration.](../resources/workforceintegration.md)</span><span class="sxs-lookup"><span data-stu-id="9f748-105">Create a new [workforceIntegration](../resources/workforceintegration.md) object.</span></span>
<span data-ttu-id="9f748-106">Você pode configurar para quais entidades deseja receber notificações de alteração síncrona shifts e definir entidades para configurar a filtragem por qualificação de regras WFM, incluindo solicitações de troca.</span><span class="sxs-lookup"><span data-stu-id="9f748-106">You can set up which entities you want to receive Shifts synchronous change notifications on and set entities to configure filtering by WFM rules eligibility for, including swap requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f748-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="9f748-107">Permissions</span></span>

<span data-ttu-id="9f748-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f748-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9f748-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f748-110">Permission type</span></span>                        | <span data-ttu-id="9f748-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9f748-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9f748-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f748-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9f748-113">WorkforceIntegration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f748-113">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="9f748-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9f748-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f748-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f748-115">Not supported.</span></span> |
| <span data-ttu-id="9f748-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9f748-116">Application</span></span>                            | <span data-ttu-id="9f748-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f748-117">Not supported.</span></span> |

> <span data-ttu-id="9f748-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="9f748-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="9f748-119">Os administradores globais podem acessar grupos dos que não são membros.</span><span class="sxs-lookup"><span data-stu-id="9f748-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="9f748-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f748-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="9f748-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f748-121">Request headers</span></span>

| <span data-ttu-id="9f748-122">Nome</span><span class="sxs-lookup"><span data-stu-id="9f748-122">Name</span></span>          | <span data-ttu-id="9f748-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f748-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9f748-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9f748-124">Authorization</span></span> | <span data-ttu-id="9f748-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f748-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9f748-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="9f748-127">Content-type</span></span> | <span data-ttu-id="9f748-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f748-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f748-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9f748-130">Request body</span></span>

<span data-ttu-id="9f748-131">No corpo da solicitação, fornece uma representação JSON de um [objeto workforceIntegration.](../resources/workforceintegration.md)</span><span class="sxs-lookup"><span data-stu-id="9f748-131">In the request body, supply a JSON representation of a [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9f748-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f748-132">Response</span></span>

<span data-ttu-id="9f748-133">Se tiver êxito, este método retornará um código `201 Created` de resposta e um novo objeto [workforceIntegration](../resources/workforceintegration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9f748-133">If successful, this method returns a `201 Created` response code and a new [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9f748-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9f748-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9f748-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f748-135">Request</span></span>

<span data-ttu-id="9f748-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9f748-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9f748-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f748-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_workforceintegration_from_teamwork"
}-->

```http
POST https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations
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
# <a name="c"></a>[<span data-ttu-id="9f748-138">C#</span><span class="sxs-lookup"><span data-stu-id="9f748-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-workforceintegration-from-teamwork-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9f748-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f748-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-workforceintegration-from-teamwork-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9f748-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9f748-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-workforceintegration-from-teamwork-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9f748-141">Java</span><span class="sxs-lookup"><span data-stu-id="9f748-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-workforceintegration-from-teamwork-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="9f748-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f748-142">Response</span></span>

<span data-ttu-id="9f748-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9f748-143">The following is an example of the response.</span></span>

> <span data-ttu-id="9f748-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9f748-144">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration"
} -->

```http
HTTP/1.1 201 Created
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

## <a name="examples-for-use-cases-of-workforceintegration-entity-for-filtering-by-wfm-rules-eligibility"></a><span data-ttu-id="9f748-145">Exemplos de casos de uso da entidade WorkforceIntegration para filtragem por qualificação de regras WFM</span><span class="sxs-lookup"><span data-stu-id="9f748-145">Examples for Use cases of WorkforceIntegration entity for Filtering by WFM rules eligibility</span></span>

### <a name="use-case-create-a-new-workforceintegration-with-swaprequest-enabled-for-eligibility-filtering"></a><span data-ttu-id="9f748-146">Caso de uso: Criar uma nova WorkforceIntegration com SwapRequest habilitada para filtragem de qualificação</span><span class="sxs-lookup"><span data-stu-id="9f748-146">Use case: Create a new WorkforceIntegration with SwapRequest enabled for eligibility filtering</span></span>

### <a name="request"></a><span data-ttu-id="9f748-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f748-147">Request</span></span>

<span data-ttu-id="9f748-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9f748-148">The following is an example of the request.</span></span> 
```
POST https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations/
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
Authorization: Bearer {token}
Content-type: application/json
```
### <a name="response"></a><span data-ttu-id="9f748-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f748-149">Response</span></span>

<span data-ttu-id="9f748-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9f748-150">The following is an example of the response.</span></span>
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
<span data-ttu-id="9f748-151">Para ver como atualizar uma força de trabalho existente com SwapRequest habilitado para filtragem de qualificação, consulte [Update](../api/workforceintegration-update.md).</span><span class="sxs-lookup"><span data-stu-id="9f748-151">To see how to update an existing workforceintegration with SwapRequest enabled for eligibility filtering, see [Update](../api/workforceintegration-update.md).</span></span>

## <a name="example-of-fetching-eligible-shifts-when-swaprequest-is-included-in-eligibilityfilteringenabledentities"></a><span data-ttu-id="9f748-152">Exemplo de busca de turnos qualificados quando SwapRequest está incluído em eligibilityFilteringEnabledEntities</span><span class="sxs-lookup"><span data-stu-id="9f748-152">Example of fetching eligible shifts when SwapRequest is included in eligibilityFilteringEnabledEntities</span></span>
<span data-ttu-id="9f748-153">A interação entre o aplicativo Shifts e os pontos de extremidade de integração da força de trabalho seguirá o padrão existente.</span><span class="sxs-lookup"><span data-stu-id="9f748-153">The interaction between Shifts app and workforce integration endpoints will follow the existing pattern.</span></span>

### <a name="request"></a><span data-ttu-id="9f748-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f748-154">Request</span></span>

<span data-ttu-id="9f748-155">A seguir, um exemplo da solicitação feita por Shifts para o ponto de extremidade de integração da força de trabalho para buscar turnos qualificados para uma solicitação de troca.</span><span class="sxs-lookup"><span data-stu-id="9f748-155">The following is an example of the request made by Shifts to the workforce integration endpoint to fetch eligible shifts for a swap request.</span></span>

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
### <a name="response"></a><span data-ttu-id="9f748-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f748-156">Response</span></span>

<span data-ttu-id="9f748-157">A seguir, um exemplo da resposta do serviço de integração da força de trabalho.</span><span class="sxs-lookup"><span data-stu-id="9f748-157">The following is an example of the response from the workforce integration service.</span></span>
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
  "description": "Create workforceIntegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

