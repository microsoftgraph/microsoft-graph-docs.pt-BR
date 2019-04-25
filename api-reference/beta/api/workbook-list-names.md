---
title: Listar nomes
description: Recupere uma lista de objetos nameditem.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: da13ae0734c5508c1eb2db2bb5874a52957c27db
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536450"
---
# <a name="list-names"></a><span data-ttu-id="578e5-103">Listar nomes</span><span class="sxs-lookup"><span data-stu-id="578e5-103">List names</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="578e5-104">Recupere uma lista de objetos nameditem.</span><span class="sxs-lookup"><span data-stu-id="578e5-104">Retrieve a list of nameditem objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="578e5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="578e5-105">Permissions</span></span>
<span data-ttu-id="578e5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="578e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="578e5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="578e5-108">Permission type</span></span>      | <span data-ttu-id="578e5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="578e5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="578e5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="578e5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="578e5-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="578e5-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="578e5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="578e5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="578e5-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="578e5-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="578e5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="578e5-114">Application</span></span> | <span data-ttu-id="578e5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="578e5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="578e5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="578e5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names
```
## <a name="optional-query-parameters"></a><span data-ttu-id="578e5-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="578e5-117">Optional query parameters</span></span>
<span data-ttu-id="578e5-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="578e5-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="578e5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="578e5-119">Request headers</span></span>
| <span data-ttu-id="578e5-120">Nome</span><span class="sxs-lookup"><span data-stu-id="578e5-120">Name</span></span>      |<span data-ttu-id="578e5-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="578e5-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="578e5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="578e5-122">Authorization</span></span>  | <span data-ttu-id="578e5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="578e5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="578e5-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="578e5-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="578e5-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="578e5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="578e5-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="578e5-128">Request body</span></span>
<span data-ttu-id="578e5-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="578e5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="578e5-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="578e5-130">Response</span></span>

<span data-ttu-id="578e5-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [NamedItem](../resources/nameditem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="578e5-131">If successful, this method returns a `200 OK` response code and collection of [NamedItem](../resources/nameditem.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="578e5-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="578e5-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="578e5-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="578e5-133">Request</span></span>
<span data-ttu-id="578e5-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="578e5-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_names"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names
```
##### <a name="response"></a><span data-ttu-id="578e5-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="578e5-135">Response</span></span>
<span data-ttu-id="578e5-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="578e5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "value": [
    {
      "name": "name-value",
      "type": "type-value",
      "value": {
      },
      "visible": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List names",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/workbook-list-names.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
