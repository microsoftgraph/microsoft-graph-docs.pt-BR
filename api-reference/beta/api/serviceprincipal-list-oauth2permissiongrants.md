---
title: 'servicePrincipalName: listar oAuth2Permissiongrants'
description: Recupere uma lista de objetos oAuth2Permissiongrant.
localization_priority: Normal
ms.openlocfilehash: 34f769f5bd194458689914dd608583c69bbe2076
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537528"
---
# <a name="serviceprincipal-list-oauth2permissiongrants"></a><span data-ttu-id="8ff42-103">servicePrincipalName: listar oAuth2Permissiongrants</span><span class="sxs-lookup"><span data-stu-id="8ff42-103">servicePrincipal: List oAuth2Permissiongrants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ff42-104">Recupere uma lista de objetos oAuth2Permissiongrant.</span><span class="sxs-lookup"><span data-stu-id="8ff42-104">Retrieve a list of oAuth2Permissiongrant objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ff42-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8ff42-105">Permissions</span></span>
<span data-ttu-id="8ff42-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ff42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ff42-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ff42-108">Permission type</span></span>      | <span data-ttu-id="8ff42-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8ff42-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ff42-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ff42-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8ff42-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8ff42-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8ff42-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ff42-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ff42-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ff42-113">Not supported.</span></span>    |
|<span data-ttu-id="8ff42-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ff42-114">Application</span></span> | <span data-ttu-id="8ff42-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ff42-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ff42-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ff42-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/oAuth2Permissiongrants
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8ff42-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8ff42-117">Optional query parameters</span></span>
<span data-ttu-id="8ff42-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8ff42-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8ff42-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ff42-119">Request headers</span></span>
| <span data-ttu-id="8ff42-120">Nome</span><span class="sxs-lookup"><span data-stu-id="8ff42-120">Name</span></span>       | <span data-ttu-id="8ff42-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ff42-121">Type</span></span> | <span data-ttu-id="8ff42-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ff42-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8ff42-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ff42-123">Authorization</span></span>  | <span data-ttu-id="8ff42-124">string</span><span class="sxs-lookup"><span data-stu-id="8ff42-124">string</span></span>  | <span data-ttu-id="8ff42-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ff42-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ff42-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ff42-127">Request body</span></span>
<span data-ttu-id="8ff42-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8ff42-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ff42-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ff42-129">Response</span></span>

<span data-ttu-id="8ff42-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ff42-130">If successful, this method returns a `200 OK` response code and collection of [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8ff42-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ff42-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8ff42-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ff42-132">Request</span></span>
<span data-ttu-id="8ff42-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ff42-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_oAuth2Permissiongrants"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/oAuth2Permissiongrants
```
##### <a name="response"></a><span data-ttu-id="8ff42-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ff42-134">Response</span></span>
<span data-ttu-id="8ff42-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8ff42-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2Permissiongrant",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 253

{
  "value": [
    {
      "clientId": "clientId-value",
      "consentType": "consentType-value",
      "expiryTime": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "principalId": "principalId-value",
      "resourceId": "resourceId-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List oAuth2Permissiongrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-list-oauth2permissiongrants.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
