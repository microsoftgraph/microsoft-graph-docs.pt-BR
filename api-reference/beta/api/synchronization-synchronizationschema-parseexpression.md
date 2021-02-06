---
title: 'synchronizationSchema: parseExpression'
description: '(.. Objeto /resources/synchronization_attributemappingsource.md). '
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: c53046032ea4927d5f475cbb05961253fd323939
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136357"
---
# <a name="synchronizationschema-parseexpression"></a><span data-ttu-id="495a5-103">synchronizationSchema: parseExpression</span><span class="sxs-lookup"><span data-stu-id="495a5-103">synchronizationSchema: parseExpression</span></span>

<span data-ttu-id="495a5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="495a5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="495a5-105">Analisar uma determinada expressão de cadeia de caracteres em [um objeto attributeMappingSource.](../resources/synchronization-attributemappingsource.md)</span><span class="sxs-lookup"><span data-stu-id="495a5-105">Parse a given string expression into an [attributeMappingSource](../resources/synchronization-attributemappingsource.md) object.</span></span>

<span data-ttu-id="495a5-106">Para obter mais informações sobre expressões, consulte [Escrever expressões para mapeamentos de atributos no Azure Active Directory.](/azure/active-directory/active-directory-saas-writing-expressions-for-attribute-mappings)</span><span class="sxs-lookup"><span data-stu-id="495a5-106">For more information about expressions, see [Writing Expressions for Attribute Mappings in Azure Active Directory](/azure/active-directory/active-directory-saas-writing-expressions-for-attribute-mappings).</span></span>

## <a name="permissions"></a><span data-ttu-id="495a5-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="495a5-107">Permissions</span></span>
<span data-ttu-id="495a5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="495a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="495a5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="495a5-110">Permission type</span></span>                        | <span data-ttu-id="495a5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="495a5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="495a5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="495a5-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="495a5-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="495a5-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="495a5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="495a5-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="495a5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="495a5-115">Not supported.</span></span>|
|<span data-ttu-id="495a5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="495a5-116">Application</span></span>                            |<span data-ttu-id="495a5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="495a5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="495a5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="495a5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/schema/parseExpression
POST /servicePrincipals/{id}/synchronization/templates/{id}/schema/parseExpression

```
## <a name="request-headers"></a><span data-ttu-id="495a5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="495a5-119">Request headers</span></span>
| <span data-ttu-id="495a5-120">Nome</span><span class="sxs-lookup"><span data-stu-id="495a5-120">Name</span></span>       | <span data-ttu-id="495a5-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="495a5-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="495a5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="495a5-122">Authorization</span></span>  | <span data-ttu-id="495a5-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="495a5-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="495a5-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="495a5-124">Request body</span></span>
<span data-ttu-id="495a5-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="495a5-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="495a5-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="495a5-126">Parameter</span></span>    | <span data-ttu-id="495a5-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="495a5-127">Type</span></span>   |<span data-ttu-id="495a5-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="495a5-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="495a5-129">expressão</span><span class="sxs-lookup"><span data-stu-id="495a5-129">expression</span></span>               |<span data-ttu-id="495a5-130">String</span><span class="sxs-lookup"><span data-stu-id="495a5-130">String</span></span>               |<span data-ttu-id="495a5-131">Expressão a ser analisado.</span><span class="sxs-lookup"><span data-stu-id="495a5-131">Expression to parse.</span></span>|
|<span data-ttu-id="495a5-132">testInputObject</span><span class="sxs-lookup"><span data-stu-id="495a5-132">testInputObject</span></span>          |[<span data-ttu-id="495a5-133">expressionInputObject</span><span class="sxs-lookup"><span data-stu-id="495a5-133">expressionInputObject</span></span>](../resources/synchronization-expressioninputobject.md)|<span data-ttu-id="495a5-134">Teste o objeto de dados para avaliar a expressão.</span><span class="sxs-lookup"><span data-stu-id="495a5-134">Test data object to evaluate expression against.</span></span> <span data-ttu-id="495a5-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="495a5-135">Optional.</span></span>|
|<span data-ttu-id="495a5-136">targetAttributeDefinition</span><span class="sxs-lookup"><span data-stu-id="495a5-136">targetAttributeDefinition</span></span>|[<span data-ttu-id="495a5-137">attributeDefinition</span><span class="sxs-lookup"><span data-stu-id="495a5-137">attributeDefinition</span></span>](../resources/synchronization-attributedefinition.md) |<span data-ttu-id="495a5-138">Definição do atributo que será mapeado para essa expressão.</span><span class="sxs-lookup"><span data-stu-id="495a5-138">Definition of the attribute that will be mapped to this expression.</span></span> <span data-ttu-id="495a5-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="495a5-139">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="495a5-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="495a5-140">Response</span></span>
<span data-ttu-id="495a5-141">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto parseExpressionResponse](../resources/synchronization-parseexpressionresponse.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="495a5-141">If successful, this method returns a `200 OK` response code and a [parseExpressionResponse](../resources/synchronization-parseexpressionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="495a5-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="495a5-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="495a5-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="495a5-143">Request</span></span>
<span data-ttu-id="495a5-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="495a5-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="495a5-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="495a5-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_parseexpression"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{id}/schema/parseExpression
Content-type: application/json

{
    "expression":"Replace([preferredLanguage], \"-\", , , \"_\", ,  )",
    "targetAttributeDefinition":null,
    "testInputObject": {
        definition: null,
        properties:[
            { key: "objectId", value : "66E4A8CC-1B7B-435E-95F8-F06CEA133828" },
            { key: "IsSoftDeleted", value: "false"},
            { key: "accountEnabled", value: "true"},
            { key: "streetAddress", value: "1 Redmond Way"},
            { key: "city", value: "Redmond"},
            { key: "state", value: "WA"},
            { key: "postalCode", value: "98052"},
            { key: "country", value: "USA"},
            { key: "department", value: "Sales"},
            { key: "displayName", value: "John Smith"},
            { key: "extensionAttribute1", value: "Sample 1"},
            { key: "extensionAttribute2", value: "Sample 2"},
            { key: "extensionAttribute3", value: "Sample 3"},
            { key: "extensionAttribute4", value: "Sample 4"},
            { key: "extensionAttribute5", value: "Sample 5"},
            { key: "extensionAttribute6", value: "Sample 6"},
            { key: "extensionAttribute7", value: "Sample 1"},
            { key: "extensionAttribute8", value: "Sample 1"},
            { key: "extensionAttribute9", value: "Sample 1"},
            { key: "extensionAttribute10", value: "Sample 1"},
            { key: "extensionAttribute11", value: "Sample 1"},
            { key: "extensionAttribute12", value: "Sample 1"},
            { key: "extensionAttribute13", value: "Sample 1"},
            { key: "extensionAttribute14", value: "Sample 1"},
            { key: "extensionAttribute15", value: "Sample 1"},
            { key: "givenName", value: "John"},
            { key: "jobTitle", value: "Finance manager"},
            { key: "mail", value: "johns@contoso.com"},
            { key: "mailNickname", value: "johns"},
            { key: "manager", value: "maxs@contoso.com"},
            { key: "mobile", value: "425-555-0010"},
            { key: "onPremisesSecurityIdentifier", value: "66E4A8CC-1B7B-435E-95F8-F06CEA133828"},
            { key: "passwordProfile.password", value: ""},
            { key: "physicalDeliveryOfficeName", value: "Main Office"},
            { key: "preferredLanguage", value: "EN-US"},
            { key: "proxyAddresses", value: ""},
            { key: "surname", value: "Smith"},
            { key: "telephoneNumber", value: "425-555-0011"},
            { key: "userPrincipalName", value: "johns@contoso.com"},
            { key: "appRoleAssignments", "value@odata.type":"#Collection(String)", value: ["Default Assignment"] }
        ]
    }
}
```
# <a name="c"></a>[<span data-ttu-id="495a5-146">C#</span><span class="sxs-lookup"><span data-stu-id="495a5-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationschema-parseexpression-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="495a5-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="495a5-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationschema-parseexpression-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="495a5-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="495a5-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationschema-parseexpression-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="495a5-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="495a5-149">Response</span></span>
<span data-ttu-id="495a5-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="495a5-150">The following is an example of the response.</span></span>

><span data-ttu-id="495a5-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="495a5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.parseExpressionResponse"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "error": null,
    "evaluationSucceeded": true,
    "evaluationResult": [
        "EN_US"
    ],
    "parsedExpression": {
        "expression": "Replace([preferredLanguage], \"-\", , , \"_\", , )",
        "name": "Replace",
        "parameters": [
            {
                "key": "source",
                "value": {
                    "expression": "[preferredLanguage]",
                    "name": "preferredLanguage",
                    "parameters": [],
                    "type": "Attribute"
                }
            },
            {
                "key": "Find",
                "value": {
                    "expression": "\"-\"",
                    "name": "-",
                    "parameters": [],
                    "type": "Constant"
                }
            },
            {
                "key": "Replacement",
                "value": {
                    "expression": "\"_\"",
                    "name": "_",
                    "parameters": [],
                    "type": "Constant"
                }
            }
        ],
        "type": "Function"
    },
    "parsingSucceeded": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationSchema: parseExpression",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


