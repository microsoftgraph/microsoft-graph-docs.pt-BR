---
title: 'Group: ValidateProperties'
description: Validar se o nome de exibição ou o apelido de email de um grupo do Office 365 está em conformidade com as políticas de nomenclatura. Os clientes podem usar a API para determinar se um nome de exibição ou apelido de email é válido antes de tentar **Atualizar** um grupo do Office 365. Para validar as propriedades antes de criar um grupo, use a função ValidateProperties para objetos de diretório.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f58b8d0dde3f998e093450817be82a38c77594c6
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420515"
---
# <a name="group-validateproperties"></a><span data-ttu-id="b2d94-105">Group: ValidateProperties</span><span class="sxs-lookup"><span data-stu-id="b2d94-105">group: validateProperties</span></span>

<span data-ttu-id="b2d94-106">Validar se o nome de exibição ou o apelido de email de um grupo do Office 365 está em conformidade com as políticas de nomenclatura.</span><span class="sxs-lookup"><span data-stu-id="b2d94-106">Validate if an Office 365 group's display name or mail nickname complies with naming policies.</span></span> <span data-ttu-id="b2d94-107">Os clientes podem usar a API para determinar se um nome de exibição ou apelido de email é válido antes de tentar **Atualizar** um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="b2d94-107">Clients can use the API to determine if a display name or mail nickname is valid before trying to **update** an Office 365 group.</span></span> <span data-ttu-id="b2d94-108">Para validar as propriedades antes de criar um grupo, use a [função ValidateProperties](directoryobject-validateproperties.md) para objetos de diretório.</span><span class="sxs-lookup"><span data-stu-id="b2d94-108">For validating properties before creating a group, use the [validateProperties function](directoryobject-validateproperties.md) for directory objects.</span></span>

<span data-ttu-id="b2d94-109">As seguintes validações são realizadas para o nome de exibição e as propriedades de apelido de email:</span><span class="sxs-lookup"><span data-stu-id="b2d94-109">The following validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="b2d94-110">Validar a política de nomenclatura de prefixo e sufixo</span><span class="sxs-lookup"><span data-stu-id="b2d94-110">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="b2d94-111">Validar a política personalizada de palavras banidas</span><span class="sxs-lookup"><span data-stu-id="b2d94-111">Validate the custom banned words policy</span></span>

<span data-ttu-id="b2d94-112">Essa API retorna com a primeira falha encontrada.</span><span class="sxs-lookup"><span data-stu-id="b2d94-112">This API returns with the first failure encountered.</span></span> <span data-ttu-id="b2d94-113">Se uma ou mais propriedades falharem várias validações, somente a propriedade com a primeira falha de validação será retornada.</span><span class="sxs-lookup"><span data-stu-id="b2d94-113">If one or more properties fail multiple validations, only the property with the first validation failure is returned.</span></span> <span data-ttu-id="b2d94-114">No entanto, você pode validar tanto o apelido de email quanto o nome de exibição e receber uma coleção de erros de validação se você estiver validando apenas o prefixo e a política de nomenclatura de sufixo.</span><span class="sxs-lookup"><span data-stu-id="b2d94-114">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2d94-115">Permissões</span><span class="sxs-lookup"><span data-stu-id="b2d94-115">Permissions</span></span>

<span data-ttu-id="b2d94-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2d94-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2d94-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2d94-118">Permission type</span></span>      | <span data-ttu-id="b2d94-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b2d94-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2d94-120">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2d94-120">Delegated (work or school account)</span></span> | <span data-ttu-id="b2d94-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2d94-121">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b2d94-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2d94-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2d94-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2d94-123">Not supported.</span></span>    |
|<span data-ttu-id="b2d94-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2d94-124">Application</span></span> | <span data-ttu-id="b2d94-125">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2d94-125">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2d94-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2d94-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/{id}/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="b2d94-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2d94-127">Request headers</span></span>

| <span data-ttu-id="b2d94-128">Nome</span><span class="sxs-lookup"><span data-stu-id="b2d94-128">Name</span></span>           | <span data-ttu-id="b2d94-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2d94-129">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="b2d94-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2d94-130">Authorization</span></span>  | <span data-ttu-id="b2d94-131">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="b2d94-131">Bearer {code}</span></span>    |
| <span data-ttu-id="b2d94-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b2d94-132">Content-Type</span></span>   | <span data-ttu-id="b2d94-133">application/json</span><span class="sxs-lookup"><span data-stu-id="b2d94-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b2d94-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2d94-134">Request body</span></span>

<span data-ttu-id="b2d94-135">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2d94-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b2d94-136">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b2d94-136">Parameter</span></span>    | <span data-ttu-id="b2d94-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2d94-137">Type</span></span>   |<span data-ttu-id="b2d94-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2d94-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2d94-139">displayName</span><span class="sxs-lookup"><span data-stu-id="b2d94-139">displayName</span></span>|<span data-ttu-id="b2d94-140">String</span><span class="sxs-lookup"><span data-stu-id="b2d94-140">String</span></span>| <span data-ttu-id="b2d94-141">O nome de exibição do grupo a ser validado.</span><span class="sxs-lookup"><span data-stu-id="b2d94-141">The display name of the group to validate.</span></span> <span data-ttu-id="b2d94-142">A propriedade não é necessária individualmente.</span><span class="sxs-lookup"><span data-stu-id="b2d94-142">The property is not individually required.</span></span> <span data-ttu-id="b2d94-143">No entanto, pelo menos uma propriedade (displayName ou mailNickname) é necessária.</span><span class="sxs-lookup"><span data-stu-id="b2d94-143">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="b2d94-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="b2d94-144">mailNickname</span></span>|<span data-ttu-id="b2d94-145">String</span><span class="sxs-lookup"><span data-stu-id="b2d94-145">String</span></span>| <span data-ttu-id="b2d94-146">O apelido de email do grupo a ser validado.</span><span class="sxs-lookup"><span data-stu-id="b2d94-146">The mail nickname of the group to validate.</span></span> <span data-ttu-id="b2d94-147">A propriedade não é necessária individualmente.</span><span class="sxs-lookup"><span data-stu-id="b2d94-147">The property is not individually required.</span></span> <span data-ttu-id="b2d94-148">No entanto, pelo menos uma propriedade (displayName ou mailNickname) é necessária.</span><span class="sxs-lookup"><span data-stu-id="b2d94-148">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="b2d94-149">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="b2d94-149">onBehalfOfUserId</span></span>|<span data-ttu-id="b2d94-150">Guid</span><span class="sxs-lookup"><span data-stu-id="b2d94-150">Guid</span></span>| <span data-ttu-id="b2d94-151">A ID de objeto do usuário a ser representada ao chamar a API.</span><span class="sxs-lookup"><span data-stu-id="b2d94-151">The object ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="b2d94-152">Os resultados de validação são para os atributos e funções do onBehalfOfUserId.</span><span class="sxs-lookup"><span data-stu-id="b2d94-152">The validation results are for the onBehalfOfUserId's attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="b2d94-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2d94-153">Response</span></span>
<span data-ttu-id="b2d94-154">Se tiver êxito e não houver erros de validação, o método `204 No Content` retornará o código de resposta.</span><span class="sxs-lookup"><span data-stu-id="b2d94-154">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="b2d94-155">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2d94-155">It does not return anything in the response body.</span></span>

<span data-ttu-id="b2d94-156">Se a solicitação for inválida, o método `400 Bad Request` retornará um código de resposta.</span><span class="sxs-lookup"><span data-stu-id="b2d94-156">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="b2d94-157">Uma mensagem de erro com detalhes sobre a solicitação inválida é retornada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2d94-157">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="b2d94-158">Se houver um erro de validação.</span><span class="sxs-lookup"><span data-stu-id="b2d94-158">If there is a validation error.</span></span> <span data-ttu-id="b2d94-159">O método retorna `422 Unprocessable Entity` um código de resposta.</span><span class="sxs-lookup"><span data-stu-id="b2d94-159">The method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="b2d94-160">Uma mensagem de erro e um conjunto de detalhes de erro é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2d94-160">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b2d94-161">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b2d94-161">Examples</span></span>

<span data-ttu-id="b2d94-162">Este é um exemplo de uma solicitação de validação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="b2d94-162">This is an example of a successful validation request.</span></span>

### <a name="request"></a><span data-ttu-id="b2d94-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2d94-163">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b2d94-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2d94-164">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b2d94-165">C#</span><span class="sxs-lookup"><span data-stu-id="b2d94-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b2d94-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2d94-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b2d94-167">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b2d94-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b2d94-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2d94-168">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="b2d94-169">Este é um exemplo de uma solicitação com erros de validação.</span><span class="sxs-lookup"><span data-stu-id="b2d94-169">This is an example of a request with validation errors.</span></span>

### <a name="request"></a><span data-ttu-id="b2d94-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2d94-170">Request</span></span>
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

### <a name="response"></a><span data-ttu-id="b2d94-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2d94-171">Response</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
