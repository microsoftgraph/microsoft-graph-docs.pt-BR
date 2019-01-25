---
title: Obter privilegedApproval
description: Recupere as propriedades e relações do objeto privilegedapproval.
localization_priority: Normal
ms.openlocfilehash: c718c8d3c9382c5f8af9debf88fd6de5a55b461b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513617"
---
# <a name="get-privilegedapproval"></a><span data-ttu-id="ea488-103">Obter privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="ea488-103">Get privilegedApproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea488-104">Recupere as propriedades e relações do objeto privilegedapproval.</span><span class="sxs-lookup"><span data-stu-id="ea488-104">Retrieve the properties and relationships of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ea488-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ea488-105">Permissions</span></span>
<span data-ttu-id="ea488-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea488-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ea488-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ea488-108">Permission type</span></span>      | <span data-ttu-id="ea488-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ea488-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea488-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ea488-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ea488-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ea488-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="ea488-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ea488-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea488-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea488-113">Not supported.</span></span>    |
|<span data-ttu-id="ea488-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ea488-114">Application</span></span> | <span data-ttu-id="ea488-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea488-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea488-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ea488-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ea488-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ea488-117">Optional query parameters</span></span>
<span data-ttu-id="ea488-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ea488-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ea488-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ea488-119">Request headers</span></span>
| <span data-ttu-id="ea488-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ea488-120">Name</span></span>      |<span data-ttu-id="ea488-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea488-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ea488-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ea488-122">Authorization</span></span>  | <span data-ttu-id="ea488-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea488-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea488-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ea488-125">Request body</span></span>
<span data-ttu-id="ea488-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ea488-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea488-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea488-127">Response</span></span>

<span data-ttu-id="ea488-128">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [privilegedApproval](../resources/privilegedapproval.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ea488-128">If successful, this method returns a `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="ea488-129">Observe que o inquilino deve ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="ea488-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="ea488-130">Caso contrário, será retornado o código de status HTTP 403-Proibido.</span><span class="sxs-lookup"><span data-stu-id="ea488-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="ea488-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ea488-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ea488-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ea488-132">Request</span></span>
<span data-ttu-id="ea488-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ea488-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval/<id>
```
##### <a name="response"></a><span data-ttu-id="ea488-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea488-134">Response</span></span>
<span data-ttu-id="ea488-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ea488-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 193

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedapproval-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
