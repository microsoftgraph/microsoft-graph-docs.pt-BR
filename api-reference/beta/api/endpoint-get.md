---
title: Obter o ponto de extremidade
description: Recupere as propriedades e relacionamentos de um objeto de ponto de extremidade específico.
localization_priority: Normal
ms.openlocfilehash: 7c5b7bd28b06e20dbc92b09ff961214828749999
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640424"
---
# <a name="get-endpoint"></a><span data-ttu-id="f1d36-103">Obter o ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="f1d36-103">Get endpoint</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1d36-104">Recupere as propriedades e relacionamentos de um objeto específico de [ponto de extremidade](../resources/endpoint.md) .</span><span class="sxs-lookup"><span data-stu-id="f1d36-104">Retrieve the properties and relationships of a specific [endpoint](../resources/endpoint.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1d36-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f1d36-105">Permissions</span></span>
<span data-ttu-id="f1d36-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1d36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f1d36-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1d36-108">Permission type</span></span>      | <span data-ttu-id="f1d36-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1d36-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1d36-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1d36-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f1d36-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1d36-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f1d36-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1d36-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1d36-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1d36-113">Not supported.</span></span>    |
|<span data-ttu-id="f1d36-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1d36-114">Application</span></span> | <span data-ttu-id="f1d36-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1d36-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1d36-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1d36-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f1d36-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f1d36-117">Optional query parameters</span></span>
<span data-ttu-id="f1d36-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f1d36-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f1d36-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1d36-119">Request headers</span></span>
| <span data-ttu-id="f1d36-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f1d36-120">Name</span></span>      |<span data-ttu-id="f1d36-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1d36-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f1d36-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1d36-122">Authorization</span></span>  | <span data-ttu-id="f1d36-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1d36-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="f1d36-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f1d36-125">Content-Type</span></span>   | <span data-ttu-id="f1d36-126">Application/Json</span><span class="sxs-lookup"><span data-stu-id="f1d36-126">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1d36-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1d36-127">Request body</span></span>
<span data-ttu-id="f1d36-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f1d36-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1d36-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1d36-129">Response</span></span>

<span data-ttu-id="f1d36-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto de [ponto de extremidade](../resources/endpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1d36-130">If successful, this method returns a `200 OK` response code and [Endpoint](../resources/endpoint.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f1d36-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1d36-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1d36-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1d36-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_endpoint"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/endpoints/{id}
```
##### <a name="response"></a><span data-ttu-id="f1d36-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1d36-133">Response</span></span>
<span data-ttu-id="f1d36-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1d36-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Endpoint"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 208

{
  "capability": "Conversations",
  "providerId": "{Yammer GUID}",
  "providerName": "Yammer",
  "uri": "uri-value",
  "providerResourceId": "Yammer.FeedURL",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Endpoint",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/endpoint-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
