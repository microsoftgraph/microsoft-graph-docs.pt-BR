---
title: Lista taskFolders
description: Obtenha todas as pastas de tarefas do Outlook na caixa de correio do usuário.
localization_priority: Normal
ms.openlocfilehash: 71cacaf2cc666376dc696a1df124847b6a2a45eb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837580"
---
# <a name="list-taskfolders"></a><span data-ttu-id="e9357-103">Lista taskFolders</span><span class="sxs-lookup"><span data-stu-id="e9357-103">List taskFolders</span></span>

> <span data-ttu-id="e9357-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e9357-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e9357-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e9357-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e9357-106">Obtenha todas as pastas de tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="e9357-106">Get all the Outlook task folders in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="e9357-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="e9357-107">Permissions</span></span>
<span data-ttu-id="e9357-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9357-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9357-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9357-110">Permission type</span></span>      | <span data-ttu-id="e9357-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e9357-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9357-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9357-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e9357-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="e9357-113">Tasks.Read</span></span>    |
|<span data-ttu-id="e9357-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9357-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9357-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="e9357-115">Tasks.Read</span></span>    |
|<span data-ttu-id="e9357-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9357-116">Application</span></span> | <span data-ttu-id="e9357-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9357-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9357-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9357-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/taskFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e9357-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e9357-119">Optional query parameters</span></span>
<span data-ttu-id="e9357-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e9357-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9357-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9357-121">Request headers</span></span>
| <span data-ttu-id="e9357-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e9357-122">Name</span></span>      |<span data-ttu-id="e9357-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9357-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e9357-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9357-124">Authorization</span></span>  | <span data-ttu-id="e9357-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9357-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9357-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9357-127">Request body</span></span>
<span data-ttu-id="e9357-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e9357-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9357-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9357-129">Response</span></span>

<span data-ttu-id="e9357-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [outlookTaskFolder](../resources/outlooktaskfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9357-130">If successful, this method returns a `200 OK` response code and collection of [outlookTaskFolder](../resources/outlooktaskfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e9357-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9357-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e9357-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9357-132">Request</span></span>
<span data-ttu-id="e9357-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9357-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_taskfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskFolders
```
##### <a name="response"></a><span data-ttu-id="e9357-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9357-134">Response</span></span>
<span data-ttu-id="e9357-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e9357-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List TaskFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
