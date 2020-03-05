---
title: 'Group: ValidateProperties'
description: Validar se o nome de exibição ou o apelido de email de um grupo do Office 365 está em conformidade com as políticas de nomenclatura. Os clientes podem usar a API para determinar se um nome de exibição ou apelido de email é válido antes de tentar **Atualizar** um grupo do Office 365. Para validar as propriedades antes de criar um grupo, use a função ValidateProperties para objetos de diretório.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: cb0d6ca17a7c6bb9d48919235dfc8c3a9cec1059
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446671"
---
# <a name="group-validateproperties"></a><span data-ttu-id="02024-105">Group: ValidateProperties</span><span class="sxs-lookup"><span data-stu-id="02024-105">group: validateProperties</span></span>

<span data-ttu-id="02024-106">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="02024-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="02024-107">Validar se o nome de exibição ou o apelido de email de um grupo do Office 365 está em conformidade com as políticas de nomenclatura.</span><span class="sxs-lookup"><span data-stu-id="02024-107">Validate if an Office 365 group's display name or mail nickname complies with naming policies.</span></span> <span data-ttu-id="02024-108">Os clientes podem usar a API para determinar se um nome de exibição ou apelido de email é válido antes de tentar **Atualizar** um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="02024-108">Clients can use the API to determine if a display name or mail nickname is valid before trying to **update** an Office 365 group.</span></span> <span data-ttu-id="02024-109">Para validar as propriedades antes de criar um grupo, use a [função ValidateProperties](directoryobject-validateproperties.md) para objetos de diretório.</span><span class="sxs-lookup"><span data-stu-id="02024-109">For validating properties before creating a group, use the [validateProperties function](directoryobject-validateproperties.md) for directory objects.</span></span>

<span data-ttu-id="02024-110">As seguintes validações são realizadas para o nome de exibição e as propriedades de apelido de email:</span><span class="sxs-lookup"><span data-stu-id="02024-110">The following validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="02024-111">Validar a política de nomenclatura de prefixo e sufixo</span><span class="sxs-lookup"><span data-stu-id="02024-111">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="02024-112">Validar a política personalizada de palavras banidas</span><span class="sxs-lookup"><span data-stu-id="02024-112">Validate the custom banned words policy</span></span>

<span data-ttu-id="02024-113">Essa API retorna com a primeira falha encontrada.</span><span class="sxs-lookup"><span data-stu-id="02024-113">This API returns with the first failure encountered.</span></span> <span data-ttu-id="02024-114">Se uma ou mais propriedades falharem várias validações, somente a propriedade com a primeira falha de validação será retornada.</span><span class="sxs-lookup"><span data-stu-id="02024-114">If one or more properties fail multiple validations, only the property with the first validation failure is returned.</span></span> <span data-ttu-id="02024-115">No entanto, você pode validar tanto o apelido de email quanto o nome de exibição e receber uma coleção de erros de validação se você estiver validando apenas o prefixo e a política de nomenclatura de sufixo.</span><span class="sxs-lookup"><span data-stu-id="02024-115">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="02024-116">Permissões</span><span class="sxs-lookup"><span data-stu-id="02024-116">Permissions</span></span>

<span data-ttu-id="02024-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02024-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02024-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02024-119">Permission type</span></span>      | <span data-ttu-id="02024-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02024-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02024-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02024-121">Delegated (work or school account)</span></span> | <span data-ttu-id="02024-122">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02024-122">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="02024-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02024-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02024-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02024-124">Not supported.</span></span>    |
|<span data-ttu-id="02024-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02024-125">Application</span></span> | <span data-ttu-id="02024-126">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02024-126">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="02024-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02024-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/{id}/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="02024-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02024-128">Request headers</span></span>

| <span data-ttu-id="02024-129">Nome</span><span class="sxs-lookup"><span data-stu-id="02024-129">Name</span></span>           | <span data-ttu-id="02024-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="02024-130">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="02024-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="02024-131">Authorization</span></span>  | <span data-ttu-id="02024-132">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="02024-132">Bearer {code}</span></span>    |
| <span data-ttu-id="02024-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="02024-133">Content-Type</span></span>   | <span data-ttu-id="02024-134">application/json</span><span class="sxs-lookup"><span data-stu-id="02024-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="02024-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02024-135">Request body</span></span>

<span data-ttu-id="02024-136">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02024-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="02024-137">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="02024-137">Parameter</span></span>    | <span data-ttu-id="02024-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="02024-138">Type</span></span>   |<span data-ttu-id="02024-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="02024-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02024-140">displayName</span><span class="sxs-lookup"><span data-stu-id="02024-140">displayName</span></span>|<span data-ttu-id="02024-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02024-141">String</span></span>| <span data-ttu-id="02024-142">O nome de exibição do grupo a ser validado.</span><span class="sxs-lookup"><span data-stu-id="02024-142">The display name of the group to validate.</span></span> <span data-ttu-id="02024-143">A propriedade não é necessária individualmente.</span><span class="sxs-lookup"><span data-stu-id="02024-143">The property is not individually required.</span></span> <span data-ttu-id="02024-144">No entanto, pelo menos uma propriedade (displayName ou mailNickname) é necessária.</span><span class="sxs-lookup"><span data-stu-id="02024-144">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="02024-145">mailNickname</span><span class="sxs-lookup"><span data-stu-id="02024-145">mailNickname</span></span>|<span data-ttu-id="02024-146">String</span><span class="sxs-lookup"><span data-stu-id="02024-146">String</span></span>| <span data-ttu-id="02024-147">O apelido de email do grupo a ser validado.</span><span class="sxs-lookup"><span data-stu-id="02024-147">The mail nickname of the group to validate.</span></span> <span data-ttu-id="02024-148">A propriedade não é necessária individualmente.</span><span class="sxs-lookup"><span data-stu-id="02024-148">The property is not individually required.</span></span> <span data-ttu-id="02024-149">No entanto, pelo menos uma propriedade (displayName ou mailNickname) é necessária.</span><span class="sxs-lookup"><span data-stu-id="02024-149">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="02024-150">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="02024-150">onBehalfOfUserId</span></span>|<span data-ttu-id="02024-151">Guid</span><span class="sxs-lookup"><span data-stu-id="02024-151">Guid</span></span>| <span data-ttu-id="02024-152">A ID de objeto do usuário a ser representada ao chamar a API.</span><span class="sxs-lookup"><span data-stu-id="02024-152">The object ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="02024-153">Os resultados de validação são para os atributos e funções do onBehalfOfUserId.</span><span class="sxs-lookup"><span data-stu-id="02024-153">The validation results are for the onBehalfOfUserId's attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="02024-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="02024-154">Response</span></span>
<span data-ttu-id="02024-155">Se tiver êxito e não houver erros de validação, o método `204 No Content` retornará o código de resposta.</span><span class="sxs-lookup"><span data-stu-id="02024-155">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="02024-156">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02024-156">It does not return anything in the response body.</span></span>

<span data-ttu-id="02024-157">Se a solicitação for inválida, o método `400 Bad Request` retornará um código de resposta.</span><span class="sxs-lookup"><span data-stu-id="02024-157">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="02024-158">Uma mensagem de erro com detalhes sobre a solicitação inválida é retornada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02024-158">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="02024-159">Se houver um erro de validação.</span><span class="sxs-lookup"><span data-stu-id="02024-159">If there is a validation error.</span></span> <span data-ttu-id="02024-160">O método retorna `422 Unprocessable Entity` um código de resposta.</span><span class="sxs-lookup"><span data-stu-id="02024-160">The method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="02024-161">Uma mensagem de erro e um conjunto de detalhes de erro é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02024-161">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="02024-162">Exemplos</span><span class="sxs-lookup"><span data-stu-id="02024-162">Examples</span></span>

<span data-ttu-id="02024-163">Este é um exemplo de uma solicitação de validação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="02024-163">This is an example of a successful validation request.</span></span>

### <a name="request"></a><span data-ttu-id="02024-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02024-164">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="02024-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="02024-165">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="02024-166">C#</span><span class="sxs-lookup"><span data-stu-id="02024-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02024-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02024-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02024-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02024-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="02024-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="02024-169">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="02024-170">Este é um exemplo de uma solicitação com erros de validação.</span><span class="sxs-lookup"><span data-stu-id="02024-170">This is an example of a request with validation errors.</span></span>

### <a name="request"></a><span data-ttu-id="02024-171">Solicitar</span><span class="sxs-lookup"><span data-stu-id="02024-171">Request</span></span>
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

### <a name="response"></a><span data-ttu-id="02024-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="02024-172">Response</span></span>
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
