---
title: Listar aplicativos
description: Recupere uma lista de objetos de aplicativo associados ao objeto Connector.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 546bc83891aa81d5c687906275df5d5a05bdd8bb
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2020
ms.locfileid: "44555762"
---
# <a name="list-applications-assigned-to-a-connectorgroup"></a><span data-ttu-id="e3eca-103">Listar aplicativos atribuídos a um conector</span><span class="sxs-lookup"><span data-stu-id="e3eca-103">List applications assigned to a connectorGroup</span></span>

<span data-ttu-id="e3eca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3eca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3eca-105">Recupere uma lista de objetos de [aplicativo](../resources/application.md) associados ao objeto [Connector](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="e3eca-105">Retrieve a list of [application](../resources/application.md) objects associated with the [connectorGroup](../resources/connectorgroup.md).</span></span> <span data-ttu-id="e3eca-106">Esta lista contém todos os aplicativos atribuídos ao grupo de conectores específico.</span><span class="sxs-lookup"><span data-stu-id="e3eca-106">This list contains all applications assigned to the specific connector group.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3eca-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e3eca-107">Permissions</span></span>
<span data-ttu-id="e3eca-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3eca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3eca-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3eca-110">Permission type</span></span>      | <span data-ttu-id="e3eca-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e3eca-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3eca-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3eca-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e3eca-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e3eca-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e3eca-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3eca-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3eca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3eca-115">Not supported.</span></span>    |
|<span data-ttu-id="e3eca-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3eca-116">Application</span></span> | <span data-ttu-id="e3eca-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3eca-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3eca-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3eca-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e3eca-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e3eca-119">Optional query parameters</span></span>
<span data-ttu-id="e3eca-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e3eca-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3eca-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3eca-121">Request headers</span></span>
| <span data-ttu-id="e3eca-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e3eca-122">Name</span></span>      |<span data-ttu-id="e3eca-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3eca-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e3eca-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3eca-124">Authorization</span></span>  | <span data-ttu-id="e3eca-125">Portador.</span><span class="sxs-lookup"><span data-stu-id="e3eca-125">Bearer.</span></span> <span data-ttu-id="e3eca-126">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="e3eca-126">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3eca-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3eca-127">Request body</span></span>
<span data-ttu-id="e3eca-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e3eca-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3eca-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3eca-129">Response</span></span>

<span data-ttu-id="e3eca-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [Application](../resources/application.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3eca-130">If successful, this method returns a `200 OK` response code and collection of [application](../resources/application.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3eca-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3eca-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3eca-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3eca-132">Request</span></span>
<span data-ttu-id="e3eca-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3eca-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_applications"
}-->
```http
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/applications
```
##### <a name="response"></a><span data-ttu-id="e3eca-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3eca-134">Response</span></span>
<span data-ttu-id="e3eca-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e3eca-135">The following is an example of the response.</span></span> <span data-ttu-id="e3eca-136">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="e3eca-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e3eca-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3eca-137">All of the properties will be returned from an actual call.</span></span>
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
