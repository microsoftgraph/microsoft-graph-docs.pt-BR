---
title: 'servicePrincipalName: listar oAuth2Permissiongrants'
description: Recupere uma lista de objetos oAuth2Permissiongrant.
localization_priority: Normal
ms.openlocfilehash: e136724287db1d2c8b4d49a882a2871fb551b2fa
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331416"
---
# <a name="serviceprincipal-list-oauth2permissiongrants"></a><span data-ttu-id="fb18b-103">servicePrincipalName: listar oAuth2Permissiongrants</span><span class="sxs-lookup"><span data-stu-id="fb18b-103">servicePrincipal: List oAuth2Permissiongrants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb18b-104">Recupere uma lista de objetos oAuth2Permissiongrant.</span><span class="sxs-lookup"><span data-stu-id="fb18b-104">Retrieve a list of oAuth2Permissiongrant objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb18b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="fb18b-105">Permissions</span></span>
<span data-ttu-id="fb18b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb18b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb18b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb18b-108">Permission type</span></span>      | <span data-ttu-id="fb18b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fb18b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb18b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb18b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fb18b-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fb18b-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fb18b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb18b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb18b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb18b-113">Not supported.</span></span>    |
|<span data-ttu-id="fb18b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb18b-114">Application</span></span> | <span data-ttu-id="fb18b-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb18b-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb18b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb18b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/oAuth2Permissiongrants
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fb18b-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fb18b-117">Optional query parameters</span></span>
<span data-ttu-id="fb18b-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fb18b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fb18b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb18b-119">Request headers</span></span>
| <span data-ttu-id="fb18b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="fb18b-120">Name</span></span>       | <span data-ttu-id="fb18b-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb18b-121">Type</span></span> | <span data-ttu-id="fb18b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb18b-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fb18b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb18b-123">Authorization</span></span>  | <span data-ttu-id="fb18b-124">string</span><span class="sxs-lookup"><span data-stu-id="fb18b-124">string</span></span>  | <span data-ttu-id="fb18b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb18b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fb18b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb18b-127">Request body</span></span>
<span data-ttu-id="fb18b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fb18b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb18b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb18b-129">Response</span></span>

<span data-ttu-id="fb18b-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb18b-130">If successful, this method returns a `200 OK` response code and collection of [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fb18b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fb18b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fb18b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb18b-132">Request</span></span>
<span data-ttu-id="fb18b-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fb18b-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_oAuth2Permissiongrants"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/oAuth2Permissiongrants
```
##### <a name="response"></a><span data-ttu-id="fb18b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb18b-134">Response</span></span>
<span data-ttu-id="fb18b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fb18b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
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
  "suppressions": []
}
-->
