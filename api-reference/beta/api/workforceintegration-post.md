---
title: Criar workforceIntegration
description: Criar um novo objeto workforceIntegration.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c67023a11f105008361de7167b8adc14ce5cfa40
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970700"
---
# <a name="create-workforceintegration"></a><span data-ttu-id="49196-103">Criar workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="49196-103">Create workforceIntegration</span></span>

<span data-ttu-id="49196-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49196-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49196-105">Criar um novo objeto [workforceIntegration](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="49196-105">Create a new [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="49196-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="49196-106">Permissions</span></span>

<span data-ttu-id="49196-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49196-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="49196-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49196-109">Permission type</span></span>                        | <span data-ttu-id="49196-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="49196-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="49196-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49196-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="49196-112">WorkforceIntegration. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="49196-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="49196-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49196-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49196-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49196-114">Not supported.</span></span> |
| <span data-ttu-id="49196-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49196-115">Application</span></span>                            | <span data-ttu-id="49196-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49196-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="49196-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49196-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="49196-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49196-118">Request headers</span></span>

| <span data-ttu-id="49196-119">Nome</span><span class="sxs-lookup"><span data-stu-id="49196-119">Name</span></span>          | <span data-ttu-id="49196-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="49196-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="49196-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="49196-121">Authorization</span></span> | <span data-ttu-id="49196-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49196-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="49196-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="49196-124">Content-type</span></span> | <span data-ttu-id="49196-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49196-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="49196-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49196-127">Request body</span></span>

<span data-ttu-id="49196-128">No corpo da solicitação, forneça uma representação JSON de um objeto [workforceIntegration](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="49196-128">In the request body, supply a JSON representation of a [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="49196-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="49196-129">Response</span></span>

<span data-ttu-id="49196-130">Se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto [workforceIntegration](../resources/workforceintegration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49196-130">If successful, this method returns a `201 Created` response code and a new [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="49196-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="49196-131">Examples</span></span>

### <a name="example-1-create-a-new-workforceintegration-object"></a><span data-ttu-id="49196-132">Exemplo 1: criar um novo objeto workforceIntegration.</span><span class="sxs-lookup"><span data-stu-id="49196-132">Example 1: Create a new workforceIntegration object.</span></span>

#### <a name="request"></a><span data-ttu-id="49196-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49196-133">Request</span></span>

<span data-ttu-id="49196-134">Veja a seguir um exemplo de uma solicitação para criar um novo objeto **workforceIntegration** .</span><span class="sxs-lookup"><span data-stu-id="49196-134">The following is an example of a request to create a new **workforceIntegration** object.</span></span>

# <a name="http"></a>[<span data-ttu-id="49196-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="49196-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_workforceintegration_from_teamwork"
}-->

```http
POST https://graph.microsoft.com/beta/teamwork/workforceIntegrations
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
# <a name="c"></a>[<span data-ttu-id="49196-136">C#</span><span class="sxs-lookup"><span data-stu-id="49196-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-workforceintegration-from-teamwork-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49196-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49196-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-workforceintegration-from-teamwork-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49196-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49196-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-workforceintegration-from-teamwork-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="49196-139">Java</span><span class="sxs-lookup"><span data-stu-id="49196-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-workforceintegration-from-teamwork-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="49196-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="49196-140">Response</span></span>

<span data-ttu-id="49196-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="49196-141">The following is an example of the response.</span></span>

> <span data-ttu-id="49196-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="49196-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "supports": "supports-value"
}
```

### <a name="example-2-create-a-new-workforceintegration-with-swaprequest-enabled-for-eligibility-filtering"></a><span data-ttu-id="49196-144">Exemplo 2: criar um novo workforceIntegration com o SwapRequest habilitado para filtragem de qualificação</span><span class="sxs-lookup"><span data-stu-id="49196-144">Example 2: Create a new workforceIntegration with SwapRequest enabled for eligibility filtering</span></span>

<span data-ttu-id="49196-145">Veja a seguir um exemplo de uma solicitação com o SwapRequest habilitado para filtragem de qualificação.</span><span class="sxs-lookup"><span data-stu-id="49196-145">The following is an example of a request with SwapRequest enabled for eligibility filtering.</span></span> 

#### <a name="request"></a><span data-ttu-id="49196-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49196-146">Request</span></span>

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
#### <a name="response"></a><span data-ttu-id="49196-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="49196-147">Response</span></span>

<span data-ttu-id="49196-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="49196-148">The following is an example of the response.</span></span>
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
<span data-ttu-id="49196-149">Para atualizar um objeto **workforceIntegration** existente com o SwapRequest habilitado para filtragem de qualificação, confira o método [Update](../api/workforceintegration-update.md) .</span><span class="sxs-lookup"><span data-stu-id="49196-149">To update an existing **workforceIntegration** object with SwapRequest enabled for eligibility filtering, see the [Update](../api/workforceintegration-update.md) method.</span></span>

### <a name="example-3-fetching-eligible-shifts-when-swaprequest-is-included-in-eligibilityfilteringenabledentities"></a><span data-ttu-id="49196-150">Exemplo 3: buscando turnos qualificados quando o SwapRequest está incluído no eligibilityFilteringEnabledEntities</span><span class="sxs-lookup"><span data-stu-id="49196-150">Example 3: Fetching eligible shifts when SwapRequest is included in eligibilityFilteringEnabledEntities</span></span>

<span data-ttu-id="49196-151">A interação entre o aplicativo turnos e os pontos de extremidade de integração da força de força seguirá o padrão existente.</span><span class="sxs-lookup"><span data-stu-id="49196-151">The interaction between Shifts app and workforce integration endpoints will follow the existing pattern.</span></span>

### <a name="request"></a><span data-ttu-id="49196-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49196-152">Request</span></span>

<span data-ttu-id="49196-153">Veja a seguir um exemplo da solicitação feita por turnos para o ponto de extremidade de integração de força de funcionários para buscar turnos qualificados para uma solicitação de troca.</span><span class="sxs-lookup"><span data-stu-id="49196-153">The following is an example of the request made by Shifts to the workforce integration endpoint to fetch eligible shifts for a swap request.</span></span>

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
### <a name="response"></a><span data-ttu-id="49196-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="49196-154">Response</span></span>

<span data-ttu-id="49196-155">Veja a seguir um exemplo da resposta do serviço de integração de força de funcionários.</span><span class="sxs-lookup"><span data-stu-id="49196-155">The following is an example of the response from the workforce integration service.</span></span>
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


