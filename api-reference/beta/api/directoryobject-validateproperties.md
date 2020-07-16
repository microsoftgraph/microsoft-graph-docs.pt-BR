---
title: 'directoryobject: ValidateProperties'
description: Validar que o nome de exibição ou o apelido de email de um grupo do Microsoft 365 está em conformidade com as políticas de nomenclatura.
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 45178491bb6ae451cb1ee39a182263a3d99ce59f
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895745"
---
# <a name="directoryobject-validateproperties"></a><span data-ttu-id="17e13-103">directoryobject: ValidateProperties</span><span class="sxs-lookup"><span data-stu-id="17e13-103">directoryObject: validateProperties</span></span>

<span data-ttu-id="17e13-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17e13-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="17e13-105">Validar que o nome de exibição ou o apelido de email de um grupo do Microsoft 365 está em conformidade com as políticas de nomenclatura.</span><span class="sxs-lookup"><span data-stu-id="17e13-105">Validate that a Microsoft 365 group's display name or mail nickname complies with naming policies.</span></span>  <span data-ttu-id="17e13-106">Os clientes podem usar essa API para determinar se um nome de exibição ou apelido de email é válido antes de tentar **criar** um grupo do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="17e13-106">Clients can use this API to determine whether a display name or mail nickname is valid before trying to **create** a Microsoft 365 group.</span></span> <span data-ttu-id="17e13-107">Para validar as propriedades de um grupo existente, use a [função ValidateProperties](group-validateproperties.md) para grupos.</span><span class="sxs-lookup"><span data-stu-id="17e13-107">For validating properties of an existing group, use the [validateProperties function](group-validateproperties.md) for groups.</span></span>

<span data-ttu-id="17e13-108">As seguintes validações são realizadas para o nome de exibição e as propriedades de apelido de email:</span><span class="sxs-lookup"><span data-stu-id="17e13-108">The following validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="17e13-109">Validar a política de nomenclatura de prefixo e sufixo</span><span class="sxs-lookup"><span data-stu-id="17e13-109">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="17e13-110">Validar a política personalizada de palavras banidas</span><span class="sxs-lookup"><span data-stu-id="17e13-110">Validate the custom banned words policy</span></span>
3. <span data-ttu-id="17e13-111">Validar o apelido do email é exclusivo</span><span class="sxs-lookup"><span data-stu-id="17e13-111">Validate the mail nickname is unique</span></span>

<span data-ttu-id="17e13-112">Essa API retorna com a primeira falha encontrada.</span><span class="sxs-lookup"><span data-stu-id="17e13-112">This API returns with the first failure encountered.</span></span> <span data-ttu-id="17e13-113">Se uma ou mais propriedades falharem várias validações, somente a propriedade com a primeira falha de validação será retornada.</span><span class="sxs-lookup"><span data-stu-id="17e13-113">If one or more properties fail multiple validations, only the property with the first validation failure is returned.</span></span> <span data-ttu-id="17e13-114">No entanto, você pode validar tanto o apelido de email quanto o nome de exibição e receber uma coleção de erros de validação se você estiver validando apenas o prefixo e a política de nomenclatura de sufixo.</span><span class="sxs-lookup"><span data-stu-id="17e13-114">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="17e13-115">Permissões</span><span class="sxs-lookup"><span data-stu-id="17e13-115">Permissions</span></span>
<span data-ttu-id="17e13-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17e13-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17e13-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17e13-118">Permission type</span></span>      | <span data-ttu-id="17e13-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="17e13-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17e13-120">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17e13-120">Delegated (work or school account)</span></span> | <span data-ttu-id="17e13-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="17e13-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="17e13-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17e13-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17e13-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17e13-123">Not supported.</span></span>    |
|<span data-ttu-id="17e13-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17e13-124">Application</span></span> | <span data-ttu-id="17e13-125">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17e13-125">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="17e13-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17e13-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="17e13-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17e13-127">Request headers</span></span>

| <span data-ttu-id="17e13-128">Nome</span><span class="sxs-lookup"><span data-stu-id="17e13-128">Name</span></span>           | <span data-ttu-id="17e13-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="17e13-129">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="17e13-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="17e13-130">Authorization</span></span>  | <span data-ttu-id="17e13-131">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="17e13-131">Bearer {code}.</span></span> <span data-ttu-id="17e13-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17e13-132">Required.</span></span>   |
| <span data-ttu-id="17e13-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="17e13-133">Content-Type</span></span>   | <span data-ttu-id="17e13-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17e13-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="17e13-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17e13-136">Request body</span></span>
<span data-ttu-id="17e13-137">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="17e13-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="17e13-138">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="17e13-138">Parameter</span></span>    | <span data-ttu-id="17e13-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="17e13-139">Type</span></span>   |<span data-ttu-id="17e13-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="17e13-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17e13-141">entityType</span><span class="sxs-lookup"><span data-stu-id="17e13-141">entityType</span></span>|<span data-ttu-id="17e13-142">String</span><span class="sxs-lookup"><span data-stu-id="17e13-142">String</span></span>| <span data-ttu-id="17e13-143">`Group`é o único tipo de entidade com suporte.</span><span class="sxs-lookup"><span data-stu-id="17e13-143">`Group` is the only supported entity type.</span></span> |
|<span data-ttu-id="17e13-144">displayName</span><span class="sxs-lookup"><span data-stu-id="17e13-144">displayName</span></span>|<span data-ttu-id="17e13-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17e13-145">String</span></span>| <span data-ttu-id="17e13-146">O nome de exibição do grupo a ser validado.</span><span class="sxs-lookup"><span data-stu-id="17e13-146">The display name of the group to validate.</span></span> <span data-ttu-id="17e13-147">A propriedade não é necessária individualmente.</span><span class="sxs-lookup"><span data-stu-id="17e13-147">The property is not individually required.</span></span> <span data-ttu-id="17e13-148">No entanto, pelo menos uma propriedade (displayName ou mailNickname) é necessária.</span><span class="sxs-lookup"><span data-stu-id="17e13-148">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="17e13-149">mailNickname</span><span class="sxs-lookup"><span data-stu-id="17e13-149">mailNickname</span></span>|<span data-ttu-id="17e13-150">String</span><span class="sxs-lookup"><span data-stu-id="17e13-150">String</span></span>| <span data-ttu-id="17e13-151">O apelido de email do grupo a ser validado.</span><span class="sxs-lookup"><span data-stu-id="17e13-151">The mail nickname of the group to validate.</span></span> <span data-ttu-id="17e13-152">A propriedade não é necessária individualmente.</span><span class="sxs-lookup"><span data-stu-id="17e13-152">The property is not individually required.</span></span> <span data-ttu-id="17e13-153">No entanto, pelo menos uma propriedade (displayName ou mailNickname) é necessária.</span><span class="sxs-lookup"><span data-stu-id="17e13-153">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="17e13-154">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="17e13-154">onBehalfOfUserId</span></span>|<span data-ttu-id="17e13-155">Guid</span><span class="sxs-lookup"><span data-stu-id="17e13-155">Guid</span></span>| <span data-ttu-id="17e13-156">A ID de objeto do usuário a ser representada ao chamar a API.</span><span class="sxs-lookup"><span data-stu-id="17e13-156">The object ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="17e13-157">Os resultados de validação são para os atributos e funções do onBehalfOfUserId.</span><span class="sxs-lookup"><span data-stu-id="17e13-157">The validation results are for the onBehalfOfUserId's attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="17e13-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="17e13-158">Response</span></span>

<span data-ttu-id="17e13-159">Se tiver êxito e não houver erros de validação, o método retornará o `204 No Content` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="17e13-159">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="17e13-160">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17e13-160">It does not return anything in the response body.</span></span>

<span data-ttu-id="17e13-161">Se a solicitação for inválida, o método retornará um `400 Bad Request` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="17e13-161">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="17e13-162">Uma mensagem de erro com detalhes sobre a solicitação inválida é retornada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17e13-162">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="17e13-163">Se houver um erro de validação, o método retornará um `422 Unprocessable Entity` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="17e13-163">If there is a validation error, the method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="17e13-164">Uma mensagem de erro e um conjunto de detalhes de erro é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17e13-164">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="17e13-165">Exemplos</span><span class="sxs-lookup"><span data-stu-id="17e13-165">Examples</span></span>

<span data-ttu-id="17e13-166">Este é um exemplo de uma solicitação de validação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="17e13-166">This is an example of a successful validation request.</span></span>

### <a name="request"></a><span data-ttu-id="17e13-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17e13-167">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="17e13-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="17e13-168">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="17e13-169">C#</span><span class="sxs-lookup"><span data-stu-id="17e13-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="17e13-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17e13-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="17e13-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="17e13-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="17e13-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="17e13-172">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="17e13-173">Este é um exemplo de uma solicitação com erros de validação.</span><span class="sxs-lookup"><span data-stu-id="17e13-173">This is an example of a request with validation errors.</span></span>

### <a name="request"></a><span data-ttu-id="17e13-174">Solicitar</span><span class="sxs-lookup"><span data-stu-id="17e13-174">Request</span></span>
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

### <a name="response"></a><span data-ttu-id="17e13-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="17e13-175">Response</span></span>
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
