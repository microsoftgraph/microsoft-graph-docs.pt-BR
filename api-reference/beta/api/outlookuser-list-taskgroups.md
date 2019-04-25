---
title: Listar taskGroups
description: Obter todos os grupos de tarefas do Outlook na caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b3ebf2896ff8805280c23680915e54f9a094a7c8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539616"
---
# <a name="list-taskgroups"></a><span data-ttu-id="0a042-103">Listar taskGroups</span><span class="sxs-lookup"><span data-stu-id="0a042-103">List taskGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a042-104">Obter todos os grupos de tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="0a042-104">Get all the Outlook task groups in the user's mailbox.</span></span>

<span data-ttu-id="0a042-105">A resposta sempre inclui o grupo de tarefas padrão `My Tasks` e quaisquer outros grupos de tarefas criados na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="0a042-105">The response always includes the default task group `My Tasks`, and any other task groups that have been created in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="0a042-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0a042-106">Permissions</span></span>
<span data-ttu-id="0a042-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a042-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a042-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a042-109">Permission type</span></span>      | <span data-ttu-id="0a042-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0a042-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a042-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a042-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0a042-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="0a042-112">Tasks.Read</span></span>    |
|<span data-ttu-id="0a042-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a042-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a042-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="0a042-114">Tasks.Read</span></span>    |
|<span data-ttu-id="0a042-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0a042-115">Application</span></span> | <span data-ttu-id="0a042-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a042-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a042-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a042-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups
GET /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0a042-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0a042-118">Optional query parameters</span></span>
<span data-ttu-id="0a042-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0a042-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0a042-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a042-120">Request headers</span></span>
| <span data-ttu-id="0a042-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0a042-121">Name</span></span>      |<span data-ttu-id="0a042-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a042-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0a042-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a042-123">Authorization</span></span>  | <span data-ttu-id="0a042-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a042-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a042-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a042-126">Request body</span></span>
<span data-ttu-id="0a042-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0a042-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a042-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a042-128">Response</span></span>

<span data-ttu-id="0a042-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [outlookTaskGroup](../resources/outlooktaskgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a042-129">If successful, this method returns a `200 OK` response code and collection of [outlookTaskGroup](../resources/outlooktaskgroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0a042-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0a042-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0a042-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a042-131">Request</span></span>
<span data-ttu-id="0a042-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a042-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_taskgroups"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups
```
##### <a name="response"></a><span data-ttu-id="0a042-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a042-133">Response</span></span>
<span data-ttu-id="0a042-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0a042-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 187

{
  "value": [
    {
      "id": "AAMkADIyAAADJ5pYAAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAInHxLA==",
      "isDefaultGroup": true,
      "name": "My Tasks",
      "groupKey": "0006f0b7-0000-0000-c000-000000000046"
    },
    {
      "id": "AAMkADIyAAAhrbe-AAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAInHxKw==",
      "isDefaultGroup": false,
      "name": "Leisure Tasks",
      "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"
    }

  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List TaskGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookuser-list-taskgroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
