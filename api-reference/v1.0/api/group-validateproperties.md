---
title: 'Group: ValidateProperties'
description: Valide se o nome de exibição ou o apelido de email de um grupo do Office 365 está em conformidade com as políticas de nomenclatura.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e2699e50012f92d8a776fcce20c5cd3d87be83d6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373301"
---
# <a name="group-validateproperties"></a><span data-ttu-id="ddb01-103">Group: ValidateProperties</span><span class="sxs-lookup"><span data-stu-id="ddb01-103">group: validateProperties</span></span>

<span data-ttu-id="ddb01-104">Valide se o nome de exibição ou o apelido de email de um grupo do Office 365 está em conformidade com as políticas de nomenclatura.</span><span class="sxs-lookup"><span data-stu-id="ddb01-104">Validate that an Office 365 group's display name or mail nickname complies with naming policies.</span></span>  <span data-ttu-id="ddb01-105">Os clientes podem usar essa API para determinar se um nome de exibição ou apelido de email é válido antes de tentar [Atualizar](group-update.md) um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="ddb01-105">Clients can use this API to determine whether a display name or mail nickname is valid before trying to [update](group-update.md) an Office 365 group.</span></span> <span data-ttu-id="ddb01-106">Para validar as propriedades antes de criar um grupo, use a função [directoryobject: ValidateProperties](directoryobject-validateproperties.md) .</span><span class="sxs-lookup"><span data-stu-id="ddb01-106">To validate the properties before creating a group, use the [directoryobject:validateProperties](directoryobject-validateproperties.md) function.</span></span>

<span data-ttu-id="ddb01-107">As seguintes validações de política são realizadas para o nome de exibição e as propriedades de apelido de email:</span><span class="sxs-lookup"><span data-stu-id="ddb01-107">The following policy validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="ddb01-108">Validar a política de nomenclatura de prefixo e sufixo</span><span class="sxs-lookup"><span data-stu-id="ddb01-108">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="ddb01-109">Validar a política personalizada de palavras banidas</span><span class="sxs-lookup"><span data-stu-id="ddb01-109">Validate the custom banned words policy</span></span>

<span data-ttu-id="ddb01-110">Essa API só retorna a primeira falha de validação encontrada.</span><span class="sxs-lookup"><span data-stu-id="ddb01-110">This API only returns the first validation failure that is encountered.</span></span> <span data-ttu-id="ddb01-111">Se as propriedades falharem várias validações, somente a primeira falha de validação será retornada.</span><span class="sxs-lookup"><span data-stu-id="ddb01-111">If the properties fail multiple validations, only the first validation failure is returned.</span></span> <span data-ttu-id="ddb01-112">No entanto, você pode validar tanto o apelido de email quanto o nome de exibição e receber uma coleção de erros de validação se você estiver validando apenas o prefixo e a política de nomenclatura de sufixo.</span><span class="sxs-lookup"><span data-stu-id="ddb01-112">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span> <span data-ttu-id="ddb01-113">Para saber mais sobre como configurar políticas de nomenclatura, consulte [Configure Naming Policy](https://docs.microsoft.com/en-us/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell).</span><span class="sxs-lookup"><span data-stu-id="ddb01-113">To learn more about configuring naming policies, see [Configure naming policy](https://docs.microsoft.com/en-us/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell).</span></span>

## <a name="permissions"></a><span data-ttu-id="ddb01-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="ddb01-114">Permissions</span></span>

<span data-ttu-id="ddb01-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddb01-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddb01-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ddb01-117">Permission type</span></span>      | <span data-ttu-id="ddb01-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ddb01-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ddb01-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ddb01-119">Delegated (work or school account)</span></span> | <span data-ttu-id="ddb01-120">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddb01-120">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ddb01-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ddb01-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddb01-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ddb01-122">Not supported.</span></span>    |
|<span data-ttu-id="ddb01-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddb01-123">Application</span></span> | <span data-ttu-id="ddb01-124">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddb01-124">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ddb01-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ddb01-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/{id}/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="ddb01-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ddb01-126">Request headers</span></span>

| <span data-ttu-id="ddb01-127">Nome</span><span class="sxs-lookup"><span data-stu-id="ddb01-127">Name</span></span>           | <span data-ttu-id="ddb01-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddb01-128">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="ddb01-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="ddb01-129">Authorization</span></span>  | <span data-ttu-id="ddb01-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ddb01-p104">Bearer {token}. Required.</span></span>    |
| <span data-ttu-id="ddb01-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ddb01-132">Content-Type</span></span>   | <span data-ttu-id="ddb01-133">application/json</span><span class="sxs-lookup"><span data-stu-id="ddb01-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ddb01-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ddb01-134">Request body</span></span>

<span data-ttu-id="ddb01-135">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddb01-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ddb01-136">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ddb01-136">Parameter</span></span>    | <span data-ttu-id="ddb01-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="ddb01-137">Type</span></span>   |<span data-ttu-id="ddb01-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddb01-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ddb01-139">displayName</span><span class="sxs-lookup"><span data-stu-id="ddb01-139">displayName</span></span>|<span data-ttu-id="ddb01-140">String</span><span class="sxs-lookup"><span data-stu-id="ddb01-140">String</span></span>| <span data-ttu-id="ddb01-141">O nome de exibição do grupo a ser validado.</span><span class="sxs-lookup"><span data-stu-id="ddb01-141">The display name of the group to validate.</span></span> <span data-ttu-id="ddb01-142">A propriedade não é necessária individualmente.</span><span class="sxs-lookup"><span data-stu-id="ddb01-142">The property is not individually required.</span></span> <span data-ttu-id="ddb01-143">No entanto, pelo menos uma propriedade (**DisplayName** ou **mailNickname**) é necessária.</span><span class="sxs-lookup"><span data-stu-id="ddb01-143">However, at least one property (**displayName** or **mailNickname**) is required.</span></span> |
|<span data-ttu-id="ddb01-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="ddb01-144">mailNickname</span></span>|<span data-ttu-id="ddb01-145">String</span><span class="sxs-lookup"><span data-stu-id="ddb01-145">String</span></span>| <span data-ttu-id="ddb01-146">O apelido de email do grupo a ser validado.</span><span class="sxs-lookup"><span data-stu-id="ddb01-146">The mail nickname of the group to validate.</span></span> <span data-ttu-id="ddb01-147">A propriedade não é necessária individualmente.</span><span class="sxs-lookup"><span data-stu-id="ddb01-147">The property is not individually required.</span></span> <span data-ttu-id="ddb01-148">No entanto, pelo menos uma propriedade (**DisplayName** ou **mailNickname**) é necessária.</span><span class="sxs-lookup"><span data-stu-id="ddb01-148">However, at least one property (**displayName** or **mailNickname**) is required.</span></span> |
|<span data-ttu-id="ddb01-149">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="ddb01-149">onBehalfOfUserId</span></span>|<span data-ttu-id="ddb01-150">Guid</span><span class="sxs-lookup"><span data-stu-id="ddb01-150">Guid</span></span>| <span data-ttu-id="ddb01-151">A ID do usuário a ser personificada ao chamar a API.</span><span class="sxs-lookup"><span data-stu-id="ddb01-151">The ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="ddb01-152">Os resultados de validação são para os atributos e funções **do onBehalfOfUserId** .</span><span class="sxs-lookup"><span data-stu-id="ddb01-152">The validation results are for the **onBehalfOfUserId's** attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="ddb01-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddb01-153">Response</span></span>
<span data-ttu-id="ddb01-154">Se tiver êxito e não houver erros de validação, o método `204 No Content` retornará o código de resposta.</span><span class="sxs-lookup"><span data-stu-id="ddb01-154">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="ddb01-155">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ddb01-155">It does not return anything in the response body.</span></span>

<span data-ttu-id="ddb01-156">Se a solicitação for inválida, o método `400 Bad Request` retornará um código de resposta.</span><span class="sxs-lookup"><span data-stu-id="ddb01-156">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="ddb01-157">Uma mensagem de erro com detalhes sobre a solicitação inválida é retornada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ddb01-157">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="ddb01-158">Se houver um erro de validação.</span><span class="sxs-lookup"><span data-stu-id="ddb01-158">If there is a validation error.</span></span> <span data-ttu-id="ddb01-159">O método retorna `422 Unprocessable Entity` um código de resposta.</span><span class="sxs-lookup"><span data-stu-id="ddb01-159">The method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="ddb01-160">Uma mensagem de erro e um conjunto de detalhes de erro é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ddb01-160">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ddb01-161">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ddb01-161">Examples</span></span>

### <a name="example-1-successful-validation-request"></a><span data-ttu-id="ddb01-162">Exemplo 1: solicitação de validação bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="ddb01-162">Example 1: Successful validation request</span></span>
<span data-ttu-id="ddb01-163">Este é um exemplo de uma solicitação de validação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="ddb01-163">This is an example of a successful validation request.</span></span>

#### <a name="request"></a><span data-ttu-id="ddb01-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddb01-164">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ddb01-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="ddb01-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/v1.0/groups/{id}/validateProperties
Content-type: application/json
Content-length: 132

{
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ddb01-166">C#</span><span class="sxs-lookup"><span data-stu-id="ddb01-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ddb01-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddb01-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ddb01-168">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ddb01-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ddb01-169">Java</span><span class="sxs-lookup"><span data-stu-id="ddb01-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-validateproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ddb01-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddb01-170">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-validation-errors"></a><span data-ttu-id="ddb01-171">Exemplo 2: solicitação com erros de validação</span><span class="sxs-lookup"><span data-stu-id="ddb01-171">Example 2: Request with validation errors</span></span>
<span data-ttu-id="ddb01-172">Este é um exemplo de uma solicitação com erros de validação.</span><span class="sxs-lookup"><span data-stu-id="ddb01-172">This is an example of a request with validation errors.</span></span>

#### <a name="request"></a><span data-ttu-id="ddb01-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddb01-173">Request</span></span>
``` http
POST https://graph.microsoft.com/v1.0/groups/{id}/validateProperties
Content-type: application/json
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

#### <a name="response"></a><span data-ttu-id="ddb01-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddb01-174">Response</span></span>
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
