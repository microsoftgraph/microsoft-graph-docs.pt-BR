---
title: Listar Administrativeunits dos quais
description: Recupere uma lista de objetos administrativeUnit.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 603af0d7a2e4f9e1ffe5e29d4485db2e99686ddc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459273"
---
# <a name="list-administrativeunits"></a><span data-ttu-id="aff3a-103">Listar Administrativeunits dos quais</span><span class="sxs-lookup"><span data-stu-id="aff3a-103">List administrativeUnits</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aff3a-104">Recupere uma lista de objetos [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="aff3a-104">Retrieve a list of [administrativeUnit](../resources/administrativeunit.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="aff3a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="aff3a-105">Permissions</span></span>
<span data-ttu-id="aff3a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aff3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="aff3a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aff3a-108">Permission type</span></span>      | <span data-ttu-id="aff3a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aff3a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aff3a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aff3a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="aff3a-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aff3a-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="aff3a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aff3a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aff3a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aff3a-113">Not supported.</span></span>    |
|<span data-ttu-id="aff3a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aff3a-114">Application</span></span> | <span data-ttu-id="aff3a-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aff3a-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aff3a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aff3a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits
```
## <a name="optional-query-parameters"></a><span data-ttu-id="aff3a-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="aff3a-117">Optional query parameters</span></span>
<span data-ttu-id="aff3a-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="aff3a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aff3a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aff3a-119">Request headers</span></span>
| <span data-ttu-id="aff3a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="aff3a-120">Name</span></span>      |<span data-ttu-id="aff3a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="aff3a-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="aff3a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="aff3a-122">Authorization</span></span>  | <span data-ttu-id="aff3a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aff3a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aff3a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aff3a-125">Request body</span></span>
<span data-ttu-id="aff3a-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aff3a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aff3a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="aff3a-127">Response</span></span>

<span data-ttu-id="aff3a-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [administrativeUnit](../resources/administrativeunit.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aff3a-128">If successful, this method returns a `200 OK` response code and collection of [administrativeUnit](../resources/administrativeunit.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aff3a-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aff3a-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aff3a-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aff3a-130">Request</span></span>
<span data-ttu-id="aff3a-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aff3a-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_administrativeunits"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits
```
##### <a name="response"></a><span data-ttu-id="aff3a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="aff3a-132">Response</span></span>
<span data-ttu-id="aff3a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aff3a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "value": [
    {
      "displayName": "displayName-value",
      "description": "description-value",
      "visibility": "visibility-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List administrativeUnits",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
