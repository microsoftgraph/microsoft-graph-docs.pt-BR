---
title: Obter outlookTaskFolder
description: Obtenha as propriedades e relacionamentos da pasta de tarefas do Outlook especificado.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 61f31f95ab31aab254c3497f088117480e84a512
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853540"
---
# <a name="get-outlooktaskfolder"></a><span data-ttu-id="c7a24-103">Obter outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="c7a24-103">Get outlookTaskFolder</span></span>

> <span data-ttu-id="c7a24-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c7a24-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7a24-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c7a24-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c7a24-106">Obtenha as propriedades e relacionamentos da pasta de tarefas do Outlook especificado.</span><span class="sxs-lookup"><span data-stu-id="c7a24-106">Get the properties and relationships of the specified Outlook task folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="c7a24-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="c7a24-107">Permissions</span></span>
<span data-ttu-id="c7a24-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7a24-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7a24-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7a24-110">Permission type</span></span>      | <span data-ttu-id="c7a24-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c7a24-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7a24-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7a24-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c7a24-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="c7a24-113">Tasks.Read</span></span>    |
|<span data-ttu-id="c7a24-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7a24-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7a24-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="c7a24-115">Tasks.Read</span></span>    |
|<span data-ttu-id="c7a24-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7a24-116">Application</span></span> | <span data-ttu-id="c7a24-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7a24-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7a24-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7a24-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c7a24-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c7a24-119">Optional query parameters</span></span>
<span data-ttu-id="c7a24-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c7a24-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7a24-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7a24-121">Request headers</span></span>
| <span data-ttu-id="c7a24-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c7a24-122">Name</span></span>      |<span data-ttu-id="c7a24-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7a24-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c7a24-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7a24-124">Authorization</span></span>  | <span data-ttu-id="c7a24-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7a24-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7a24-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7a24-127">Request body</span></span>
<span data-ttu-id="c7a24-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c7a24-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7a24-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7a24-129">Response</span></span>

<span data-ttu-id="c7a24-130">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [outlookTaskFolder](../resources/outlooktaskfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7a24-130">If successful, this method returns a `200 OK` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c7a24-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7a24-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c7a24-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7a24-132">Request</span></span>
<span data-ttu-id="c7a24-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7a24-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskFolders('AAMkADIyAAAAABrJAAA=')
```
##### <a name="response"></a><span data-ttu-id="c7a24-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7a24-134">Response</span></span>
<span data-ttu-id="c7a24-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c7a24-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 151

{
  "id": "AAMkADIyAAAAABrJAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAAAAeAA==",
  "isDefaultFolder": false,
  "name": "Monthly tasks",
  "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
