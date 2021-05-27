---
title: 'group: validateProperties'
description: Valide se Microsoft 365 nome de exibição de um grupo ou apelido de email estiver em conformidade com as políticas de nomenização.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 6f41ee4f9ae52133d3c7611b52b42997480dfc40
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681218"
---
# <a name="group-validateproperties"></a><span data-ttu-id="7aa23-103">group: validateProperties</span><span class="sxs-lookup"><span data-stu-id="7aa23-103">group: validateProperties</span></span>

<span data-ttu-id="7aa23-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7aa23-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7aa23-105">Valide se Microsoft 365 nome de exibição de um grupo ou apelido de email estiver em conformidade com as políticas de nomenização.</span><span class="sxs-lookup"><span data-stu-id="7aa23-105">Validate if a Microsoft 365 group's display name or mail nickname complies with naming policies.</span></span> <span data-ttu-id="7aa23-106">Os clientes podem usar **a** API para determinar se um nome de exibição ou apelido de email é válido antes de tentar atualizar um Microsoft 365 grupo.</span><span class="sxs-lookup"><span data-stu-id="7aa23-106">Clients can use the API to determine if a display name or mail nickname is valid before trying to **update** a Microsoft 365 group.</span></span> <span data-ttu-id="7aa23-107">Para validar propriedades antes de criar um grupo, use a [função validateProperties](directoryobject-validateproperties.md) para objetos de diretório.</span><span class="sxs-lookup"><span data-stu-id="7aa23-107">For validating properties before creating a group, use the [validateProperties function](directoryobject-validateproperties.md) for directory objects.</span></span>

<span data-ttu-id="7aa23-108">As seguintes validações são executadas para as propriedades nome de exibição e apelido de email:</span><span class="sxs-lookup"><span data-stu-id="7aa23-108">The following validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="7aa23-109">Validar a política de nomeação de prefixo e sufixo</span><span class="sxs-lookup"><span data-stu-id="7aa23-109">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="7aa23-110">Validar a política de palavras proibidas personalizada</span><span class="sxs-lookup"><span data-stu-id="7aa23-110">Validate the custom banned words policy</span></span>

<span data-ttu-id="7aa23-111">Essa API retorna com a primeira falha encontrada.</span><span class="sxs-lookup"><span data-stu-id="7aa23-111">This API returns with the first failure encountered.</span></span> <span data-ttu-id="7aa23-112">Se uma ou mais propriedades falharem em várias validações, somente a propriedade com a primeira falha de validação será retornada.</span><span class="sxs-lookup"><span data-stu-id="7aa23-112">If one or more properties fail multiple validations, only the property with the first validation failure is returned.</span></span> <span data-ttu-id="7aa23-113">No entanto, você pode validar o apelido de email e o nome de exibição e receber uma coleção de erros de validação se estiver validando apenas a política de nomenis de prefixo e sufixo.</span><span class="sxs-lookup"><span data-stu-id="7aa23-113">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="7aa23-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="7aa23-114">Permissions</span></span>

<span data-ttu-id="7aa23-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7aa23-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7aa23-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7aa23-117">Permission type</span></span>      | <span data-ttu-id="7aa23-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7aa23-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7aa23-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7aa23-119">Delegated (work or school account)</span></span> | <span data-ttu-id="7aa23-120">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aa23-120">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7aa23-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7aa23-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7aa23-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7aa23-122">Not supported.</span></span>    |
|<span data-ttu-id="7aa23-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7aa23-123">Application</span></span> | <span data-ttu-id="7aa23-124">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aa23-124">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7aa23-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7aa23-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/{id}/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="7aa23-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7aa23-126">Request headers</span></span>

| <span data-ttu-id="7aa23-127">Nome</span><span class="sxs-lookup"><span data-stu-id="7aa23-127">Name</span></span>           | <span data-ttu-id="7aa23-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="7aa23-128">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="7aa23-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="7aa23-129">Authorization</span></span>  | <span data-ttu-id="7aa23-130">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="7aa23-130">Bearer {code}</span></span>    |
| <span data-ttu-id="7aa23-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7aa23-131">Content-Type</span></span>   | <span data-ttu-id="7aa23-132">application/json</span><span class="sxs-lookup"><span data-stu-id="7aa23-132">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7aa23-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7aa23-133">Request body</span></span>

<span data-ttu-id="7aa23-134">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7aa23-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7aa23-135">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7aa23-135">Parameter</span></span>    | <span data-ttu-id="7aa23-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="7aa23-136">Type</span></span>   |<span data-ttu-id="7aa23-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="7aa23-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7aa23-138">displayName</span><span class="sxs-lookup"><span data-stu-id="7aa23-138">displayName</span></span>|<span data-ttu-id="7aa23-139">String</span><span class="sxs-lookup"><span data-stu-id="7aa23-139">String</span></span>| <span data-ttu-id="7aa23-140">O nome de exibição do grupo a ser validado.</span><span class="sxs-lookup"><span data-stu-id="7aa23-140">The display name of the group to validate.</span></span> <span data-ttu-id="7aa23-141">A propriedade não é necessária individualmente.</span><span class="sxs-lookup"><span data-stu-id="7aa23-141">The property is not individually required.</span></span> <span data-ttu-id="7aa23-142">No entanto, pelo menos uma propriedade (displayName ou mailNickname) é necessária.</span><span class="sxs-lookup"><span data-stu-id="7aa23-142">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="7aa23-143">mailNickname</span><span class="sxs-lookup"><span data-stu-id="7aa23-143">mailNickname</span></span>|<span data-ttu-id="7aa23-144">String</span><span class="sxs-lookup"><span data-stu-id="7aa23-144">String</span></span>| <span data-ttu-id="7aa23-145">O apelido de email do grupo a ser validado.</span><span class="sxs-lookup"><span data-stu-id="7aa23-145">The mail nickname of the group to validate.</span></span> <span data-ttu-id="7aa23-146">A propriedade não é necessária individualmente.</span><span class="sxs-lookup"><span data-stu-id="7aa23-146">The property is not individually required.</span></span> <span data-ttu-id="7aa23-147">No entanto, pelo menos uma propriedade (displayName ou mailNickname) é necessária.</span><span class="sxs-lookup"><span data-stu-id="7aa23-147">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="7aa23-148">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="7aa23-148">onBehalfOfUserId</span></span>|<span data-ttu-id="7aa23-149">Guid</span><span class="sxs-lookup"><span data-stu-id="7aa23-149">Guid</span></span>| <span data-ttu-id="7aa23-150">A ID do objeto do usuário a ser personificado ao chamar a API.</span><span class="sxs-lookup"><span data-stu-id="7aa23-150">The object ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="7aa23-151">Os resultados da validação são para os atributos e funções de onBehalfOfUserId.</span><span class="sxs-lookup"><span data-stu-id="7aa23-151">The validation results are for the onBehalfOfUserId's attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="7aa23-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="7aa23-152">Response</span></span>
<span data-ttu-id="7aa23-153">Se tiver êxito e não houver erros de validação, o método retornará `204 No Content` o código de resposta.</span><span class="sxs-lookup"><span data-stu-id="7aa23-153">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="7aa23-154">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7aa23-154">It does not return anything in the response body.</span></span>

<span data-ttu-id="7aa23-155">Se a solicitação for inválida, o método retornará `400 Bad Request` o código de resposta.</span><span class="sxs-lookup"><span data-stu-id="7aa23-155">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="7aa23-156">Uma mensagem de erro com detalhes sobre a solicitação inválida é retornada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7aa23-156">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="7aa23-157">Se houver um erro de validação.</span><span class="sxs-lookup"><span data-stu-id="7aa23-157">If there is a validation error.</span></span> <span data-ttu-id="7aa23-158">O método retorna `422 Unprocessable Entity` o código de resposta.</span><span class="sxs-lookup"><span data-stu-id="7aa23-158">The method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="7aa23-159">Uma mensagem de erro e uma coleção de detalhes de erro é retornada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7aa23-159">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7aa23-160">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7aa23-160">Examples</span></span>

<span data-ttu-id="7aa23-161">Este é um exemplo de uma solicitação de validação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="7aa23-161">This is an example of a successful validation request.</span></span>

### <a name="request"></a><span data-ttu-id="7aa23-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7aa23-162">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7aa23-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="7aa23-163">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7aa23-164">C#</span><span class="sxs-lookup"><span data-stu-id="7aa23-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7aa23-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7aa23-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7aa23-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7aa23-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7aa23-167">Java</span><span class="sxs-lookup"><span data-stu-id="7aa23-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-validateproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7aa23-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="7aa23-168">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="7aa23-169">Este é um exemplo de uma solicitação com erros de validação.</span><span class="sxs-lookup"><span data-stu-id="7aa23-169">This is an example of a request with validation errors.</span></span>

### <a name="request"></a><span data-ttu-id="7aa23-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7aa23-170">Request</span></span>
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

### <a name="response"></a><span data-ttu-id="7aa23-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="7aa23-171">Response</span></span>
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


