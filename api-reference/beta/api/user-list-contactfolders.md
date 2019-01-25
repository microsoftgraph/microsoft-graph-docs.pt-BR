---
title: Listar contactFolders
description: Obtenha todas as pastas de contato na caixa de correio do usuário conectado.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f5f0a485c3c134b6627fce5d3b8f04c26dee503e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523278"
---
# <a name="list-contactfolders"></a><span data-ttu-id="95226-103">Listar contactFolders</span><span class="sxs-lookup"><span data-stu-id="95226-103">List contactFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95226-104">Obtenha todas as pastas de contato na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="95226-104">Get all the contact folders in the signed-in user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="95226-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="95226-105">Permissions</span></span>
<span data-ttu-id="95226-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95226-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95226-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95226-108">Permission type</span></span>      | <span data-ttu-id="95226-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="95226-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95226-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95226-110">Delegated (work or school account)</span></span> | <span data-ttu-id="95226-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="95226-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="95226-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95226-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95226-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="95226-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="95226-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95226-114">Application</span></span> | <span data-ttu-id="95226-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="95226-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="95226-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95226-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/contactFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="95226-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="95226-117">Optional query parameters</span></span>
<span data-ttu-id="95226-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="95226-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="95226-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95226-119">Request headers</span></span>
| <span data-ttu-id="95226-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="95226-120">Header</span></span>       | <span data-ttu-id="95226-121">Valor</span><span class="sxs-lookup"><span data-stu-id="95226-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="95226-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="95226-122">Authorization</span></span>  | <span data-ttu-id="95226-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95226-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="95226-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="95226-125">Content-Type</span></span>   | <span data-ttu-id="95226-126">application/json</span><span class="sxs-lookup"><span data-stu-id="95226-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="95226-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95226-127">Request body</span></span>
<span data-ttu-id="95226-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="95226-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95226-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="95226-129">Response</span></span>

<span data-ttu-id="95226-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [ContactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95226-130">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="95226-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="95226-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="95226-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95226-132">Request</span></span>
<span data-ttu-id="95226-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="95226-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders
```
##### <a name="response"></a><span data-ttu-id="95226-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="95226-134">Response</span></span>
<span data-ttu-id="95226-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="95226-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "displayName": "displayName-value",
      "wellKnownName": "wellKnownName-value",
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
  "description": "List contactFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-contactfolders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
