---
title: Obter oAuth2Permissiongrant
description: Recupere as propriedades e os relacionamentos do objeto oAuth2Permissiongrant.
localization_priority: Normal
ms.openlocfilehash: 2b389e7f811444b9dc9fb1d9c2f619006611e11e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32540153"
---
# <a name="get-oauth2permissiongrant"></a><span data-ttu-id="c95ad-103">Obter oAuth2Permissiongrant</span><span class="sxs-lookup"><span data-stu-id="c95ad-103">Get oAuth2Permissiongrant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c95ad-104">Recupere as propriedades e os relacionamentos do objeto oAuth2Permissiongrant.</span><span class="sxs-lookup"><span data-stu-id="c95ad-104">Retrieve the properties and relationships of oAuth2Permissiongrant object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c95ad-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c95ad-105">Permissions</span></span>
<span data-ttu-id="c95ad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c95ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c95ad-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c95ad-108">Permission type</span></span>      | <span data-ttu-id="c95ad-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c95ad-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c95ad-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c95ad-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c95ad-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c95ad-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c95ad-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c95ad-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c95ad-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c95ad-113">Not supported.</span></span>    |
|<span data-ttu-id="c95ad-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c95ad-114">Application</span></span> | <span data-ttu-id="c95ad-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c95ad-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c95ad-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c95ad-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /oAuth2Permissiongrants/{id}
GET /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
GET /drive/root/createdByUser/oAuth2Permissiongrants/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c95ad-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c95ad-117">Optional query parameters</span></span>
<span data-ttu-id="c95ad-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c95ad-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c95ad-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c95ad-119">Request headers</span></span>
| <span data-ttu-id="c95ad-120">Nome</span><span class="sxs-lookup"><span data-stu-id="c95ad-120">Name</span></span>       | <span data-ttu-id="c95ad-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="c95ad-121">Type</span></span> | <span data-ttu-id="c95ad-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c95ad-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c95ad-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c95ad-123">Authorization</span></span>  | <span data-ttu-id="c95ad-124">string</span><span class="sxs-lookup"><span data-stu-id="c95ad-124">string</span></span>  | <span data-ttu-id="c95ad-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c95ad-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c95ad-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c95ad-127">Request body</span></span>
<span data-ttu-id="c95ad-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c95ad-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c95ad-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c95ad-129">Response</span></span>

<span data-ttu-id="c95ad-130">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c95ad-130">If successful, this method returns a `200 OK` response code and [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c95ad-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c95ad-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c95ad-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c95ad-132">Request</span></span>
<span data-ttu-id="c95ad-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c95ad-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_oAuth2Permissiongrant"
}-->
```http
GET https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
```
##### <a name="response"></a><span data-ttu-id="c95ad-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c95ad-134">Response</span></span>
<span data-ttu-id="c95ad-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c95ad-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2Permissiongrant"
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
