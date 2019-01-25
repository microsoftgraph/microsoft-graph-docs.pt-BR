---
title: Lista oauth2PermissionGrants
description: Recupere uma lista de objetos oauth2PermissionGrant.
localization_priority: Normal
ms.openlocfilehash: 9af84b4af64466658058259a665d426484511526
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525826"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="0438f-103">Lista oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="0438f-103">List oauth2PermissionGrants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0438f-104">Recupere uma lista de objetos oauth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="0438f-104">Retrieve a list of oauth2PermissionGrant objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="0438f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0438f-105">Permissions</span></span>

<span data-ttu-id="0438f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0438f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0438f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0438f-108">Permission type</span></span>      | <span data-ttu-id="0438f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0438f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0438f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0438f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0438f-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0438f-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0438f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0438f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0438f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0438f-113">Not supported.</span></span>    |
|<span data-ttu-id="0438f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0438f-114">Application</span></span> | <span data-ttu-id="0438f-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0438f-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0438f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0438f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /oauth2PermissionGrants
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0438f-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0438f-117">Optional query parameters</span></span>
<span data-ttu-id="0438f-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0438f-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0438f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0438f-119">Request headers</span></span>
| <span data-ttu-id="0438f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="0438f-120">Name</span></span> | <span data-ttu-id="0438f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0438f-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="0438f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0438f-122">Authorization</span></span>  | <span data-ttu-id="0438f-123">string</span><span class="sxs-lookup"><span data-stu-id="0438f-123">string</span></span>  | <span data-ttu-id="0438f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0438f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0438f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0438f-126">Request body</span></span>
<span data-ttu-id="0438f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0438f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0438f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0438f-128">Response</span></span>

<span data-ttu-id="0438f-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0438f-129">If successful, this method returns a `200 OK` response code and collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0438f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0438f-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0438f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0438f-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_oauth2permissiongrants"
}-->
```http
GET https://graph.microsoft.com/beta/oauth2PermissionGrants
```
##### <a name="response"></a><span data-ttu-id="0438f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0438f-132">Response</span></span>

<span data-ttu-id="0438f-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0438f-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2Permissiongrant",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 259

{
  "value": [
    {
      "clientId": "clientId-value",
      "consentType": "consentType-value",
      "expiryTime": "datetime-value",
      "id": "id-value",
      "principalId": "principalId-value",
      "resourceId": "resourceId-value",
      "scope": "scope-value",
      "startTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List oauth2PermissionGrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/oauth2permissiongrant-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
