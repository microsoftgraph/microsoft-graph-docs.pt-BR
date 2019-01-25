---
title: Obter administrativeUnit
description: Recupere as propriedades e relacionamentos de um objeto administrativeUnit.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 588d116d546503fa8db6c8ba56c5d0e328a10b8a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521604"
---
# <a name="get-administrativeunit"></a><span data-ttu-id="1e67c-103">Obter administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="1e67c-103">Get administrativeUnit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e67c-104">Recupere as propriedades e relacionamentos de um objeto [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="1e67c-104">Retrieve the properties and relationships of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="1e67c-105">Desde que o recurso de **administrativeUnit** oferece suporte às [extensões](/graph/extensibility-overview), você também pode usar o `GET` operação obter dados de extensão e propriedades personalizadas em uma instância de **administrativeUnit** .</span><span class="sxs-lookup"><span data-stu-id="1e67c-105">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **administrativeUnit** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e67c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1e67c-106">Permissions</span></span>
<span data-ttu-id="1e67c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e67c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1e67c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e67c-109">Permission type</span></span>      | <span data-ttu-id="1e67c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1e67c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e67c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e67c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1e67c-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1e67c-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1e67c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e67c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e67c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e67c-114">Not supported.</span></span>    |
|<span data-ttu-id="1e67c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e67c-115">Application</span></span> | <span data-ttu-id="1e67c-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e67c-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e67c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e67c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1e67c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1e67c-118">Optional query parameters</span></span>
<span data-ttu-id="1e67c-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1e67c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1e67c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e67c-120">Request headers</span></span>
| <span data-ttu-id="1e67c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="1e67c-121">Name</span></span>      |<span data-ttu-id="1e67c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e67c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1e67c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e67c-123">Authorization</span></span>  | <span data-ttu-id="1e67c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e67c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e67c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e67c-126">Request body</span></span>
<span data-ttu-id="1e67c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1e67c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e67c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e67c-128">Response</span></span>

<span data-ttu-id="1e67c-129">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [administrativeUnit](../resources/administrativeunit.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e67c-129">If successful, this method returns a `200 OK` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1e67c-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e67c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1e67c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e67c-131">Request</span></span>
<span data-ttu-id="1e67c-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e67c-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_administrativeunit"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}
```
##### <a name="response"></a><span data-ttu-id="1e67c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e67c-133">Response</span></span>
<span data-ttu-id="1e67c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1e67c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "displayName": "displayName-value",
  "description": "description-value",
  "visibility": "visibility-value",
  "id": "id-value"
}
```

## <a name="see-also"></a><span data-ttu-id="1e67c-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="1e67c-137">See also</span></span>

- [<span data-ttu-id="1e67c-138">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="1e67c-138">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="1e67c-139">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="1e67c-139">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
