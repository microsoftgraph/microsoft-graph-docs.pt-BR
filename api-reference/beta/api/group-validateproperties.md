---
title: 'grupo: validateProperties'
description: Valide se apelido de nome ou email de exibição de um grupo Office 365 está em conformidade com as políticas de nomenclatura. Os clientes podem usar a API para determinar se um nome para exibição ou apelido de email é válido antes de tentar **Atualizar** um grupo do Office 365. Para validar as propriedades antes de criar um grupo, use a função de validateProperties para objetos de diretório.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 5361e05d2a58e2d4c27bd662f158d4f185c447fe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990884"
---
# <a name="group-validateproperties"></a><span data-ttu-id="eccd1-105">grupo: validateProperties</span><span class="sxs-lookup"><span data-stu-id="eccd1-105">group: validateProperties</span></span>

<span data-ttu-id="eccd1-106">Valide se apelido de nome ou email de exibição de um grupo Office 365 está em conformidade com as políticas de nomenclatura.</span><span class="sxs-lookup"><span data-stu-id="eccd1-106">Validate if an Office 365 group's display name or mail nickname complies with naming policies.</span></span> <span data-ttu-id="eccd1-107">Os clientes podem usar a API para determinar se um nome para exibição ou apelido de email é válido antes de tentar **Atualizar** um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="eccd1-107">Clients can use the API to determine if a display name or mail nickname is valid before trying to **update** an Office 365 group.</span></span> <span data-ttu-id="eccd1-108">Para validar as propriedades antes de criar um grupo, use a [função validateProperties](directoryobject-validateproperties.md) para objetos de diretório.</span><span class="sxs-lookup"><span data-stu-id="eccd1-108">For validating properties before creating a group, use the [validateProperties function](directoryobject-validateproperties.md) for directory objects.</span></span>

<span data-ttu-id="eccd1-109">As validações a seguintes são executadas para as propriedades de apelido de email e o nome de exibição:</span><span class="sxs-lookup"><span data-stu-id="eccd1-109">The following validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="eccd1-110">Validar os prefixos e sufixos de diretiva de nomenclatura</span><span class="sxs-lookup"><span data-stu-id="eccd1-110">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="eccd1-111">Validar a política de palavras proibidos personalizadas</span><span class="sxs-lookup"><span data-stu-id="eccd1-111">Validate the custom banned words policy</span></span>

<span data-ttu-id="eccd1-112">Essa API retorna com a primeira falha encontrada.</span><span class="sxs-lookup"><span data-stu-id="eccd1-112">This API returns with the first failure encountered.</span></span> <span data-ttu-id="eccd1-113">Se uma ou mais propriedades falharem validações vários, apenas a propriedade com a primeira falha de validação será retornada.</span><span class="sxs-lookup"><span data-stu-id="eccd1-113">If one or more properties fail multiple validations, only the property with the first validation failure is returned.</span></span> <span data-ttu-id="eccd1-114">No entanto, você pode validar o apelido de email e o nome para exibição e receber uma coleção de erros de validação, se você estiver validando somente os prefixos e sufixos de diretiva de nomenclatura.</span><span class="sxs-lookup"><span data-stu-id="eccd1-114">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="eccd1-115">Permissions</span><span class="sxs-lookup"><span data-stu-id="eccd1-115">Permissions</span></span>

<span data-ttu-id="eccd1-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eccd1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eccd1-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eccd1-118">Permission type</span></span>      | <span data-ttu-id="eccd1-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eccd1-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eccd1-120">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eccd1-120">Delegated (work or school account)</span></span> | <span data-ttu-id="eccd1-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eccd1-121">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="eccd1-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eccd1-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eccd1-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eccd1-123">Not supported.</span></span>    |
|<span data-ttu-id="eccd1-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eccd1-124">Application</span></span> | <span data-ttu-id="eccd1-125">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eccd1-125">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eccd1-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eccd1-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/<id>/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="eccd1-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eccd1-127">Request headers</span></span>

| <span data-ttu-id="eccd1-128">Nome</span><span class="sxs-lookup"><span data-stu-id="eccd1-128">Name</span></span>           | <span data-ttu-id="eccd1-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="eccd1-129">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="eccd1-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="eccd1-130">Authorization</span></span>  | <span data-ttu-id="eccd1-131">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="eccd1-131">Bearer {code}</span></span>    |
| <span data-ttu-id="eccd1-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eccd1-132">Content-Type</span></span>   | <span data-ttu-id="eccd1-133">application/json</span><span class="sxs-lookup"><span data-stu-id="eccd1-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="eccd1-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eccd1-134">Request body</span></span>

<span data-ttu-id="eccd1-135">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eccd1-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="eccd1-136">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="eccd1-136">Parameter</span></span>    | <span data-ttu-id="eccd1-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="eccd1-137">Type</span></span>   |<span data-ttu-id="eccd1-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="eccd1-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eccd1-139">displayName</span><span class="sxs-lookup"><span data-stu-id="eccd1-139">displayName</span></span>|<span data-ttu-id="eccd1-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eccd1-140">String</span></span>| <span data-ttu-id="eccd1-141">O nome de exibição do grupo para validar.</span><span class="sxs-lookup"><span data-stu-id="eccd1-141">The display name of the group to validate.</span></span> <span data-ttu-id="eccd1-142">A propriedade não é necessária individualmente.</span><span class="sxs-lookup"><span data-stu-id="eccd1-142">The property is not individually required.</span></span> <span data-ttu-id="eccd1-143">No entanto, pelo menos uma propriedade (displayName ou mailNickname) é necessária.</span><span class="sxs-lookup"><span data-stu-id="eccd1-143">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="eccd1-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="eccd1-144">mailNickname</span></span>|<span data-ttu-id="eccd1-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eccd1-145">String</span></span>| <span data-ttu-id="eccd1-146">O apelido de email do grupo para validar.</span><span class="sxs-lookup"><span data-stu-id="eccd1-146">The mail nickname of the group to validate.</span></span> <span data-ttu-id="eccd1-147">A propriedade não é necessária individualmente.</span><span class="sxs-lookup"><span data-stu-id="eccd1-147">The property is not individually required.</span></span> <span data-ttu-id="eccd1-148">No entanto, pelo menos uma propriedade (displayName ou mailNickname) é necessária.</span><span class="sxs-lookup"><span data-stu-id="eccd1-148">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="eccd1-149">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="eccd1-149">onBehalfOfUserId</span></span>|<span data-ttu-id="eccd1-150">Guid</span><span class="sxs-lookup"><span data-stu-id="eccd1-150">Guid</span></span>| <span data-ttu-id="eccd1-151">A ID de objeto do usuário para representar ao chamar a API.</span><span class="sxs-lookup"><span data-stu-id="eccd1-151">The object ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="eccd1-152">Os resultados de validação são para os atributos e funções de onBehalfOfUserId.</span><span class="sxs-lookup"><span data-stu-id="eccd1-152">The validation results are for the onBehalfOfUserId's attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="eccd1-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="eccd1-153">Response</span></span>
<span data-ttu-id="eccd1-154">Se tiver êxito e não houver nenhum erro de validação, o método retornará `204 No Content` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="eccd1-154">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="eccd1-155">Ele não retornará nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eccd1-155">It does not return anything in the response body.</span></span>

<span data-ttu-id="eccd1-156">Se a solicitação for inválida, o método retornará `400 Bad Request` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="eccd1-156">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="eccd1-157">Uma mensagem de erro com detalhes sobre a solicitação inválida é retornada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eccd1-157">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="eccd1-158">Se houver um erro de validação.</span><span class="sxs-lookup"><span data-stu-id="eccd1-158">If there is a validation error.</span></span> <span data-ttu-id="eccd1-159">O método retornará `422 Unprocessable Entity` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="eccd1-159">The method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="eccd1-160">Uma mensagem de erro e uma coleção de detalhes do erro será retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eccd1-160">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eccd1-161">Exemplos</span><span class="sxs-lookup"><span data-stu-id="eccd1-161">Examples</span></span>

<span data-ttu-id="eccd1-162">Este é um exemplo de uma solicitação de validação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="eccd1-162">This is an example of a successful validation request.</span></span>

### <a name="request"></a><span data-ttu-id="eccd1-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eccd1-163">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "group_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json
Content-length: 132

{
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

### <a name="response"></a><span data-ttu-id="eccd1-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="eccd1-164">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="eccd1-165">Este é um exemplo de uma solicitação com erros de validação.</span><span class="sxs-lookup"><span data-stu-id="eccd1-165">This is an example of a request with validation errors.</span></span>

### <a name="request"></a><span data-ttu-id="eccd1-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eccd1-166">Request</span></span>
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

### <a name="response"></a><span data-ttu-id="eccd1-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="eccd1-167">Response</span></span>
```http
HTTP/1.1 422
Content-type: application/json
Content-length: 223

{
  "error": {
    "code": "Request_UnprocessableEntity",
    "message": "The values provided contain one or more validation errors.",
    "innerError": {
      "request-id": "id-value",
      "date": "date-value"
    },
    "details": [
      {
        "target": "mailNickname",
        "code": "PropertyConflict",
        "message": "Another object with the same value for property mailNickname already exists."
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: validateProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
