---
title: Lista taskFolders
description: Obtenha todas as pastas de tarefas do Outlook na caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 438f70a41044ccc5d2b94a8099647a82ae08f945
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518853"
---
# <a name="list-taskfolders"></a><span data-ttu-id="9289c-103">Lista taskFolders</span><span class="sxs-lookup"><span data-stu-id="9289c-103">List taskFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9289c-104">Obtenha todas as pastas de tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="9289c-104">Get all the Outlook task folders in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="9289c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9289c-105">Permissions</span></span>
<span data-ttu-id="9289c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9289c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9289c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9289c-108">Permission type</span></span>      | <span data-ttu-id="9289c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9289c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9289c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9289c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9289c-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="9289c-111">Tasks.Read</span></span>    |
|<span data-ttu-id="9289c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9289c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9289c-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="9289c-113">Tasks.Read</span></span>    |
|<span data-ttu-id="9289c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9289c-114">Application</span></span> | <span data-ttu-id="9289c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9289c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9289c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9289c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/taskFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9289c-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9289c-117">Optional query parameters</span></span>
<span data-ttu-id="9289c-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9289c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9289c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9289c-119">Request headers</span></span>
| <span data-ttu-id="9289c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="9289c-120">Name</span></span>      |<span data-ttu-id="9289c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9289c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9289c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9289c-122">Authorization</span></span>  | <span data-ttu-id="9289c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9289c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9289c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9289c-125">Request body</span></span>
<span data-ttu-id="9289c-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9289c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9289c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="9289c-127">Response</span></span>

<span data-ttu-id="9289c-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [outlookTaskFolder](../resources/outlooktaskfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9289c-128">If successful, this method returns a `200 OK` response code and collection of [outlookTaskFolder](../resources/outlooktaskfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9289c-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9289c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9289c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9289c-130">Request</span></span>
<span data-ttu-id="9289c-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9289c-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_taskfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskFolders
```
##### <a name="response"></a><span data-ttu-id="9289c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="9289c-132">Response</span></span>
<span data-ttu-id="9289c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9289c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "id": "AAMkADIyAAAAABrJAAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAAAAeAA==",
      "isDefaultFolder": false,
      "name": "Monthly tasks",
      "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"
    },
    {
      "id": "AAMkADIyAAAAAAESAAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAAAAAPA==",
      "isDefaultFolder": true,
      "name": "Tasks",
      "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"
    }

  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List TaskFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookuser-list-taskfolders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
