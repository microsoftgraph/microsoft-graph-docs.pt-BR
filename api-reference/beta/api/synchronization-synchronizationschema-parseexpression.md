---
title: 'synchronizationSchema: ParseName'
description: '(.. objeto/Resources/synchronization_attributemappingsource.MD). '
localization_priority: Normal
ms.openlocfilehash: b11d50bc62dafedcdbf658e15e5501e134eb7a26
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637973"
---
# <a name="synchronizationschema-parseexpression"></a><span data-ttu-id="d5280-103">synchronizationSchema: ParseName</span><span class="sxs-lookup"><span data-stu-id="d5280-103">synchronizationSchema: parseExpression</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5280-104">Analisar uma determinada expressão de cadeia de caracteres em um [attributeMappingSource | (.. objeto/Resources/synchronization_attributemappingsource.MD).</span><span class="sxs-lookup"><span data-stu-id="d5280-104">Parse a given string expression into an [attributeMappingSource|(../resources/synchronization_attributemappingsource.md) object.</span></span> 

<span data-ttu-id="d5280-105">Para obter mais informações sobre expressões, consulte [Writing Expressions for Attribute Mappings in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-writing-expressions-for-attribute-mappings).</span><span class="sxs-lookup"><span data-stu-id="d5280-105">For more information about expressions, see [Writing Expressions for Attribute Mappings in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-writing-expressions-for-attribute-mappings).</span></span>

## <a name="permissions"></a><span data-ttu-id="d5280-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d5280-106">Permissions</span></span>
<span data-ttu-id="d5280-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5280-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5280-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5280-109">Permission type</span></span>                        | <span data-ttu-id="d5280-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d5280-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5280-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5280-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="d5280-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5280-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="d5280-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5280-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="d5280-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5280-114">Not supported.</span></span>|
|<span data-ttu-id="d5280-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5280-115">Application</span></span>                            |<span data-ttu-id="d5280-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5280-116">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="d5280-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5280-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/schema/parseExpression
POST /servicePrincipals/{id}/synchronization/templates/{id}/schema/parseExpression

```
## <a name="request-headers"></a><span data-ttu-id="d5280-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5280-118">Request headers</span></span>
| <span data-ttu-id="d5280-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d5280-119">Name</span></span>       | <span data-ttu-id="d5280-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5280-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d5280-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5280-121">Authorization</span></span>  | <span data-ttu-id="d5280-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="d5280-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5280-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5280-123">Request body</span></span>
<span data-ttu-id="d5280-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5280-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d5280-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d5280-125">Parameter</span></span>    | <span data-ttu-id="d5280-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5280-126">Type</span></span>   |<span data-ttu-id="d5280-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5280-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d5280-128">expressão</span><span class="sxs-lookup"><span data-stu-id="d5280-128">expression</span></span>               |<span data-ttu-id="d5280-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5280-129">String</span></span>               |<span data-ttu-id="d5280-130">Expressão a ser analisada.</span><span class="sxs-lookup"><span data-stu-id="d5280-130">Expression to parse.</span></span>|
|<span data-ttu-id="d5280-131">testInputObject</span><span class="sxs-lookup"><span data-stu-id="d5280-131">testInputObject</span></span>          |[<span data-ttu-id="d5280-132">expressionInputObject</span><span class="sxs-lookup"><span data-stu-id="d5280-132">expressionInputObject</span></span>](../resources/synchronization-expressioninputobject.md)|<span data-ttu-id="d5280-133">Objeto de dados de teste para avaliar a expressão.</span><span class="sxs-lookup"><span data-stu-id="d5280-133">Test data object to evaluate expression against.</span></span> <span data-ttu-id="d5280-134">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d5280-134">Optional.</span></span>|
|<span data-ttu-id="d5280-135">targetAttributeDefinition</span><span class="sxs-lookup"><span data-stu-id="d5280-135">targetAttributeDefinition</span></span>|[<span data-ttu-id="d5280-136">attributeDefinition</span><span class="sxs-lookup"><span data-stu-id="d5280-136">attributeDefinition</span></span>](../resources/synchronization-attributedefinition.md) |<span data-ttu-id="d5280-137">Definição do atributo que será mapeado para esta expressão.</span><span class="sxs-lookup"><span data-stu-id="d5280-137">Definition of the attribute that will be mapped to this expression.</span></span> <span data-ttu-id="d5280-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d5280-138">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="d5280-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5280-139">Response</span></span>
<span data-ttu-id="d5280-140">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [parseExpressionResponse](../resources/synchronization-parseexpressionresponse.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5280-140">If successful, this method returns a `200 OK` response code and a [parseExpressionResponse](../resources/synchronization-parseexpressionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5280-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d5280-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d5280-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5280-142">Request</span></span>
<span data-ttu-id="d5280-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5280-143">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="d5280-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5280-144">Response</span></span>
<span data-ttu-id="d5280-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d5280-145">The following is an example of the response.</span></span> 

><span data-ttu-id="d5280-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d5280-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d5280-148">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="d5280-148">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d5280-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5280-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/synchronizationschema_parseexpression-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-parseexpression.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
