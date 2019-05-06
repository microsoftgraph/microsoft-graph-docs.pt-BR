---
title: 'Group: ValidateProperties'
description: Validar se o nome de exibição ou o apelido de email de um grupo do Office 365 está em conformidade com as políticas de nomenclatura. Os clientes podem usar a API para determinar se um nome de exibição ou apelido de email é válido antes de tentar **Atualizar** um grupo do Office 365. Para validar as propriedades antes de criar um grupo, use a função ValidateProperties para objetos de diretório.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: d5f5725885e3e37f23c2b31fc6b1ab1d856d99ad
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33592431"
---
# <a name="group-validateproperties"></a><span data-ttu-id="b5260-105">Group: ValidateProperties</span><span class="sxs-lookup"><span data-stu-id="b5260-105">group: validateProperties</span></span>

<span data-ttu-id="b5260-106">Validar se o nome de exibição ou o apelido de email de um grupo do Office 365 está em conformidade com as políticas de nomenclatura.</span><span class="sxs-lookup"><span data-stu-id="b5260-106">Validate if an Office 365 group's display name or mail nickname complies with naming policies.</span></span> <span data-ttu-id="b5260-107">Os clientes podem usar a API para determinar se um nome de exibição ou apelido de email é válido antes de tentar **Atualizar** um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="b5260-107">Clients can use the API to determine if a display name or mail nickname is valid before trying to **update** an Office 365 group.</span></span> <span data-ttu-id="b5260-108">Para validar as propriedades antes de criar um grupo, use a [função ValidateProperties](directoryobject-validateproperties.md) para objetos de diretório.</span><span class="sxs-lookup"><span data-stu-id="b5260-108">For validating properties before creating a group, use the [validateProperties function](directoryobject-validateproperties.md) for directory objects.</span></span>

<span data-ttu-id="b5260-109">As seguintes validações são realizadas para o nome de exibição e as propriedades de apelido de email:</span><span class="sxs-lookup"><span data-stu-id="b5260-109">The following validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="b5260-110">Validar a política de nomenclatura de prefixo e sufixo</span><span class="sxs-lookup"><span data-stu-id="b5260-110">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="b5260-111">Validar a política personalizada de palavras banidas</span><span class="sxs-lookup"><span data-stu-id="b5260-111">Validate the custom banned words policy</span></span>

<span data-ttu-id="b5260-112">Essa API retorna com a primeira falha encontrada.</span><span class="sxs-lookup"><span data-stu-id="b5260-112">This API returns with the first failure encountered.</span></span> <span data-ttu-id="b5260-113">Se uma ou mais propriedades falharem várias validações, somente a propriedade com a primeira falha de validação será retornada.</span><span class="sxs-lookup"><span data-stu-id="b5260-113">If one or more properties fail multiple validations, only the property with the first validation failure is returned.</span></span> <span data-ttu-id="b5260-114">No entanto, você pode validar tanto o apelido de email quanto o nome de exibição e receber uma coleção de erros de validação se você estiver validando apenas o prefixo e a política de nomenclatura de sufixo.</span><span class="sxs-lookup"><span data-stu-id="b5260-114">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5260-115">Permissões</span><span class="sxs-lookup"><span data-stu-id="b5260-115">Permissions</span></span>

<span data-ttu-id="b5260-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5260-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5260-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5260-118">Permission type</span></span>      | <span data-ttu-id="b5260-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b5260-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5260-120">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5260-120">Delegated (work or school account)</span></span> | <span data-ttu-id="b5260-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5260-121">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b5260-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5260-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5260-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5260-123">Not supported.</span></span>    |
|<span data-ttu-id="b5260-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5260-124">Application</span></span> | <span data-ttu-id="b5260-125">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5260-125">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5260-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5260-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/<id>/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="b5260-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5260-127">Request headers</span></span>

| <span data-ttu-id="b5260-128">Nome</span><span class="sxs-lookup"><span data-stu-id="b5260-128">Name</span></span>           | <span data-ttu-id="b5260-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5260-129">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="b5260-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5260-130">Authorization</span></span>  | <span data-ttu-id="b5260-131">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="b5260-131">Bearer {code}</span></span>    |
| <span data-ttu-id="b5260-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b5260-132">Content-Type</span></span>   | <span data-ttu-id="b5260-133">application/json</span><span class="sxs-lookup"><span data-stu-id="b5260-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5260-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5260-134">Request body</span></span>

<span data-ttu-id="b5260-135">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5260-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b5260-136">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b5260-136">Parameter</span></span>    | <span data-ttu-id="b5260-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5260-137">Type</span></span>   |<span data-ttu-id="b5260-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5260-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5260-139">displayName</span><span class="sxs-lookup"><span data-stu-id="b5260-139">displayName</span></span>|<span data-ttu-id="b5260-140">String</span><span class="sxs-lookup"><span data-stu-id="b5260-140">String</span></span>| <span data-ttu-id="b5260-141">O nome de exibição do grupo a ser validado.</span><span class="sxs-lookup"><span data-stu-id="b5260-141">The display name of the group to validate.</span></span> <span data-ttu-id="b5260-142">A propriedade não é necessária individualmente.</span><span class="sxs-lookup"><span data-stu-id="b5260-142">The property is not individually required.</span></span> <span data-ttu-id="b5260-143">No entanto, pelo menos uma propriedade (displayName ou mailNickname) é necessária.</span><span class="sxs-lookup"><span data-stu-id="b5260-143">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="b5260-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="b5260-144">mailNickname</span></span>|<span data-ttu-id="b5260-145">String</span><span class="sxs-lookup"><span data-stu-id="b5260-145">String</span></span>| <span data-ttu-id="b5260-146">O apelido de email do grupo a ser validado.</span><span class="sxs-lookup"><span data-stu-id="b5260-146">The mail nickname of the group to validate.</span></span> <span data-ttu-id="b5260-147">A propriedade não é necessária individualmente.</span><span class="sxs-lookup"><span data-stu-id="b5260-147">The property is not individually required.</span></span> <span data-ttu-id="b5260-148">No entanto, pelo menos uma propriedade (displayName ou mailNickname) é necessária.</span><span class="sxs-lookup"><span data-stu-id="b5260-148">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="b5260-149">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="b5260-149">onBehalfOfUserId</span></span>|<span data-ttu-id="b5260-150">Guid</span><span class="sxs-lookup"><span data-stu-id="b5260-150">Guid</span></span>| <span data-ttu-id="b5260-151">A ID de objeto do usuário a ser representada ao chamar a API.</span><span class="sxs-lookup"><span data-stu-id="b5260-151">The object ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="b5260-152">Os resultados de validação são para os atributos e funções do onBehalfOfUserId.</span><span class="sxs-lookup"><span data-stu-id="b5260-152">The validation results are for the onBehalfOfUserId's attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="b5260-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5260-153">Response</span></span>
<span data-ttu-id="b5260-154">Se tiver êxito e não houver erros de validação, o método `204 No Content` retornará o código de resposta.</span><span class="sxs-lookup"><span data-stu-id="b5260-154">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="b5260-155">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5260-155">It does not return anything in the response body.</span></span>

<span data-ttu-id="b5260-156">Se a solicitação for inválida, o método `400 Bad Request` retornará um código de resposta.</span><span class="sxs-lookup"><span data-stu-id="b5260-156">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="b5260-157">Uma mensagem de erro com detalhes sobre a solicitação inválida é retornada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5260-157">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="b5260-158">Se houver um erro de validação.</span><span class="sxs-lookup"><span data-stu-id="b5260-158">If there is a validation error.</span></span> <span data-ttu-id="b5260-159">O método retorna `422 Unprocessable Entity` um código de resposta.</span><span class="sxs-lookup"><span data-stu-id="b5260-159">The method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="b5260-160">Uma mensagem de erro e um conjunto de detalhes de erro é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5260-160">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b5260-161">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b5260-161">Examples</span></span>

<span data-ttu-id="b5260-162">Este é um exemplo de uma solicitação de validação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="b5260-162">This is an example of a successful validation request.</span></span>

### <a name="request"></a><span data-ttu-id="b5260-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5260-163">Request</span></span>
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

### <a name="response"></a><span data-ttu-id="b5260-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5260-164">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b5260-165">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="b5260-165">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b5260-166">Basic</span><span class="sxs-lookup"><span data-stu-id="b5260-166">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/group_validateproperties-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b5260-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5260-167">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/group_validateproperties-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="b5260-168">Este é um exemplo de uma solicitação com erros de validação.</span><span class="sxs-lookup"><span data-stu-id="b5260-168">This is an example of a request with validation errors.</span></span>

### <a name="request"></a><span data-ttu-id="b5260-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5260-169">Request</span></span>
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

### <a name="response"></a><span data-ttu-id="b5260-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5260-170">Response</span></span>
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
    "Error: /api-reference/beta/api/group-validateproperties.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-validateproperties.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
