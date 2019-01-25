---
title: Lista agreementAcceptances
description: Recupere uma lista de objetos de agreementAcceptance de um usuário.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 22babc13c3b1db4cf143a35ab2119e97c43c822b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517866"
---
# <a name="list-agreementacceptances"></a><span data-ttu-id="f482a-103">Lista agreementAcceptances</span><span class="sxs-lookup"><span data-stu-id="f482a-103">List agreementAcceptances</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f482a-104">Recupere uma lista de objetos de [agreementAcceptance](../resources/agreementacceptance.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f482a-104">Retrieve a list of a user's [agreementAcceptance](../resources/agreementacceptance.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="f482a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f482a-105">Permissions</span></span>
<span data-ttu-id="f482a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f482a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f482a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f482a-108">Permission type</span></span>                        | <span data-ttu-id="f482a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f482a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f482a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f482a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f482a-111">AgreementAcceptance.Read</span><span class="sxs-lookup"><span data-stu-id="f482a-111">AgreementAcceptance.Read</span></span> |
|<span data-ttu-id="f482a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f482a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f482a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f482a-113">Not supported.</span></span> |
|<span data-ttu-id="f482a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f482a-114">Application</span></span>                            | <span data-ttu-id="f482a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f482a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f482a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f482a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/agreementAcceptances
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="f482a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f482a-117">Request headers</span></span>
| <span data-ttu-id="f482a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f482a-118">Name</span></span>      |<span data-ttu-id="f482a-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f482a-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f482a-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f482a-120">Authorization</span></span> | <span data-ttu-id="f482a-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="f482a-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f482a-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f482a-122">Request body</span></span>
<span data-ttu-id="f482a-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f482a-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f482a-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="f482a-124">Response</span></span>
<span data-ttu-id="f482a-125">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [agreementAcceptance](../resources/agreementacceptance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f482a-125">If successful, this method returns a `200 OK` response code and a collection of [agreementAcceptance](../resources/agreementacceptance.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f482a-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f482a-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f482a-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f482a-127">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreementacceptances"
}-->
```http
GET https://graph.microsoft.com/beta/me/agreementAcceptances
```
##### <a name="response"></a><span data-ttu-id="f482a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f482a-128">Response</span></span>
><span data-ttu-id="f482a-p102">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f482a-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreementAcceptance",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 303

{
  "value": [
    {
      "agreementId": "agreementId-value",
      "userId": "userId-value",
      "agreementFileId": "agreementFileId-value",
      "recordedDateTime": "datetime-value",
      "userDisplayName": "userDisplayName-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List agreementAcceptances",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-agreementacceptances.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
