---
title: 'directoryobject: ValidateProperties'
description: Validar que o nome de exibição ou o apelido de email de um grupo do Microsoft 365 está em conformidade com as políticas de nomenclatura.
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a7e434313c9f66d9b780d0bf521be49dd53e8b3e
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897796"
---
# <a name="directoryobject-validateproperties"></a><span data-ttu-id="8bfd9-103">directoryobject: ValidateProperties</span><span class="sxs-lookup"><span data-stu-id="8bfd9-103">directoryObject: validateProperties</span></span>

<span data-ttu-id="8bfd9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bfd9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8bfd9-105">Validar que o nome de exibição ou o apelido de email de um grupo do Microsoft 365 está em conformidade com as políticas de nomenclatura.</span><span class="sxs-lookup"><span data-stu-id="8bfd9-105">Validate that a Microsoft 365 group's display name or mail nickname complies with naming policies.</span></span>  <span data-ttu-id="8bfd9-106">Os clientes podem usar essa API para determinar se um nome de exibição ou apelido de email é válido antes de tentar [criar](group-post-groups.md) um grupo do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="8bfd9-106">Clients can use this API to determine whether a display name or mail nickname is valid before trying to [create](group-post-groups.md) a Microsoft 365 group.</span></span> <span data-ttu-id="8bfd9-107">Para validar as propriedades de um grupo existente, use a função [Group: ValidateProperties](group-validateproperties.md) .</span><span class="sxs-lookup"><span data-stu-id="8bfd9-107">To validate the properties of an existing group, use the [group: validateProperties](group-validateproperties.md) function.</span></span>

<span data-ttu-id="8bfd9-108">As seguintes validações de política são realizadas para o nome de exibição e as propriedades de apelido de email:</span><span class="sxs-lookup"><span data-stu-id="8bfd9-108">The following policy validations are performed for the display name and mail nickname properties:</span></span>
1. <span data-ttu-id="8bfd9-109">Validar a política de nomenclatura de prefixo e sufixo</span><span class="sxs-lookup"><span data-stu-id="8bfd9-109">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="8bfd9-110">Validar a política personalizada de palavras banidas</span><span class="sxs-lookup"><span data-stu-id="8bfd9-110">Validate the custom banned words policy</span></span>
3. <span data-ttu-id="8bfd9-111">Validar que o apelido do email é exclusivo</span><span class="sxs-lookup"><span data-stu-id="8bfd9-111">Validate that the mail nickname is unique</span></span>

<span data-ttu-id="8bfd9-112">Essa API só retorna a primeira falha de validação encontrada.</span><span class="sxs-lookup"><span data-stu-id="8bfd9-112">This API only returns the first validation failure that is encountered.</span></span> <span data-ttu-id="8bfd9-113">Se as propriedades falharem várias validações, somente a primeira falha de validação será retornada.</span><span class="sxs-lookup"><span data-stu-id="8bfd9-113">If the properties fail multiple validations, only the first validation failure is returned.</span></span> <span data-ttu-id="8bfd9-114">No entanto, você pode validar tanto o apelido de email quanto o nome de exibição e receber uma coleção de erros de validação se você estiver validando apenas o prefixo e a política de nomenclatura de sufixo.</span><span class="sxs-lookup"><span data-stu-id="8bfd9-114">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span> <span data-ttu-id="8bfd9-115">Para saber mais sobre como configurar políticas de nomenclatura, consulte [Configure Naming Policy](/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell).</span><span class="sxs-lookup"><span data-stu-id="8bfd9-115">To learn more about configuring naming policies, see [Configure naming policy](/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell).</span></span>

## <a name="permissions"></a><span data-ttu-id="8bfd9-116">Permissões</span><span class="sxs-lookup"><span data-stu-id="8bfd9-116">Permissions</span></span>
<span data-ttu-id="8bfd9-117">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="8bfd9-117">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="8bfd9-118">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bfd9-118">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bfd9-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8bfd9-119">Permission type</span></span>      | <span data-ttu-id="8bfd9-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8bfd9-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8bfd9-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8bfd9-121">Delegated (work or school account)</span></span> | <span data-ttu-id="8bfd9-122">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8bfd9-122">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="8bfd9-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8bfd9-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bfd9-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8bfd9-124">Not supported.</span></span>    |
|<span data-ttu-id="8bfd9-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8bfd9-125">Application</span></span> | <span data-ttu-id="8bfd9-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bfd9-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8bfd9-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8bfd9-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="8bfd9-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8bfd9-128">Request headers</span></span>

| <span data-ttu-id="8bfd9-129">Nome</span><span class="sxs-lookup"><span data-stu-id="8bfd9-129">Name</span></span>           | <span data-ttu-id="8bfd9-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="8bfd9-130">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="8bfd9-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="8bfd9-131">Authorization</span></span>  | <span data-ttu-id="8bfd9-132">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="8bfd9-132">Bearer {token}.</span></span> <span data-ttu-id="8bfd9-133">Required.</span><span class="sxs-lookup"><span data-stu-id="8bfd9-133">Required.</span></span>    |
| <span data-ttu-id="8bfd9-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8bfd9-134">Content-Type</span></span>   | <span data-ttu-id="8bfd9-135">application/json</span><span class="sxs-lookup"><span data-stu-id="8bfd9-135">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8bfd9-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8bfd9-136">Request body</span></span>
<span data-ttu-id="8bfd9-137">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8bfd9-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8bfd9-138">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8bfd9-138">Parameter</span></span>    | <span data-ttu-id="8bfd9-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="8bfd9-139">Type</span></span>   |<span data-ttu-id="8bfd9-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="8bfd9-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8bfd9-141">entityType</span><span class="sxs-lookup"><span data-stu-id="8bfd9-141">entityType</span></span>|<span data-ttu-id="8bfd9-142">String</span><span class="sxs-lookup"><span data-stu-id="8bfd9-142">String</span></span>| <span data-ttu-id="8bfd9-143">Group é o único tipo de entidade com suporte.</span><span class="sxs-lookup"><span data-stu-id="8bfd9-143">Group is the only supported entity type.</span></span> |
|<span data-ttu-id="8bfd9-144">displayName</span><span class="sxs-lookup"><span data-stu-id="8bfd9-144">displayName</span></span>|<span data-ttu-id="8bfd9-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8bfd9-145">String</span></span>| <span data-ttu-id="8bfd9-146">O nome de exibição do grupo a ser validado.</span><span class="sxs-lookup"><span data-stu-id="8bfd9-146">The display name of the group to validate.</span></span> <span data-ttu-id="8bfd9-147">A propriedade não é necessária individualmente.</span><span class="sxs-lookup"><span data-stu-id="8bfd9-147">The property is not individually required.</span></span> <span data-ttu-id="8bfd9-148">No entanto, pelo menos uma propriedade (**DisplayName** ou **mailNickname**) é necessária.</span><span class="sxs-lookup"><span data-stu-id="8bfd9-148">However, at least one property (**displayName** or **mailNickname**) is required.</span></span> |
|<span data-ttu-id="8bfd9-149">mailNickname</span><span class="sxs-lookup"><span data-stu-id="8bfd9-149">mailNickname</span></span>|<span data-ttu-id="8bfd9-150">String</span><span class="sxs-lookup"><span data-stu-id="8bfd9-150">String</span></span>| <span data-ttu-id="8bfd9-151">O apelido de email do grupo a ser validado.</span><span class="sxs-lookup"><span data-stu-id="8bfd9-151">The mail nickname of the group to validate.</span></span> <span data-ttu-id="8bfd9-152">A propriedade não é necessária individualmente.</span><span class="sxs-lookup"><span data-stu-id="8bfd9-152">The property is not individually required.</span></span> <span data-ttu-id="8bfd9-153">No entanto, pelo menos uma propriedade (**DisplayName** ou **mailNickname**) é necessária.</span><span class="sxs-lookup"><span data-stu-id="8bfd9-153">However, at least one property (**displayName** or **mailNickname**) is required.</span></span> |
|<span data-ttu-id="8bfd9-154">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="8bfd9-154">onBehalfOfUserId</span></span>|<span data-ttu-id="8bfd9-155">Guid</span><span class="sxs-lookup"><span data-stu-id="8bfd9-155">Guid</span></span>| <span data-ttu-id="8bfd9-156">A ID do usuário a ser personificada ao chamar a API.</span><span class="sxs-lookup"><span data-stu-id="8bfd9-156">The ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="8bfd9-157">Os resultados de validação são para os atributos e funções **do onBehalfOfUserId** .</span><span class="sxs-lookup"><span data-stu-id="8bfd9-157">The validation results are for the **onBehalfOfUserId's** attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="8bfd9-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bfd9-158">Response</span></span>

<span data-ttu-id="8bfd9-159">Se tiver êxito e não houver erros de validação, o método retornará o `204 No Content` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="8bfd9-159">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="8bfd9-160">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8bfd9-160">It does not return anything in the response body.</span></span>

<span data-ttu-id="8bfd9-161">Se a solicitação for inválida, o método retornará um `400 Bad Request` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="8bfd9-161">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="8bfd9-162">Uma mensagem de erro com detalhes sobre a solicitação inválida é retornada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8bfd9-162">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="8bfd9-163">Se houver um erro de validação, o método retornará um `422 Unprocessable Entity` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="8bfd9-163">If there is a validation error, the method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="8bfd9-164">Uma mensagem de erro e um conjunto de detalhes de erro é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8bfd9-164">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8bfd9-165">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8bfd9-165">Examples</span></span>

### <a name="example-1-successful-validation-request"></a><span data-ttu-id="8bfd9-166">Exemplo 1: solicitação de validação bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="8bfd9-166">Example 1: Successful validation request</span></span>
<span data-ttu-id="8bfd9-167">Este é um exemplo de uma solicitação de validação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="8bfd9-167">This is an example of a successful validation request.</span></span>

#### <a name="request"></a><span data-ttu-id="8bfd9-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8bfd9-168">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8bfd9-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="8bfd9-169">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8bfd9-170">C#</span><span class="sxs-lookup"><span data-stu-id="8bfd9-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8bfd9-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8bfd9-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8bfd9-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8bfd9-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8bfd9-173">Java</span><span class="sxs-lookup"><span data-stu-id="8bfd9-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-validateproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8bfd9-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bfd9-174">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```


### <a name="example-2-request-with-validation-errors"></a><span data-ttu-id="8bfd9-175">Exemplo 2: solicitação com erros de validação</span><span class="sxs-lookup"><span data-stu-id="8bfd9-175">Example 2: Request with validation errors</span></span>
<span data-ttu-id="8bfd9-176">Este é um exemplo de uma solicitação com erros de validação.</span><span class="sxs-lookup"><span data-stu-id="8bfd9-176">This is an example of a request with validation errors.</span></span>

#### <a name="request"></a><span data-ttu-id="8bfd9-177">Solicitar</span><span class="sxs-lookup"><span data-stu-id="8bfd9-177">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="8bfd9-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bfd9-178">Response</span></span>
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
