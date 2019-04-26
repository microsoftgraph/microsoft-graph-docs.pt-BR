---
title: List oauth2PermissionGrants
description: Recupere uma lista de objetos oauth2PermissionGrant.
localization_priority: Normal
ms.openlocfilehash: 6f2a9660b740772caa46992764b905f90736c905
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333046"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="e9012-103">List oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="e9012-103">List oauth2PermissionGrants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9012-104">Recupere uma lista de objetos oauth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="e9012-104">Retrieve a list of oauth2PermissionGrant objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9012-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e9012-105">Permissions</span></span>

<span data-ttu-id="e9012-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9012-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e9012-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9012-108">Permission type</span></span>      | <span data-ttu-id="e9012-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e9012-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9012-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9012-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e9012-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e9012-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e9012-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9012-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9012-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9012-113">Not supported.</span></span>    |
|<span data-ttu-id="e9012-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9012-114">Application</span></span> | <span data-ttu-id="e9012-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9012-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9012-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9012-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /oauth2PermissionGrants
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e9012-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e9012-117">Optional query parameters</span></span>
<span data-ttu-id="e9012-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e9012-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9012-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9012-119">Request headers</span></span>
| <span data-ttu-id="e9012-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e9012-120">Name</span></span> | <span data-ttu-id="e9012-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9012-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="e9012-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9012-122">Authorization</span></span>  | <span data-ttu-id="e9012-123">string</span><span class="sxs-lookup"><span data-stu-id="e9012-123">string</span></span>  | <span data-ttu-id="e9012-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9012-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9012-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9012-126">Request body</span></span>
<span data-ttu-id="e9012-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e9012-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9012-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9012-128">Response</span></span>

<span data-ttu-id="e9012-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9012-129">If successful, this method returns a `200 OK` response code and collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e9012-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9012-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e9012-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9012-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_oauth2permissiongrants"
}-->
```http
GET https://graph.microsoft.com/beta/oauth2PermissionGrants
```
##### <a name="response"></a><span data-ttu-id="e9012-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9012-132">Response</span></span>

<span data-ttu-id="e9012-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e9012-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
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
  "suppressions": []
}
-->
