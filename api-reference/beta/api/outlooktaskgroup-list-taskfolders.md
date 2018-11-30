---
title: Lista taskFolders
description: Obtenha as pastas de tarefas do Outlook em um outlookTaskGroup específico.
ms.openlocfilehash: 243d93bbe31f0e7bb51b971a303105a8a22e7eea
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039575"
---
# <a name="list-taskfolders"></a><span data-ttu-id="f19a6-103">Lista taskFolders</span><span class="sxs-lookup"><span data-stu-id="f19a6-103">List taskFolders</span></span>

> <span data-ttu-id="f19a6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f19a6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f19a6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f19a6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f19a6-106">Obtenha as pastas de tarefas do Outlook em um determinado [outlookTaskGroup](../resources/outlooktaskgroup.md).</span><span class="sxs-lookup"><span data-stu-id="f19a6-106">Get Outlook task folders in a specific [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="f19a6-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="f19a6-107">Permissions</span></span>
<span data-ttu-id="f19a6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f19a6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f19a6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f19a6-110">Permission type</span></span>      | <span data-ttu-id="f19a6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f19a6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f19a6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f19a6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f19a6-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="f19a6-113">Tasks.Read</span></span>    |
|<span data-ttu-id="f19a6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f19a6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f19a6-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="f19a6-115">Tasks.Read</span></span>    |
|<span data-ttu-id="f19a6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f19a6-116">Application</span></span> | <span data-ttu-id="f19a6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f19a6-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f19a6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f19a6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f19a6-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f19a6-119">Optional query parameters</span></span>
<span data-ttu-id="f19a6-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f19a6-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f19a6-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f19a6-121">Request headers</span></span>
| <span data-ttu-id="f19a6-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f19a6-122">Name</span></span>      |<span data-ttu-id="f19a6-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f19a6-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f19a6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f19a6-124">Authorization</span></span>  | <span data-ttu-id="f19a6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f19a6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f19a6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f19a6-127">Request body</span></span>
<span data-ttu-id="f19a6-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f19a6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f19a6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f19a6-129">Response</span></span>

<span data-ttu-id="f19a6-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [outlookTaskFolder](../resources/outlooktaskfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f19a6-130">If successful, this method returns a `200 OK` response code and collection of [outlookTaskFolder](../resources/outlooktaskfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f19a6-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f19a6-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f19a6-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f19a6-132">Request</span></span>
<span data-ttu-id="f19a6-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f19a6-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_taskfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups('AAMkADIyAAAhrbe-AAA=')/taskFolders
```
##### <a name="response"></a><span data-ttu-id="f19a6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f19a6-134">Response</span></span>
<span data-ttu-id="f19a6-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f19a6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List taskFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->