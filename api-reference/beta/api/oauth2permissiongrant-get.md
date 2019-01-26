---
title: Obter oAuth2Permissiongrant
description: Recupere as propriedades e relações do objeto oAuth2Permissiongrant.
localization_priority: Normal
ms.openlocfilehash: 17719e175e29bbc7167fd295fb982a37f22ada52
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576693"
---
# <a name="get-oauth2permissiongrant"></a><span data-ttu-id="d7c55-103">Obter oAuth2Permissiongrant</span><span class="sxs-lookup"><span data-stu-id="d7c55-103">Get oAuth2Permissiongrant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7c55-104">Recupere as propriedades e relações do objeto oAuth2Permissiongrant.</span><span class="sxs-lookup"><span data-stu-id="d7c55-104">Retrieve the properties and relationships of oAuth2Permissiongrant object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7c55-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d7c55-105">Permissions</span></span>
<span data-ttu-id="d7c55-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7c55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d7c55-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7c55-108">Permission type</span></span>      | <span data-ttu-id="d7c55-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d7c55-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7c55-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7c55-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d7c55-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d7c55-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d7c55-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d7c55-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7c55-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7c55-113">Not supported.</span></span>    |
|<span data-ttu-id="d7c55-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7c55-114">Application</span></span> | <span data-ttu-id="d7c55-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7c55-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7c55-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7c55-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /oAuth2Permissiongrants/{id}
GET /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
GET /drive/root/createdByUser/oAuth2Permissiongrants/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d7c55-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d7c55-117">Optional query parameters</span></span>
<span data-ttu-id="d7c55-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d7c55-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d7c55-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7c55-119">Request headers</span></span>
| <span data-ttu-id="d7c55-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d7c55-120">Name</span></span>       | <span data-ttu-id="d7c55-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7c55-121">Type</span></span> | <span data-ttu-id="d7c55-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7c55-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d7c55-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7c55-123">Authorization</span></span>  | <span data-ttu-id="d7c55-124">string</span><span class="sxs-lookup"><span data-stu-id="d7c55-124">string</span></span>  | <span data-ttu-id="d7c55-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7c55-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7c55-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7c55-127">Request body</span></span>
<span data-ttu-id="d7c55-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d7c55-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7c55-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7c55-129">Response</span></span>

<span data-ttu-id="d7c55-130">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7c55-130">If successful, this method returns a `200 OK` response code and [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d7c55-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d7c55-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d7c55-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7c55-132">Request</span></span>
<span data-ttu-id="d7c55-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7c55-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_oAuth2Permissiongrant"
}-->
```http
GET https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
```
##### <a name="response"></a><span data-ttu-id="d7c55-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7c55-134">Response</span></span>
<span data-ttu-id="d7c55-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d7c55-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 200

{
  "clientId": "clientId-value",
  "consentType": "consentType-value",
  "expiryTime": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "principalId": "principalId-value",
  "resourceId": "resourceId-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get oAuth2Permissiongrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/oauth2permissiongrant-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
