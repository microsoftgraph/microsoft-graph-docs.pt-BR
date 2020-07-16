---
title: 'Group: ValidateProperties'
description: Validar que o nome de exibição ou o apelido de email de um grupo do Microsoft 365 está em conformidade com as políticas de nomenclatura.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: acdc168df631a0db5eff277348cf4b0e43d85357
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897103"
---
# <a name="group-validateproperties"></a><span data-ttu-id="47f0b-103">Group: ValidateProperties</span><span class="sxs-lookup"><span data-stu-id="47f0b-103">group: validateProperties</span></span>

<span data-ttu-id="47f0b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47f0b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="47f0b-105">Validar que o nome de exibição ou o apelido de email de um grupo do Microsoft 365 está em conformidade com as políticas de nomenclatura.</span><span class="sxs-lookup"><span data-stu-id="47f0b-105">Validate that a Microsoft 365 group's display name or mail nickname complies with naming policies.</span></span>  <span data-ttu-id="47f0b-106">Os clientes podem usar essa API para determinar se um nome de exibição ou apelido de email é válido antes de tentar [Atualizar](group-update.md) um grupo do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="47f0b-106">Clients can use this API to determine whether a display name or mail nickname is valid before trying to [update](group-update.md) a Microsoft 365 group.</span></span> <span data-ttu-id="47f0b-107">Para validar as propriedades antes de criar um grupo, use a função [directoryobject: ValidateProperties](directoryobject-validateproperties.md) .</span><span class="sxs-lookup"><span data-stu-id="47f0b-107">To validate the properties before creating a group, use the [directoryobject:validateProperties](directoryobject-validateproperties.md) function.</span></span>

<span data-ttu-id="47f0b-108">As seguintes validações de política são realizadas para o nome de exibição e as propriedades de apelido de email:</span><span class="sxs-lookup"><span data-stu-id="47f0b-108">The following policy validations are performed for the display name and mail nickname properties:</span></span>
1. <span data-ttu-id="47f0b-109">Validar a política de nomenclatura de prefixo e sufixo</span><span class="sxs-lookup"><span data-stu-id="47f0b-109">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="47f0b-110">Validar a política personalizada de palavras banidas</span><span class="sxs-lookup"><span data-stu-id="47f0b-110">Validate the custom banned words policy</span></span>

<span data-ttu-id="47f0b-111">Essa API só retorna a primeira falha de validação encontrada.</span><span class="sxs-lookup"><span data-stu-id="47f0b-111">This API only returns the first validation failure that is encountered.</span></span> <span data-ttu-id="47f0b-112">Se as propriedades falharem várias validações, somente a primeira falha de validação será retornada.</span><span class="sxs-lookup"><span data-stu-id="47f0b-112">If the properties fail multiple validations, only the first validation failure is returned.</span></span> <span data-ttu-id="47f0b-113">No entanto, você pode validar tanto o apelido de email quanto o nome de exibição e receber uma coleção de erros de validação se você estiver validando apenas o prefixo e a política de nomenclatura de sufixo.</span><span class="sxs-lookup"><span data-stu-id="47f0b-113">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span> <span data-ttu-id="47f0b-114">Para saber mais sobre como configurar políticas de nomenclatura, consulte [Configure Naming Policy](/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell).</span><span class="sxs-lookup"><span data-stu-id="47f0b-114">To learn more about configuring naming policies, see [Configure naming policy](/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell).</span></span>

## <a name="permissions"></a><span data-ttu-id="47f0b-115">Permissões</span><span class="sxs-lookup"><span data-stu-id="47f0b-115">Permissions</span></span>

<span data-ttu-id="47f0b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47f0b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47f0b-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47f0b-118">Permission type</span></span>      | <span data-ttu-id="47f0b-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47f0b-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47f0b-120">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47f0b-120">Delegated (work or school account)</span></span> | <span data-ttu-id="47f0b-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47f0b-121">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="47f0b-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47f0b-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47f0b-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47f0b-123">Not supported.</span></span>    |
|<span data-ttu-id="47f0b-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47f0b-124">Application</span></span> | <span data-ttu-id="47f0b-125">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47f0b-125">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="47f0b-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47f0b-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/{id}/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="47f0b-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47f0b-127">Request headers</span></span>

| <span data-ttu-id="47f0b-128">Nome</span><span class="sxs-lookup"><span data-stu-id="47f0b-128">Name</span></span>           | <span data-ttu-id="47f0b-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="47f0b-129">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="47f0b-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="47f0b-130">Authorization</span></span>  | <span data-ttu-id="47f0b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47f0b-p104">Bearer {token}. Required.</span></span>    |
| <span data-ttu-id="47f0b-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="47f0b-133">Content-Type</span></span>   | <span data-ttu-id="47f0b-134">application/json</span><span class="sxs-lookup"><span data-stu-id="47f0b-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="47f0b-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47f0b-135">Request body</span></span>

<span data-ttu-id="47f0b-136">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47f0b-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="47f0b-137">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="47f0b-137">Parameter</span></span>    | <span data-ttu-id="47f0b-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="47f0b-138">Type</span></span>   |<span data-ttu-id="47f0b-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="47f0b-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47f0b-140">displayName</span><span class="sxs-lookup"><span data-stu-id="47f0b-140">displayName</span></span>|<span data-ttu-id="47f0b-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="47f0b-141">String</span></span>| <span data-ttu-id="47f0b-142">O nome de exibição do grupo a ser validado.</span><span class="sxs-lookup"><span data-stu-id="47f0b-142">The display name of the group to validate.</span></span> <span data-ttu-id="47f0b-143">A propriedade não é necessária individualmente.</span><span class="sxs-lookup"><span data-stu-id="47f0b-143">The property is not individually required.</span></span> <span data-ttu-id="47f0b-144">No entanto, pelo menos uma propriedade (**DisplayName** ou **mailNickname**) é necessária.</span><span class="sxs-lookup"><span data-stu-id="47f0b-144">However, at least one property (**displayName** or **mailNickname**) is required.</span></span> |
|<span data-ttu-id="47f0b-145">mailNickname</span><span class="sxs-lookup"><span data-stu-id="47f0b-145">mailNickname</span></span>|<span data-ttu-id="47f0b-146">String</span><span class="sxs-lookup"><span data-stu-id="47f0b-146">String</span></span>| <span data-ttu-id="47f0b-147">O apelido de email do grupo a ser validado.</span><span class="sxs-lookup"><span data-stu-id="47f0b-147">The mail nickname of the group to validate.</span></span> <span data-ttu-id="47f0b-148">A propriedade não é necessária individualmente.</span><span class="sxs-lookup"><span data-stu-id="47f0b-148">The property is not individually required.</span></span> <span data-ttu-id="47f0b-149">No entanto, pelo menos uma propriedade (**DisplayName** ou **mailNickname**) é necessária.</span><span class="sxs-lookup"><span data-stu-id="47f0b-149">However, at least one property (**displayName** or **mailNickname**) is required.</span></span> |
|<span data-ttu-id="47f0b-150">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="47f0b-150">onBehalfOfUserId</span></span>|<span data-ttu-id="47f0b-151">Guid</span><span class="sxs-lookup"><span data-stu-id="47f0b-151">Guid</span></span>| <span data-ttu-id="47f0b-152">A ID do usuário a ser personificada ao chamar a API.</span><span class="sxs-lookup"><span data-stu-id="47f0b-152">The ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="47f0b-153">Os resultados de validação são para os atributos e funções **do onBehalfOfUserId** .</span><span class="sxs-lookup"><span data-stu-id="47f0b-153">The validation results are for the **onBehalfOfUserId's** attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="47f0b-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="47f0b-154">Response</span></span>
<span data-ttu-id="47f0b-155">Se tiver êxito e não houver erros de validação, o método retornará o `204 No Content` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="47f0b-155">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="47f0b-156">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47f0b-156">It does not return anything in the response body.</span></span>

<span data-ttu-id="47f0b-157">Se a solicitação for inválida, o método retornará um `400 Bad Request` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="47f0b-157">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="47f0b-158">Uma mensagem de erro com detalhes sobre a solicitação inválida é retornada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47f0b-158">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="47f0b-159">Se houver um erro de validação.</span><span class="sxs-lookup"><span data-stu-id="47f0b-159">If there is a validation error.</span></span> <span data-ttu-id="47f0b-160">O método retorna um `422 Unprocessable Entity` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="47f0b-160">The method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="47f0b-161">Uma mensagem de erro e um conjunto de detalhes de erro é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47f0b-161">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="47f0b-162">Exemplos</span><span class="sxs-lookup"><span data-stu-id="47f0b-162">Examples</span></span>

### <a name="example-1-successful-validation-request"></a><span data-ttu-id="47f0b-163">Exemplo 1: solicitação de validação bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="47f0b-163">Example 1: Successful validation request</span></span>
<span data-ttu-id="47f0b-164">Este é um exemplo de uma solicitação de validação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="47f0b-164">This is an example of a successful validation request.</span></span>

#### <a name="request"></a><span data-ttu-id="47f0b-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47f0b-165">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="47f0b-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="47f0b-166">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="47f0b-167">C#</span><span class="sxs-lookup"><span data-stu-id="47f0b-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="47f0b-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47f0b-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="47f0b-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47f0b-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="47f0b-170">Java</span><span class="sxs-lookup"><span data-stu-id="47f0b-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-validateproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="47f0b-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="47f0b-171">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-validation-errors"></a><span data-ttu-id="47f0b-172">Exemplo 2: solicitação com erros de validação</span><span class="sxs-lookup"><span data-stu-id="47f0b-172">Example 2: Request with validation errors</span></span>
<span data-ttu-id="47f0b-173">Este é um exemplo de uma solicitação com erros de validação.</span><span class="sxs-lookup"><span data-stu-id="47f0b-173">This is an example of a request with validation errors.</span></span>

#### <a name="request"></a><span data-ttu-id="47f0b-174">Solicitar</span><span class="sxs-lookup"><span data-stu-id="47f0b-174">Request</span></span>
``` http
POST https://graph.microsoft.com/v1.0/groups/{id}/validateProperties
Content-type: application/json
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

#### <a name="response"></a><span data-ttu-id="47f0b-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="47f0b-175">Response</span></span>
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
