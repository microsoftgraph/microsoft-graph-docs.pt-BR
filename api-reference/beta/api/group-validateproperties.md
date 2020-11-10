---
title: 'Group: ValidateProperties'
description: Validar se o nome de exibição ou o apelido de email de um grupo do Microsoft 365 está em conformidade com as políticas de nomenclatura.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 08089b1a3f0737f854e21cd9d72b06f684f48bdd
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953653"
---
# <a name="group-validateproperties"></a><span data-ttu-id="bba5d-103">Group: ValidateProperties</span><span class="sxs-lookup"><span data-stu-id="bba5d-103">group: validateProperties</span></span>

<span data-ttu-id="bba5d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bba5d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bba5d-105">Validar se o nome de exibição ou o apelido de email de um grupo do Microsoft 365 está em conformidade com as políticas de nomenclatura.</span><span class="sxs-lookup"><span data-stu-id="bba5d-105">Validate if a Microsoft 365 group's display name or mail nickname complies with naming policies.</span></span> <span data-ttu-id="bba5d-106">Os clientes podem usar a API para determinar se um nome de exibição ou apelido de email é válido antes de tentar **Atualizar** um grupo do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="bba5d-106">Clients can use the API to determine if a display name or mail nickname is valid before trying to **update** a Microsoft 365 group.</span></span> <span data-ttu-id="bba5d-107">Para validar as propriedades antes de criar um grupo, use a [função ValidateProperties](directoryobject-validateproperties.md) para objetos de diretório.</span><span class="sxs-lookup"><span data-stu-id="bba5d-107">For validating properties before creating a group, use the [validateProperties function](directoryobject-validateproperties.md) for directory objects.</span></span>

<span data-ttu-id="bba5d-108">As seguintes validações são realizadas para o nome de exibição e as propriedades de apelido de email:</span><span class="sxs-lookup"><span data-stu-id="bba5d-108">The following validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="bba5d-109">Validar a política de nomenclatura de prefixo e sufixo</span><span class="sxs-lookup"><span data-stu-id="bba5d-109">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="bba5d-110">Validar a política personalizada de palavras banidas</span><span class="sxs-lookup"><span data-stu-id="bba5d-110">Validate the custom banned words policy</span></span>

<span data-ttu-id="bba5d-111">Essa API retorna com a primeira falha encontrada.</span><span class="sxs-lookup"><span data-stu-id="bba5d-111">This API returns with the first failure encountered.</span></span> <span data-ttu-id="bba5d-112">Se uma ou mais propriedades falharem várias validações, somente a propriedade com a primeira falha de validação será retornada.</span><span class="sxs-lookup"><span data-stu-id="bba5d-112">If one or more properties fail multiple validations, only the property with the first validation failure is returned.</span></span> <span data-ttu-id="bba5d-113">No entanto, você pode validar tanto o apelido de email quanto o nome de exibição e receber uma coleção de erros de validação se você estiver validando apenas o prefixo e a política de nomenclatura de sufixo.</span><span class="sxs-lookup"><span data-stu-id="bba5d-113">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="bba5d-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="bba5d-114">Permissions</span></span>

<span data-ttu-id="bba5d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bba5d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bba5d-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bba5d-117">Permission type</span></span>      | <span data-ttu-id="bba5d-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bba5d-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bba5d-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bba5d-119">Delegated (work or school account)</span></span> | <span data-ttu-id="bba5d-120">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bba5d-120">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bba5d-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bba5d-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bba5d-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bba5d-122">Not supported.</span></span>    |
|<span data-ttu-id="bba5d-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bba5d-123">Application</span></span> | <span data-ttu-id="bba5d-124">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bba5d-124">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bba5d-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bba5d-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/{id}/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="bba5d-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bba5d-126">Request headers</span></span>

| <span data-ttu-id="bba5d-127">Nome</span><span class="sxs-lookup"><span data-stu-id="bba5d-127">Name</span></span>           | <span data-ttu-id="bba5d-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="bba5d-128">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="bba5d-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="bba5d-129">Authorization</span></span>  | <span data-ttu-id="bba5d-130">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="bba5d-130">Bearer {code}</span></span>    |
| <span data-ttu-id="bba5d-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bba5d-131">Content-Type</span></span>   | <span data-ttu-id="bba5d-132">application/json</span><span class="sxs-lookup"><span data-stu-id="bba5d-132">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="bba5d-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bba5d-133">Request body</span></span>

<span data-ttu-id="bba5d-134">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bba5d-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bba5d-135">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bba5d-135">Parameter</span></span>    | <span data-ttu-id="bba5d-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="bba5d-136">Type</span></span>   |<span data-ttu-id="bba5d-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="bba5d-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bba5d-138">displayName</span><span class="sxs-lookup"><span data-stu-id="bba5d-138">displayName</span></span>|<span data-ttu-id="bba5d-139">String</span><span class="sxs-lookup"><span data-stu-id="bba5d-139">String</span></span>| <span data-ttu-id="bba5d-140">O nome de exibição do grupo a ser validado.</span><span class="sxs-lookup"><span data-stu-id="bba5d-140">The display name of the group to validate.</span></span> <span data-ttu-id="bba5d-141">A propriedade não é necessária individualmente.</span><span class="sxs-lookup"><span data-stu-id="bba5d-141">The property is not individually required.</span></span> <span data-ttu-id="bba5d-142">No entanto, pelo menos uma propriedade (displayName ou mailNickname) é necessária.</span><span class="sxs-lookup"><span data-stu-id="bba5d-142">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="bba5d-143">mailNickname</span><span class="sxs-lookup"><span data-stu-id="bba5d-143">mailNickname</span></span>|<span data-ttu-id="bba5d-144">String</span><span class="sxs-lookup"><span data-stu-id="bba5d-144">String</span></span>| <span data-ttu-id="bba5d-145">O apelido de email do grupo a ser validado.</span><span class="sxs-lookup"><span data-stu-id="bba5d-145">The mail nickname of the group to validate.</span></span> <span data-ttu-id="bba5d-146">A propriedade não é necessária individualmente.</span><span class="sxs-lookup"><span data-stu-id="bba5d-146">The property is not individually required.</span></span> <span data-ttu-id="bba5d-147">No entanto, pelo menos uma propriedade (displayName ou mailNickname) é necessária.</span><span class="sxs-lookup"><span data-stu-id="bba5d-147">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="bba5d-148">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="bba5d-148">onBehalfOfUserId</span></span>|<span data-ttu-id="bba5d-149">Guid</span><span class="sxs-lookup"><span data-stu-id="bba5d-149">Guid</span></span>| <span data-ttu-id="bba5d-150">A ID de objeto do usuário a ser representada ao chamar a API.</span><span class="sxs-lookup"><span data-stu-id="bba5d-150">The object ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="bba5d-151">Os resultados de validação são para os atributos e funções do onBehalfOfUserId.</span><span class="sxs-lookup"><span data-stu-id="bba5d-151">The validation results are for the onBehalfOfUserId's attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="bba5d-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="bba5d-152">Response</span></span>
<span data-ttu-id="bba5d-153">Se tiver êxito e não houver erros de validação, o método retornará o `204 No Content` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="bba5d-153">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="bba5d-154">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bba5d-154">It does not return anything in the response body.</span></span>

<span data-ttu-id="bba5d-155">Se a solicitação for inválida, o método retornará um `400 Bad Request` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="bba5d-155">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="bba5d-156">Uma mensagem de erro com detalhes sobre a solicitação inválida é retornada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bba5d-156">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="bba5d-157">Se houver um erro de validação.</span><span class="sxs-lookup"><span data-stu-id="bba5d-157">If there is a validation error.</span></span> <span data-ttu-id="bba5d-158">O método retorna um `422 Unprocessable Entity` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="bba5d-158">The method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="bba5d-159">Uma mensagem de erro e um conjunto de detalhes de erro é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bba5d-159">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bba5d-160">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bba5d-160">Examples</span></span>

<span data-ttu-id="bba5d-161">Este é um exemplo de uma solicitação de validação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="bba5d-161">This is an example of a successful validation request.</span></span>

### <a name="request"></a><span data-ttu-id="bba5d-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bba5d-162">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="bba5d-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="bba5d-163">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="bba5d-164">C#</span><span class="sxs-lookup"><span data-stu-id="bba5d-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bba5d-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bba5d-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bba5d-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bba5d-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bba5d-167">Java</span><span class="sxs-lookup"><span data-stu-id="bba5d-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-validateproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bba5d-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="bba5d-168">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="bba5d-169">Este é um exemplo de uma solicitação com erros de validação.</span><span class="sxs-lookup"><span data-stu-id="bba5d-169">This is an example of a request with validation errors.</span></span>

### <a name="request"></a><span data-ttu-id="bba5d-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bba5d-170">Request</span></span>
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

### <a name="response"></a><span data-ttu-id="bba5d-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="bba5d-171">Response</span></span>
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


