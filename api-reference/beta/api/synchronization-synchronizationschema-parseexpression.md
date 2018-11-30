---
title: 'synchronizationSchema: parseExpression'
description: '(.. / resources/synchronization_attributemappingsource.md) objeto. '
ms.openlocfilehash: d6cc929681458ff00a806150aa8db9daf115548a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036670"
---
# <a name="synchronizationschema-parseexpression"></a><span data-ttu-id="19064-103">synchronizationSchema: parseExpression</span><span class="sxs-lookup"><span data-stu-id="19064-103">synchronizationSchema: parseExpression</span></span>

> <span data-ttu-id="19064-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="19064-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19064-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="19064-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="19064-106">Analisar uma expressão de cadeia de caracteres específica em uma [attributeMappingSource | (… / resources/synchronization_attributemappingsource.md) objeto.</span><span class="sxs-lookup"><span data-stu-id="19064-106">Parse a given string expression into an [attributeMappingSource|(../resources/synchronization_attributemappingsource.md) object.</span></span> 

<span data-ttu-id="19064-107">Para obter mais informações sobre expressões, consulte [Como escrever expressões para mapeamentos de atributo no Windows Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-writing-expressions-for-attribute-mappings).</span><span class="sxs-lookup"><span data-stu-id="19064-107">For more information about expressions, see [Writing Expressions for Attribute Mappings in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-writing-expressions-for-attribute-mappings).</span></span>

## <a name="permissions"></a><span data-ttu-id="19064-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="19064-108">Permissions</span></span>
<span data-ttu-id="19064-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19064-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19064-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19064-111">Permission type</span></span>                        | <span data-ttu-id="19064-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="19064-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="19064-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19064-113">Delegated (work or school account)</span></span>     |<span data-ttu-id="19064-114">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19064-114">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="19064-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19064-115">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="19064-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19064-116">Not supported.</span></span>|
|<span data-ttu-id="19064-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19064-117">Application</span></span>                            |<span data-ttu-id="19064-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19064-118">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="19064-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19064-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/schema/parseExpression
POST /servicePrincipals/{id}/synchronization/templates/{id}/schema/parseExpression

```
## <a name="request-headers"></a><span data-ttu-id="19064-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19064-120">Request headers</span></span>
| <span data-ttu-id="19064-121">Nome</span><span class="sxs-lookup"><span data-stu-id="19064-121">Name</span></span>       | <span data-ttu-id="19064-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="19064-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="19064-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="19064-123">Authorization</span></span>  | <span data-ttu-id="19064-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="19064-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="19064-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19064-125">Request body</span></span>
<span data-ttu-id="19064-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="19064-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="19064-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="19064-127">Parameter</span></span>    | <span data-ttu-id="19064-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="19064-128">Type</span></span>   |<span data-ttu-id="19064-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="19064-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19064-130">expressão</span><span class="sxs-lookup"><span data-stu-id="19064-130">expression</span></span>               |<span data-ttu-id="19064-131">String</span><span class="sxs-lookup"><span data-stu-id="19064-131">String</span></span>               |<span data-ttu-id="19064-132">Expressão para analisar.</span><span class="sxs-lookup"><span data-stu-id="19064-132">Expression to parse.</span></span>|
|<span data-ttu-id="19064-133">testInputObject</span><span class="sxs-lookup"><span data-stu-id="19064-133">testInputObject</span></span>          |[<span data-ttu-id="19064-134">expressionInputObject</span><span class="sxs-lookup"><span data-stu-id="19064-134">expressionInputObject</span></span>](../resources/synchronization-expressioninputobject.md)|<span data-ttu-id="19064-135">Objeto de dados de teste para avaliar a expressão contra.</span><span class="sxs-lookup"><span data-stu-id="19064-135">Test data object to evaluate expression against.</span></span> <span data-ttu-id="19064-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="19064-136">Optional.</span></span>|
|<span data-ttu-id="19064-137">targetAttributeDefinition</span><span class="sxs-lookup"><span data-stu-id="19064-137">targetAttributeDefinition</span></span>|[<span data-ttu-id="19064-138">attributeDefinition</span><span class="sxs-lookup"><span data-stu-id="19064-138">attributeDefinition</span></span>](../resources/synchronization-attributedefinition.md) |<span data-ttu-id="19064-139">Definição do atributo que será mapeada para esta expressão.</span><span class="sxs-lookup"><span data-stu-id="19064-139">Definition of the attribute that will be mapped to this expression.</span></span> <span data-ttu-id="19064-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="19064-140">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="19064-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="19064-141">Response</span></span>
<span data-ttu-id="19064-142">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [parseExpressionResponse](../resources/synchronization-parseexpressionresponse.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19064-142">If successful, this method returns a `200 OK` response code and a [parseExpressionResponse](../resources/synchronization-parseexpressionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19064-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="19064-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="19064-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19064-144">Request</span></span>
<span data-ttu-id="19064-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="19064-145">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="19064-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="19064-146">Response</span></span>
<span data-ttu-id="19064-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="19064-147">The following is an example of the response.</span></span> 

><span data-ttu-id="19064-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="19064-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSchema: parseExpression",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->