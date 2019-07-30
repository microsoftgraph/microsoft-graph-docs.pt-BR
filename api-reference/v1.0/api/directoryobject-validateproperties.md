---
title: 'directoryobject: ValidateProperties'
description: Valide se o nome de exibição ou o apelido de email de um grupo do Office 365 está em conformidade com as políticas de nomenclatura.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f26857514ec180dbbc50c73eeb8eccc4b30185ed
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932195"
---
# <a name="directoryobject-validateproperties"></a><span data-ttu-id="e076b-103">directoryobject: ValidateProperties</span><span class="sxs-lookup"><span data-stu-id="e076b-103">directoryObject: validateProperties</span></span>

<span data-ttu-id="e076b-104">Valide se o nome de exibição ou o apelido de email de um grupo do Office 365 está em conformidade com as políticas de nomenclatura.</span><span class="sxs-lookup"><span data-stu-id="e076b-104">Validate that an Office 365 group's display name or mail nickname complies with naming policies.</span></span>  <span data-ttu-id="e076b-105">Os clientes podem usar essa API para determinar se um nome de exibição ou apelido de email é válido antes de tentar [criar](group-post-groups.md) um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="e076b-105">Clients can use this API to determine whether a display name or mail nickname is valid before trying to [create](group-post-groups.md) an Office 365 group.</span></span> <span data-ttu-id="e076b-106">Para validar as propriedades de um grupo existente, use a função [Group: ValidateProperties](group-validateproperties.md) .</span><span class="sxs-lookup"><span data-stu-id="e076b-106">To validate the properties of an existing group, use the [group: validateProperties](group-validateproperties.md) function.</span></span>

<span data-ttu-id="e076b-107">As seguintes validações de política são realizadas para o nome de exibição e as propriedades de apelido de email:</span><span class="sxs-lookup"><span data-stu-id="e076b-107">The following policy validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="e076b-108">Validar a política de nomenclatura de prefixo e sufixo</span><span class="sxs-lookup"><span data-stu-id="e076b-108">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="e076b-109">Validar a política personalizada de palavras banidas</span><span class="sxs-lookup"><span data-stu-id="e076b-109">Validate the custom banned words policy</span></span>
3. <span data-ttu-id="e076b-110">Validar que o apelido do email é exclusivo</span><span class="sxs-lookup"><span data-stu-id="e076b-110">Validate that the mail nickname is unique</span></span>

<span data-ttu-id="e076b-111">Essa API só retorna a primeira falha de validação encontrada.</span><span class="sxs-lookup"><span data-stu-id="e076b-111">This API only returns the first validation failure that is encountered.</span></span> <span data-ttu-id="e076b-112">Se as propriedades falharem várias validações, somente a primeira falha de validação será retornada.</span><span class="sxs-lookup"><span data-stu-id="e076b-112">If the properties fail multiple validations, only the first validation failure is returned.</span></span> <span data-ttu-id="e076b-113">No entanto, você pode validar tanto o apelido de email quanto o nome de exibição e receber uma coleção de erros de validação se você estiver validando apenas o prefixo e a política de nomenclatura de sufixo.</span><span class="sxs-lookup"><span data-stu-id="e076b-113">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span> <span data-ttu-id="e076b-114">Para saber mais sobre como configurar políticas de nomenclatura, consulte [Configure Naming Policy](https://docs.microsoft.com/en-us/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell).</span><span class="sxs-lookup"><span data-stu-id="e076b-114">To learn more about configuring naming policies, see [Configure naming policy](https://docs.microsoft.com/en-us/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell).</span></span>

## <a name="permissions"></a><span data-ttu-id="e076b-115">Permissões</span><span class="sxs-lookup"><span data-stu-id="e076b-115">Permissions</span></span>
<span data-ttu-id="e076b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e076b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e076b-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e076b-118">Permission type</span></span>      | <span data-ttu-id="e076b-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e076b-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e076b-120">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e076b-120">Delegated (work or school account)</span></span> | <span data-ttu-id="e076b-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e076b-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="e076b-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e076b-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e076b-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e076b-123">Not supported.</span></span>    |
|<span data-ttu-id="e076b-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e076b-124">Application</span></span> | <span data-ttu-id="e076b-125">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e076b-125">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e076b-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e076b-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="e076b-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e076b-127">Request headers</span></span>

| <span data-ttu-id="e076b-128">Nome</span><span class="sxs-lookup"><span data-stu-id="e076b-128">Name</span></span>           | <span data-ttu-id="e076b-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="e076b-129">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="e076b-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="e076b-130">Authorization</span></span>  | <span data-ttu-id="e076b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e076b-p104">Bearer {token}. Required.</span></span>    |
| <span data-ttu-id="e076b-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e076b-133">Content-Type</span></span>   | <span data-ttu-id="e076b-134">application/json</span><span class="sxs-lookup"><span data-stu-id="e076b-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e076b-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e076b-135">Request body</span></span>
<span data-ttu-id="e076b-136">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e076b-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e076b-137">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e076b-137">Parameter</span></span>    | <span data-ttu-id="e076b-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="e076b-138">Type</span></span>   |<span data-ttu-id="e076b-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="e076b-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e076b-140">entityType</span><span class="sxs-lookup"><span data-stu-id="e076b-140">entityType</span></span>|<span data-ttu-id="e076b-141">String</span><span class="sxs-lookup"><span data-stu-id="e076b-141">String</span></span>| <span data-ttu-id="e076b-142">Group é o único tipo de entidade com suporte.</span><span class="sxs-lookup"><span data-stu-id="e076b-142">Group is the only supported entity type.</span></span> |
|<span data-ttu-id="e076b-143">displayName</span><span class="sxs-lookup"><span data-stu-id="e076b-143">displayName</span></span>|<span data-ttu-id="e076b-144">String</span><span class="sxs-lookup"><span data-stu-id="e076b-144">String</span></span>| <span data-ttu-id="e076b-145">O nome de exibição do grupo a ser validado.</span><span class="sxs-lookup"><span data-stu-id="e076b-145">The display name of the group to validate.</span></span> <span data-ttu-id="e076b-146">A propriedade não é necessária individualmente.</span><span class="sxs-lookup"><span data-stu-id="e076b-146">The property is not individually required.</span></span> <span data-ttu-id="e076b-147">No entanto, pelo menos uma propriedade (**DisplayName** ou **mailNickname**) é necessária.</span><span class="sxs-lookup"><span data-stu-id="e076b-147">However, at least one property (**displayName** or **mailNickname**) is required.</span></span> |
|<span data-ttu-id="e076b-148">mailNickname</span><span class="sxs-lookup"><span data-stu-id="e076b-148">mailNickname</span></span>|<span data-ttu-id="e076b-149">String</span><span class="sxs-lookup"><span data-stu-id="e076b-149">String</span></span>| <span data-ttu-id="e076b-150">O apelido de email do grupo a ser validado.</span><span class="sxs-lookup"><span data-stu-id="e076b-150">The mail nickname of the group to validate.</span></span> <span data-ttu-id="e076b-151">A propriedade não é necessária individualmente.</span><span class="sxs-lookup"><span data-stu-id="e076b-151">The property is not individually required.</span></span> <span data-ttu-id="e076b-152">No entanto, pelo menos uma propriedade (**DisplayName** ou **mailNickname**) é necessária.</span><span class="sxs-lookup"><span data-stu-id="e076b-152">However, at least one property (**displayName** or **mailNickname**) is required.</span></span> |
|<span data-ttu-id="e076b-153">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="e076b-153">onBehalfOfUserId</span></span>|<span data-ttu-id="e076b-154">Guid</span><span class="sxs-lookup"><span data-stu-id="e076b-154">Guid</span></span>| <span data-ttu-id="e076b-155">A ID do usuário a ser personificada ao chamar a API.</span><span class="sxs-lookup"><span data-stu-id="e076b-155">The ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="e076b-156">Os resultados de validação são para os atributos e funções **do onBehalfOfUserId** .</span><span class="sxs-lookup"><span data-stu-id="e076b-156">The validation results are for the **onBehalfOfUserId's** attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="e076b-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="e076b-157">Response</span></span>

<span data-ttu-id="e076b-158">Se tiver êxito e não houver erros de validação, o método `204 No Content` retornará o código de resposta.</span><span class="sxs-lookup"><span data-stu-id="e076b-158">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="e076b-159">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e076b-159">It does not return anything in the response body.</span></span>

<span data-ttu-id="e076b-160">Se a solicitação for inválida, o método `400 Bad Request` retornará um código de resposta.</span><span class="sxs-lookup"><span data-stu-id="e076b-160">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="e076b-161">Uma mensagem de erro com detalhes sobre a solicitação inválida é retornada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e076b-161">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="e076b-162">Se houver um erro de validação, o método retornará `422 Unprocessable Entity` um código de resposta.</span><span class="sxs-lookup"><span data-stu-id="e076b-162">If there is a validation error, the method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="e076b-163">Uma mensagem de erro e um conjunto de detalhes de erro é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e076b-163">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e076b-164">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e076b-164">Examples</span></span>

### <a name="example-1-successful-validation-request"></a><span data-ttu-id="e076b-165">Exemplo 1: solicitação de validação bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="e076b-165">Example 1: Successful validation request</span></span>
<span data-ttu-id="e076b-166">Este é um exemplo de uma solicitação de validação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="e076b-166">This is an example of a successful validation request.</span></span>

#### <a name="request"></a><span data-ttu-id="e076b-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e076b-167">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e076b-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="e076b-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/v1.0/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e076b-169">C#</span><span class="sxs-lookup"><span data-stu-id="e076b-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e076b-170">Javascript</span><span class="sxs-lookup"><span data-stu-id="e076b-170">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e076b-171">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e076b-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e076b-172">Java</span><span class="sxs-lookup"><span data-stu-id="e076b-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-validateproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e076b-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="e076b-173">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```


### <a name="example-2-request-with-validation-errors"></a><span data-ttu-id="e076b-174">Exemplo 2: solicitação com erros de validação</span><span class="sxs-lookup"><span data-stu-id="e076b-174">Example 2: Request with validation errors</span></span>
<span data-ttu-id="e076b-175">Este é um exemplo de uma solicitação com erros de validação.</span><span class="sxs-lookup"><span data-stu-id="e076b-175">This is an example of a request with validation errors.</span></span>

#### <a name="request"></a><span data-ttu-id="e076b-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e076b-176">Request</span></span>
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "test",
  "mailNickname": "test",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

#### <a name="response"></a><span data-ttu-id="e076b-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="e076b-177">Response</span></span>
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
