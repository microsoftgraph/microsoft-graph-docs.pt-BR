---
title: Listar taskFolders
description: Obter pastas de tarefas do Outlook em um outlookTaskGroup específico.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: c639fb0fe8e1ae010c3f5dbfb6b9c85c34009f00
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869460"
---
# <a name="list-taskfolders"></a><span data-ttu-id="e7d98-103">Listar taskFolders</span><span class="sxs-lookup"><span data-stu-id="e7d98-103">List taskFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7d98-104">Obter pastas de tarefas do Outlook em um [outlookTaskGroup](../resources/outlooktaskgroup.md)específico.</span><span class="sxs-lookup"><span data-stu-id="e7d98-104">Get Outlook task folders in a specific [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="e7d98-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e7d98-105">Permissions</span></span>
<span data-ttu-id="e7d98-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7d98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7d98-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7d98-108">Permission type</span></span>      | <span data-ttu-id="e7d98-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e7d98-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7d98-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7d98-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e7d98-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="e7d98-111">Tasks.Read</span></span>    |
|<span data-ttu-id="e7d98-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7d98-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7d98-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="e7d98-113">Tasks.Read</span></span>    |
|<span data-ttu-id="e7d98-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7d98-114">Application</span></span> | <span data-ttu-id="e7d98-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7d98-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7d98-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7d98-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups/{id}/taskFolders
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e7d98-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e7d98-117">Optional query parameters</span></span>
<span data-ttu-id="e7d98-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e7d98-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e7d98-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7d98-119">Request headers</span></span>
| <span data-ttu-id="e7d98-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e7d98-120">Name</span></span>      |<span data-ttu-id="e7d98-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7d98-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e7d98-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7d98-122">Authorization</span></span>  | <span data-ttu-id="e7d98-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7d98-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e7d98-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7d98-125">Request body</span></span>
<span data-ttu-id="e7d98-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e7d98-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7d98-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7d98-127">Response</span></span>

<span data-ttu-id="e7d98-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [outlookTaskFolder](../resources/outlooktaskfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7d98-128">If successful, this method returns a `200 OK` response code and collection of [outlookTaskFolder](../resources/outlooktaskfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e7d98-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7d98-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e7d98-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7d98-130">Request</span></span>
<span data-ttu-id="e7d98-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7d98-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_taskfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups('AAMkADIyAAAhrbe-AAA=')/taskFolders
```
##### <a name="response"></a><span data-ttu-id="e7d98-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7d98-132">Response</span></span>
<span data-ttu-id="e7d98-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7d98-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 200

{
  "value": [
    {
      "id": "AAMkADIyAAAhrbPXAAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAOlA==",
      "isDefaultFolder": false,
      "name": "Cooking",
      "parentGroupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"
    }

  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List taskFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktaskgroup-list-taskfolders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
