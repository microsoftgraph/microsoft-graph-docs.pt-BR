---
title: 'directoryObject: validateProperties'
description: Valide se apelido de nome ou email de exibição de um grupo Office 365 está em conformidade com as políticas de nomenclatura.  Os clientes podem usar a API para determinar se um nome para exibição ou apelido de email é válido antes de tentar **criar** um grupo do Office 365. Para validar as propriedades de um grupo existente, use a função validateProperties para grupos.
ms.openlocfilehash: 82592eff14829fdd8ae1d74c87f43402a3938adf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034588"
---
# <a name="directoryobject-validateproperties"></a><span data-ttu-id="e6767-105">directoryObject: validateProperties</span><span class="sxs-lookup"><span data-stu-id="e6767-105">directoryObject: validateProperties</span></span>

<span data-ttu-id="e6767-106">Valide se apelido de nome ou email de exibição de um grupo Office 365 está em conformidade com as políticas de nomenclatura.</span><span class="sxs-lookup"><span data-stu-id="e6767-106">Validate if an Office 365 group's display name or mail nickname complies with naming policies.</span></span>  <span data-ttu-id="e6767-107">Os clientes podem usar a API para determinar se um nome para exibição ou apelido de email é válido antes de tentar **criar** um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="e6767-107">Clients can use the API to determine if a display name or mail nickname is valid before trying to **create** an Office 365 group.</span></span> <span data-ttu-id="e6767-108">Para validar as propriedades de um grupo existente, use a [função validateProperties](group-validateproperties.md) para grupos.</span><span class="sxs-lookup"><span data-stu-id="e6767-108">For validating properties of an existing group, use the [validateProperties function](group-validateproperties.md) for groups.</span></span>

<span data-ttu-id="e6767-109">As validações a seguintes são executadas para as propriedades de apelido de email e o nome de exibição:</span><span class="sxs-lookup"><span data-stu-id="e6767-109">The following validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="e6767-110">Validar os prefixos e sufixos de diretiva de nomenclatura</span><span class="sxs-lookup"><span data-stu-id="e6767-110">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="e6767-111">Validar a política de palavras proibidos personalizadas</span><span class="sxs-lookup"><span data-stu-id="e6767-111">Validate the custom banned words policy</span></span>
3. <span data-ttu-id="e6767-112">Validar o email apelido é exclusivo</span><span class="sxs-lookup"><span data-stu-id="e6767-112">Validate the mail nickname is unique</span></span>

<span data-ttu-id="e6767-113">Essa API retorna com a primeira falha encontrada.</span><span class="sxs-lookup"><span data-stu-id="e6767-113">This API returns with the first failure encountered.</span></span> <span data-ttu-id="e6767-114">Se uma ou mais propriedades falharem validações vários, apenas a propriedade com a primeira falha de validação será retornada.</span><span class="sxs-lookup"><span data-stu-id="e6767-114">If one or more properties fail multiple validations, only the property with the first validation failure is returned.</span></span> <span data-ttu-id="e6767-115">No entanto, você pode validar o apelido de email e o nome para exibição e receber uma coleção de erros de validação, se você estiver validando somente os prefixos e sufixos de diretiva de nomenclatura.</span><span class="sxs-lookup"><span data-stu-id="e6767-115">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6767-116">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e6767-116">Prerequisites</span></span>

<span data-ttu-id="e6767-117">A seguinte **permissão** é necessária para executar essa API: *Group.Read.All*</span><span class="sxs-lookup"><span data-stu-id="e6767-117">The following **permission** is required to execute this API: *Group.Read.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="e6767-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6767-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="e6767-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6767-119">Request headers</span></span>

| <span data-ttu-id="e6767-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e6767-120">Name</span></span>           | <span data-ttu-id="e6767-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6767-121">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="e6767-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6767-122">Authorization</span></span>  | <span data-ttu-id="e6767-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="e6767-123">Bearer {code}</span></span>    |
| <span data-ttu-id="e6767-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e6767-124">Content-Type</span></span>   | <span data-ttu-id="e6767-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e6767-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e6767-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6767-126">Request body</span></span>
<span data-ttu-id="e6767-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6767-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e6767-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e6767-128">Parameter</span></span>    | <span data-ttu-id="e6767-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6767-129">Type</span></span>   |<span data-ttu-id="e6767-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6767-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6767-131">entityType</span><span class="sxs-lookup"><span data-stu-id="e6767-131">entityType</span></span>|<span data-ttu-id="e6767-132">String</span><span class="sxs-lookup"><span data-stu-id="e6767-132">String</span></span>| <span data-ttu-id="e6767-133">`Group`é o tipo de entidade com suporte apenas.</span><span class="sxs-lookup"><span data-stu-id="e6767-133">`Group` is the only supported entity type.</span></span> |
|<span data-ttu-id="e6767-134">displayName</span><span class="sxs-lookup"><span data-stu-id="e6767-134">displayName</span></span>|<span data-ttu-id="e6767-135">String</span><span class="sxs-lookup"><span data-stu-id="e6767-135">String</span></span>| <span data-ttu-id="e6767-136">O nome de exibição do grupo para validar.</span><span class="sxs-lookup"><span data-stu-id="e6767-136">The display name of the group to validate.</span></span> <span data-ttu-id="e6767-137">A propriedade não é necessária individualmente.</span><span class="sxs-lookup"><span data-stu-id="e6767-137">The property is not individually required.</span></span> <span data-ttu-id="e6767-138">No entanto, pelo menos uma propriedade (displayName ou mailNickname) é necessária.</span><span class="sxs-lookup"><span data-stu-id="e6767-138">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="e6767-139">mailNickname</span><span class="sxs-lookup"><span data-stu-id="e6767-139">mailNickname</span></span>|<span data-ttu-id="e6767-140">String</span><span class="sxs-lookup"><span data-stu-id="e6767-140">String</span></span>| <span data-ttu-id="e6767-141">O apelido de email do grupo para validar.</span><span class="sxs-lookup"><span data-stu-id="e6767-141">The mail nickname of the group to validate.</span></span> <span data-ttu-id="e6767-142">A propriedade não é necessária individualmente.</span><span class="sxs-lookup"><span data-stu-id="e6767-142">The property is not individually required.</span></span> <span data-ttu-id="e6767-143">No entanto, pelo menos uma propriedade (displayName ou mailNickname) é necessária.</span><span class="sxs-lookup"><span data-stu-id="e6767-143">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="e6767-144">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="e6767-144">onBehalfOfUserId</span></span>|<span data-ttu-id="e6767-145">Guid</span><span class="sxs-lookup"><span data-stu-id="e6767-145">Guid</span></span>| <span data-ttu-id="e6767-146">A ID de objeto do usuário para representar ao chamar a API.</span><span class="sxs-lookup"><span data-stu-id="e6767-146">The object ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="e6767-147">Os resultados de validação são para os atributos e funções de onBehalfOfUserId.</span><span class="sxs-lookup"><span data-stu-id="e6767-147">The validation results are for the onBehalfOfUserId's attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="e6767-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6767-148">Response</span></span>

<span data-ttu-id="e6767-149">Se tiver êxito e não houver nenhum erro de validação, o método retornará `204 No Content` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="e6767-149">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="e6767-150">Ele não retornará nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6767-150">It does not return anything in the response body.</span></span>

<span data-ttu-id="e6767-151">Se a solicitação for inválida, o método retornará `400 Bad Request` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="e6767-151">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="e6767-152">Uma mensagem de erro com detalhes sobre a solicitação inválida é retornada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6767-152">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="e6767-153">Se houver um erro de validação, o método retornará `422 Unprocessable Entity` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="e6767-153">If there is a validation error, the method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="e6767-154">Uma mensagem de erro e uma coleção de detalhes do erro será retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6767-154">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e6767-155">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e6767-155">Examples</span></span>

<span data-ttu-id="e6767-156">Este é um exemplo de uma solicitação de validação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="e6767-156">This is an example of a successful validation request.</span></span>

### <a name="request"></a><span data-ttu-id="e6767-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6767-157">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryobject_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

### <a name="response"></a><span data-ttu-id="e6767-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6767-158">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="e6767-159">Este é um exemplo de uma solicitação com erros de validação.</span><span class="sxs-lookup"><span data-stu-id="e6767-159">This is an example of a request with validation errors.</span></span>

### <a name="request"></a><span data-ttu-id="e6767-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6767-160">Request</span></span>
```http
POST https://graph.microsoft.com/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "test",
  "mailNickname": "test",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

### <a name="response"></a><span data-ttu-id="e6767-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6767-161">Response</span></span>
```http
HTTP/1.1 422 
Content-Type: application/json

{
  "error": {
    "code": "Request_UnprocessableEntity",
    "message": "The values provided contain one or more validation errors.",
    "innerError": {
      "request-id": "request-id-value",
      "date": "date-value"
    },
    "details": [
      {
        "target": "displayName",
        "code": "MissingPrefixSuffix",
        "message": "Property mailNickname is missing a required prefix/suffix per your organization's Group naming requirements.",
        "prefix": "Myprefix_",
        "suffix": "_mysuffix"
      },
      {
        "target": "mailNickname",
        "code": "MissingPrefixSuffix",
        "message": "Property mailNickname is missing a required prefix/suffix per your organization's Group naming requirements.",
        "prefix": "Myprefix_",
        "suffix": "_mysuffix"
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: validateProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
