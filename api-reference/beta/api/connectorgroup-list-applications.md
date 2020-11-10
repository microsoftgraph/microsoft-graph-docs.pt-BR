---
title: Listar aplicativos
description: Recupere uma lista de objetos de aplicativo associados ao objeto Connector.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a4c0dee137cc721cba180784e4f8d36a795a01aa
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957397"
---
# <a name="list-applications-assigned-to-a-connectorgroup"></a><span data-ttu-id="e3adc-103">Listar aplicativos atribuídos a um conector</span><span class="sxs-lookup"><span data-stu-id="e3adc-103">List applications assigned to a connectorGroup</span></span>

<span data-ttu-id="e3adc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3adc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3adc-105">Recupere uma lista de objetos de [aplicativo](../resources/application.md) associados ao objeto [Connector](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="e3adc-105">Retrieve a list of [application](../resources/application.md) objects associated with the [connectorGroup](../resources/connectorgroup.md).</span></span> <span data-ttu-id="e3adc-106">Esta lista contém todos os aplicativos atribuídos ao grupo de conectores específico.</span><span class="sxs-lookup"><span data-stu-id="e3adc-106">This list contains all applications assigned to the specific connector group.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3adc-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e3adc-107">Permissions</span></span>
<span data-ttu-id="e3adc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3adc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3adc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3adc-110">Permission type</span></span>      | <span data-ttu-id="e3adc-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e3adc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3adc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3adc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e3adc-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e3adc-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e3adc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3adc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3adc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3adc-115">Not supported.</span></span>    |
|<span data-ttu-id="e3adc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3adc-116">Application</span></span> | <span data-ttu-id="e3adc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3adc-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="e3adc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3adc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e3adc-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e3adc-119">Optional query parameters</span></span>
<span data-ttu-id="e3adc-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e3adc-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3adc-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3adc-121">Request headers</span></span>
| <span data-ttu-id="e3adc-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e3adc-122">Name</span></span>      |<span data-ttu-id="e3adc-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3adc-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e3adc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3adc-124">Authorization</span></span>  | <span data-ttu-id="e3adc-125">Portador.</span><span class="sxs-lookup"><span data-stu-id="e3adc-125">Bearer.</span></span> <span data-ttu-id="e3adc-126">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="e3adc-126">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3adc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3adc-127">Request body</span></span>
<span data-ttu-id="e3adc-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e3adc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3adc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3adc-129">Response</span></span>

<span data-ttu-id="e3adc-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [Application](../resources/application.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3adc-130">If successful, this method returns a `200 OK` response code and collection of [application](../resources/application.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3adc-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3adc-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3adc-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3adc-132">Request</span></span>
<span data-ttu-id="e3adc-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3adc-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e3adc-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3adc-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applications"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/applications
```
# <a name="c"></a>[<span data-ttu-id="e3adc-135">C#</span><span class="sxs-lookup"><span data-stu-id="e3adc-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e3adc-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3adc-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e3adc-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3adc-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e3adc-138">Java</span><span class="sxs-lookup"><span data-stu-id="e3adc-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-applications-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e3adc-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3adc-139">Response</span></span>
<span data-ttu-id="e3adc-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e3adc-140">The following is an example of the response.</span></span> <span data-ttu-id="e3adc-141">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="e3adc-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e3adc-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3adc-142">All of the properties will be returned from an actual call.</span></span>
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
