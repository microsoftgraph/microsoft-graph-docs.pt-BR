---
title: Listar membros
description: Recupere uma lista de objetos de conector associados a um connectorGroup.
localization_priority: Normal
ms.openlocfilehash: 0a35e2645d017d6c0ff23121a5f592438e575798
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517054"
---
# <a name="list-members"></a><span data-ttu-id="dc9f4-103">Listar membros</span><span class="sxs-lookup"><span data-stu-id="dc9f4-103">List members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc9f4-104">Recupere uma lista de objetos de conector associados a um connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="dc9f4-104">Retrieve a list of connector objects associated with a connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="dc9f4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="dc9f4-105">Permissions</span></span>
<span data-ttu-id="dc9f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc9f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc9f4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc9f4-108">Permission type</span></span>      | <span data-ttu-id="dc9f4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dc9f4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc9f4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc9f4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dc9f4-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dc9f4-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dc9f4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc9f4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc9f4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc9f4-113">Not supported.</span></span>    |
|<span data-ttu-id="dc9f4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc9f4-114">Application</span></span> | <span data-ttu-id="dc9f4-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc9f4-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc9f4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc9f4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectorGroups/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dc9f4-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dc9f4-117">Optional query parameters</span></span>
<span data-ttu-id="dc9f4-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dc9f4-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dc9f4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc9f4-119">Request headers</span></span>
| <span data-ttu-id="dc9f4-120">Nome</span><span class="sxs-lookup"><span data-stu-id="dc9f4-120">Name</span></span>      |<span data-ttu-id="dc9f4-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc9f4-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dc9f4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc9f4-122">Authorization</span></span>  | <span data-ttu-id="dc9f4-123"> de portador</span><span class="sxs-lookup"><span data-stu-id="dc9f4-123">Bearer.</span></span> <span data-ttu-id="dc9f4-124">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="dc9f4-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc9f4-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc9f4-125">Request body</span></span>
<span data-ttu-id="dc9f4-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dc9f4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc9f4-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc9f4-127">Response</span></span>

<span data-ttu-id="dc9f4-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos do [conector](../resources/connector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dc9f4-128">If successful, this method returns a `200 OK` response code and collection of [connector](../resources/connector.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dc9f4-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dc9f4-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dc9f4-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc9f4-130">Request</span></span>
<span data-ttu-id="dc9f4-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc9f4-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectorGroups/{id}/members
```
##### <a name="response"></a><span data-ttu-id="dc9f4-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc9f4-132">Response</span></span>
<span data-ttu-id="dc9f4-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dc9f4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "value": [
    {
      "id": "id-value",
      "machineName": "machineName-value",
      "externalIp": "externalIp-value",
      "status": "status-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/connectorgroup-list-members.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
