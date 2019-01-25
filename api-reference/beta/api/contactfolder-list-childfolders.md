---
title: Listar childFolders
description: Obtém uma coleção de pastas filho sob a pasta de contatos especificada.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5e4230976e032ff77189bf0b691ddcd365e92522
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507842"
---
# <a name="list-childfolders"></a><span data-ttu-id="291ad-103">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="291ad-103">List childFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="291ad-104">Obtém uma coleção de pastas filho sob a pasta de contatos especificada.</span><span class="sxs-lookup"><span data-stu-id="291ad-104">Get a collection of child folders under the specified contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="291ad-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="291ad-105">Permissions</span></span>
<span data-ttu-id="291ad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="291ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="291ad-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="291ad-108">Permission type</span></span>      | <span data-ttu-id="291ad-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="291ad-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="291ad-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="291ad-110">Delegated (work or school account)</span></span> | <span data-ttu-id="291ad-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="291ad-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="291ad-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="291ad-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="291ad-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="291ad-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="291ad-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="291ad-114">Application</span></span> | <span data-ttu-id="291ad-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="291ad-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="291ad-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="291ad-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="291ad-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="291ad-117">Optional query parameters</span></span>
<span data-ttu-id="291ad-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="291ad-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="291ad-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="291ad-119">Request headers</span></span>
| <span data-ttu-id="291ad-120">Nome</span><span class="sxs-lookup"><span data-stu-id="291ad-120">Name</span></span>       | <span data-ttu-id="291ad-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="291ad-121">Type</span></span> | <span data-ttu-id="291ad-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="291ad-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="291ad-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="291ad-123">Authorization</span></span>  | <span data-ttu-id="291ad-124">string</span><span class="sxs-lookup"><span data-stu-id="291ad-124">string</span></span>  | <span data-ttu-id="291ad-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="291ad-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="291ad-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="291ad-127">Request body</span></span>
<span data-ttu-id="291ad-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="291ad-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="291ad-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="291ad-129">Response</span></span>

<span data-ttu-id="291ad-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [ContactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="291ad-130">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="291ad-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="291ad-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="291ad-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="291ad-132">Request</span></span>
<span data-ttu-id="291ad-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="291ad-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/{id}/childFolders
```
##### <a name="response"></a><span data-ttu-id="291ad-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="291ad-134">Response</span></span>
<span data-ttu-id="291ad-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="291ad-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/contactfolder-list-childfolders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
