---
title: Lista privilegedApproval
description: Recupere uma lista de objetos privilegedapproval.
localization_priority: Normal
ms.openlocfilehash: ab3a3c2670cd0ddebf8415e112305679c1d3446c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521548"
---
# <a name="list-privilegedapproval"></a><span data-ttu-id="895c7-103">Lista privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="895c7-103">List privilegedApproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="895c7-104">Recupere uma lista de objetos privilegedapproval.</span><span class="sxs-lookup"><span data-stu-id="895c7-104">Retrieve a list of privilegedapproval objects.</span></span>

<span data-ttu-id="895c7-105">Para filtrar os resultados da consulta, use o OData standard ``$filter`` expressões nos URIs.</span><span class="sxs-lookup"><span data-stu-id="895c7-105">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="895c7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="895c7-106">Permissions</span></span>
<span data-ttu-id="895c7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="895c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="895c7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="895c7-109">Permission type</span></span>      | <span data-ttu-id="895c7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="895c7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="895c7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="895c7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="895c7-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="895c7-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="895c7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="895c7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="895c7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="895c7-114">Not supported.</span></span>    |
|<span data-ttu-id="895c7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="895c7-115">Application</span></span> | <span data-ttu-id="895c7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="895c7-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="895c7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="895c7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval
```
## <a name="optional-query-parameters"></a><span data-ttu-id="895c7-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="895c7-118">Optional query parameters</span></span>
<span data-ttu-id="895c7-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="895c7-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="895c7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="895c7-120">Request headers</span></span>
| <span data-ttu-id="895c7-121">Nome</span><span class="sxs-lookup"><span data-stu-id="895c7-121">Name</span></span>      |<span data-ttu-id="895c7-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="895c7-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="895c7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="895c7-123">Authorization</span></span>  | <span data-ttu-id="895c7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="895c7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="895c7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="895c7-126">Request body</span></span>
<span data-ttu-id="895c7-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="895c7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="895c7-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="895c7-128">Response</span></span>

<span data-ttu-id="895c7-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [privilegedApproval](../resources/privilegedapproval.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="895c7-129">If successful, this method returns a `200 OK` response code and collection of [privilegedApproval](../resources/privilegedapproval.md) objects in the response body.</span></span>

<span data-ttu-id="895c7-130">Observe que o inquilino deve ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="895c7-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="895c7-131">Caso contrário, será retornado o código de status HTTP 403-Proibido.</span><span class="sxs-lookup"><span data-stu-id="895c7-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="895c7-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="895c7-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="895c7-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="895c7-133">Request</span></span>
<span data-ttu-id="895c7-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="895c7-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval
```
##### <a name="response"></a><span data-ttu-id="895c7-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="895c7-135">Response</span></span>
<span data-ttu-id="895c7-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="895c7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 246

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "approvalType": "approvalType-value",
      "approvalState": "approvalState-value",
      "approvalDuration": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedapproval-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
