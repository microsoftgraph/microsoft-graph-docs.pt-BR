---
title: Listar aplicativos
description: Recupere uma lista de objetos de aplicativo associados ao connectorGroup.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 85b9e7eb24d880ea6fe82a7461bfec20594cee97
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047172"
---
# <a name="list-applications-assigned-to-a-connectorgroup"></a><span data-ttu-id="ba9c6-103">Listar aplicativos atribuídos a um connectorGroup</span><span class="sxs-lookup"><span data-stu-id="ba9c6-103">List applications assigned to a connectorGroup</span></span>

<span data-ttu-id="ba9c6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba9c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba9c6-105">Recupere uma lista de [objetos de](../resources/application.md) aplicativo associados ao [connectorGroup](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="ba9c6-105">Retrieve a list of [application](../resources/application.md) objects associated with the [connectorGroup](../resources/connectorgroup.md).</span></span> <span data-ttu-id="ba9c6-106">Esta lista contém todos os aplicativos atribuídos ao grupo de conectores específico.</span><span class="sxs-lookup"><span data-stu-id="ba9c6-106">This list contains all applications assigned to the specific connector group.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba9c6-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ba9c6-107">Permissions</span></span>
<span data-ttu-id="ba9c6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba9c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba9c6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba9c6-110">Permission type</span></span>      | <span data-ttu-id="ba9c6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ba9c6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba9c6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba9c6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ba9c6-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ba9c6-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ba9c6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba9c6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba9c6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba9c6-115">Not supported.</span></span>    |
|<span data-ttu-id="ba9c6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba9c6-116">Application</span></span> | <span data-ttu-id="ba9c6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba9c6-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="ba9c6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba9c6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ba9c6-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ba9c6-119">Optional query parameters</span></span>
<span data-ttu-id="ba9c6-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ba9c6-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ba9c6-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba9c6-121">Request headers</span></span>
| <span data-ttu-id="ba9c6-122">Nome</span><span class="sxs-lookup"><span data-stu-id="ba9c6-122">Name</span></span>      |<span data-ttu-id="ba9c6-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba9c6-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ba9c6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba9c6-124">Authorization</span></span>  | <span data-ttu-id="ba9c6-125">Portador.</span><span class="sxs-lookup"><span data-stu-id="ba9c6-125">Bearer.</span></span> <span data-ttu-id="ba9c6-126">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="ba9c6-126">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba9c6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba9c6-127">Request body</span></span>
<span data-ttu-id="ba9c6-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ba9c6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba9c6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba9c6-129">Response</span></span>

<span data-ttu-id="ba9c6-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [de](../resources/application.md) aplicativo no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba9c6-130">If successful, this method returns a `200 OK` response code and collection of [application](../resources/application.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba9c6-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ba9c6-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ba9c6-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba9c6-132">Request</span></span>
<span data-ttu-id="ba9c6-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba9c6-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ba9c6-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba9c6-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applications"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/applications
```
# <a name="c"></a>[<span data-ttu-id="ba9c6-135">C#</span><span class="sxs-lookup"><span data-stu-id="ba9c6-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ba9c6-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba9c6-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ba9c6-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba9c6-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ba9c6-138">Java</span><span class="sxs-lookup"><span data-stu-id="ba9c6-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-applications-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ba9c6-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba9c6-139">Response</span></span>
<span data-ttu-id="ba9c6-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ba9c6-140">The following is an example of the response.</span></span> <span data-ttu-id="ba9c6-141">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ba9c6-141">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 420

{
  "value": [
    {
      "id": "id-value",
      "onPremisesPublishing": {
        "externalUrl": "externalUrl-value",
        "internalUrl": "internalUrl-value",
        "externalAuthenticationType": "externalAuthenticationType-value",
        "isTranslateHostHeaderEnabled": true,
        "isTranslateLinksInBodyEnabled": true,
        "isOnPremPublishingEnabled": true,
        "applicationServerTimeout": "applicationServerTimeout-value",
        "applicationType": "applicationType-value",
        "verifiedCustomDomainKeyCredential": {
          "customKeyIdentifier": "customKeyIdentifier-value",
          "endDate": "datetime-value",
          "keyId": "keyId-value",
          "startDate": "datetime-value",
          "type": "type-value",
          "usage": "usage-value",
          "value": "value-value"
        },
        "verifiedCustomDomainPasswordCredential": {
          "customKeyIdentifier": "customKeyIdentifier-value",
          "endDate": "datetime-value",
          "keyId": "keyId-value",
          "startDate": "datetime-value",
          "value": "value-value"
        },
        "verifiedCustomDomainCertificatesMetadata": {
          "thumbprint": "thumbprint-value",
          "subjectName": "subjectName-value",
          "issuerName": "issuerName-value",
          "issueDate": "datetime-value",
          "expiryDate": "datetime-value"
        },
        "singleSignOnSettings": {
          "SingleSignOnMode": "SingleSignOnMode-value",
          "KerberosSignOnSettings": {
            "KerberosServicePrincipalName": "KerberosServicePrincipalName-value",
            "KerberosSignOnMappingAttributeType": "KerberosSignOnMappingAttributeType-value"
          }
        },
        "isHttpOnlyCookieEnabled": true,
        "isSecureCookieEnabled": true,
        "isPersistentCookieEnabled": true
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List applications",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

