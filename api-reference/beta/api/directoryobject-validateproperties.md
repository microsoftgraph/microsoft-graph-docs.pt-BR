---
title: 'directoryobject: ValidateProperties'
description: Validar se o nome de exibição ou o apelido de email de um grupo do Office 365 está em conformidade com as políticas de nomenclatura.  Os clientes podem usar a API para determinar se um nome de exibição ou apelido de email é válido antes de tentar **criar** um grupo do Office 365. Para validar as propriedades de um grupo existente, use a função ValidateProperties para grupos.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a2b72e5c7978ae495f85d207a38801093811d2c3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42434599"
---
# <a name="directoryobject-validateproperties"></a><span data-ttu-id="c54b7-105">directoryobject: ValidateProperties</span><span class="sxs-lookup"><span data-stu-id="c54b7-105">directoryObject: validateProperties</span></span>

<span data-ttu-id="c54b7-106">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c54b7-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c54b7-107">Validar se o nome de exibição ou o apelido de email de um grupo do Office 365 está em conformidade com as políticas de nomenclatura.</span><span class="sxs-lookup"><span data-stu-id="c54b7-107">Validate if an Office 365 group's display name or mail nickname complies with naming policies.</span></span>  <span data-ttu-id="c54b7-108">Os clientes podem usar a API para determinar se um nome de exibição ou apelido de email é válido antes de tentar **criar** um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="c54b7-108">Clients can use the API to determine if a display name or mail nickname is valid before trying to **create** an Office 365 group.</span></span> <span data-ttu-id="c54b7-109">Para validar as propriedades de um grupo existente, use a [função ValidateProperties](group-validateproperties.md) para grupos.</span><span class="sxs-lookup"><span data-stu-id="c54b7-109">For validating properties of an existing group, use the [validateProperties function](group-validateproperties.md) for groups.</span></span>

<span data-ttu-id="c54b7-110">As seguintes validações são realizadas para o nome de exibição e as propriedades de apelido de email:</span><span class="sxs-lookup"><span data-stu-id="c54b7-110">The following validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="c54b7-111">Validar a política de nomenclatura de prefixo e sufixo</span><span class="sxs-lookup"><span data-stu-id="c54b7-111">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="c54b7-112">Validar a política personalizada de palavras banidas</span><span class="sxs-lookup"><span data-stu-id="c54b7-112">Validate the custom banned words policy</span></span>
3. <span data-ttu-id="c54b7-113">Validar o apelido do email é exclusivo</span><span class="sxs-lookup"><span data-stu-id="c54b7-113">Validate the mail nickname is unique</span></span>

<span data-ttu-id="c54b7-114">Essa API retorna com a primeira falha encontrada.</span><span class="sxs-lookup"><span data-stu-id="c54b7-114">This API returns with the first failure encountered.</span></span> <span data-ttu-id="c54b7-115">Se uma ou mais propriedades falharem várias validações, somente a propriedade com a primeira falha de validação será retornada.</span><span class="sxs-lookup"><span data-stu-id="c54b7-115">If one or more properties fail multiple validations, only the property with the first validation failure is returned.</span></span> <span data-ttu-id="c54b7-116">No entanto, você pode validar tanto o apelido de email quanto o nome de exibição e receber uma coleção de erros de validação se você estiver validando apenas o prefixo e a política de nomenclatura de sufixo.</span><span class="sxs-lookup"><span data-stu-id="c54b7-116">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="c54b7-117">Permissões</span><span class="sxs-lookup"><span data-stu-id="c54b7-117">Permissions</span></span>
<span data-ttu-id="c54b7-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c54b7-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c54b7-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c54b7-120">Permission type</span></span>      | <span data-ttu-id="c54b7-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c54b7-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c54b7-122">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c54b7-122">Delegated (work or school account)</span></span> | <span data-ttu-id="c54b7-123">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c54b7-123">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="c54b7-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c54b7-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c54b7-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c54b7-125">Not supported.</span></span>    |
|<span data-ttu-id="c54b7-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c54b7-126">Application</span></span> | <span data-ttu-id="c54b7-127">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c54b7-127">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c54b7-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c54b7-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="c54b7-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c54b7-129">Request headers</span></span>

| <span data-ttu-id="c54b7-130">Nome</span><span class="sxs-lookup"><span data-stu-id="c54b7-130">Name</span></span>           | <span data-ttu-id="c54b7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c54b7-131">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="c54b7-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="c54b7-132">Authorization</span></span>  | <span data-ttu-id="c54b7-133">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="c54b7-133">Bearer {code}</span></span>    |
| <span data-ttu-id="c54b7-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c54b7-134">Content-Type</span></span>   | <span data-ttu-id="c54b7-135">application/json</span><span class="sxs-lookup"><span data-stu-id="c54b7-135">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c54b7-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c54b7-136">Request body</span></span>
<span data-ttu-id="c54b7-137">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c54b7-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c54b7-138">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c54b7-138">Parameter</span></span>    | <span data-ttu-id="c54b7-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="c54b7-139">Type</span></span>   |<span data-ttu-id="c54b7-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="c54b7-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c54b7-141">entityType</span><span class="sxs-lookup"><span data-stu-id="c54b7-141">entityType</span></span>|<span data-ttu-id="c54b7-142">String</span><span class="sxs-lookup"><span data-stu-id="c54b7-142">String</span></span>| <span data-ttu-id="c54b7-143">`Group`é o único tipo de entidade com suporte.</span><span class="sxs-lookup"><span data-stu-id="c54b7-143">`Group` is the only supported entity type.</span></span> |
|<span data-ttu-id="c54b7-144">displayName</span><span class="sxs-lookup"><span data-stu-id="c54b7-144">displayName</span></span>|<span data-ttu-id="c54b7-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c54b7-145">String</span></span>| <span data-ttu-id="c54b7-146">O nome de exibição do grupo a ser validado.</span><span class="sxs-lookup"><span data-stu-id="c54b7-146">The display name of the group to validate.</span></span> <span data-ttu-id="c54b7-147">A propriedade não é necessária individualmente.</span><span class="sxs-lookup"><span data-stu-id="c54b7-147">The property is not individually required.</span></span> <span data-ttu-id="c54b7-148">No entanto, pelo menos uma propriedade (displayName ou mailNickname) é necessária.</span><span class="sxs-lookup"><span data-stu-id="c54b7-148">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="c54b7-149">mailNickname</span><span class="sxs-lookup"><span data-stu-id="c54b7-149">mailNickname</span></span>|<span data-ttu-id="c54b7-150">String</span><span class="sxs-lookup"><span data-stu-id="c54b7-150">String</span></span>| <span data-ttu-id="c54b7-151">O apelido de email do grupo a ser validado.</span><span class="sxs-lookup"><span data-stu-id="c54b7-151">The mail nickname of the group to validate.</span></span> <span data-ttu-id="c54b7-152">A propriedade não é necessária individualmente.</span><span class="sxs-lookup"><span data-stu-id="c54b7-152">The property is not individually required.</span></span> <span data-ttu-id="c54b7-153">No entanto, pelo menos uma propriedade (displayName ou mailNickname) é necessária.</span><span class="sxs-lookup"><span data-stu-id="c54b7-153">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="c54b7-154">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="c54b7-154">onBehalfOfUserId</span></span>|<span data-ttu-id="c54b7-155">Guid</span><span class="sxs-lookup"><span data-stu-id="c54b7-155">Guid</span></span>| <span data-ttu-id="c54b7-156">A ID de objeto do usuário a ser representada ao chamar a API.</span><span class="sxs-lookup"><span data-stu-id="c54b7-156">The object ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="c54b7-157">Os resultados de validação são para os atributos e funções do onBehalfOfUserId.</span><span class="sxs-lookup"><span data-stu-id="c54b7-157">The validation results are for the onBehalfOfUserId's attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="c54b7-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="c54b7-158">Response</span></span>

<span data-ttu-id="c54b7-159">Se tiver êxito e não houver erros de validação, o método `204 No Content` retornará o código de resposta.</span><span class="sxs-lookup"><span data-stu-id="c54b7-159">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="c54b7-160">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c54b7-160">It does not return anything in the response body.</span></span>

<span data-ttu-id="c54b7-161">Se a solicitação for inválida, o método `400 Bad Request` retornará um código de resposta.</span><span class="sxs-lookup"><span data-stu-id="c54b7-161">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="c54b7-162">Uma mensagem de erro com detalhes sobre a solicitação inválida é retornada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c54b7-162">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="c54b7-163">Se houver um erro de validação, o método retornará `422 Unprocessable Entity` um código de resposta.</span><span class="sxs-lookup"><span data-stu-id="c54b7-163">If there is a validation error, the method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="c54b7-164">Uma mensagem de erro e um conjunto de detalhes de erro é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c54b7-164">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c54b7-165">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c54b7-165">Examples</span></span>

<span data-ttu-id="c54b7-166">Este é um exemplo de uma solicitação de validação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="c54b7-166">This is an example of a successful validation request.</span></span>

### <a name="request"></a><span data-ttu-id="c54b7-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c54b7-167">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c54b7-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="c54b7-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/beta/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="c54b7-169">C#</span><span class="sxs-lookup"><span data-stu-id="c54b7-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c54b7-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c54b7-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c54b7-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c54b7-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c54b7-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="c54b7-172">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="c54b7-173">Este é um exemplo de uma solicitação com erros de validação.</span><span class="sxs-lookup"><span data-stu-id="c54b7-173">This is an example of a request with validation errors.</span></span>

### <a name="request"></a><span data-ttu-id="c54b7-174">Solicitar</span><span class="sxs-lookup"><span data-stu-id="c54b7-174">Request</span></span>
```http
POST https://graph.microsoft.com/beta/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "test",
  "mailNickname": "test",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

### <a name="response"></a><span data-ttu-id="c54b7-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="c54b7-175">Response</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
