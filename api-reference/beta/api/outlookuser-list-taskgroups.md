---
title: Lista taskGroups
description: Obtenha todos os grupos de tarefas do Outlook na caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 3e0146a40698f8f150f39064b38aa562756b64ae
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913706"
---
# <a name="list-taskgroups"></a><span data-ttu-id="f2c5d-103">Lista taskGroups</span><span class="sxs-lookup"><span data-stu-id="f2c5d-103">List taskGroups</span></span>

> <span data-ttu-id="f2c5d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f2c5d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2c5d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f2c5d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f2c5d-106">Obtenha todos os grupos de tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="f2c5d-106">Get all the Outlook task groups in the user's mailbox.</span></span>

<span data-ttu-id="f2c5d-107">A resposta sempre inclui o grupo de tarefas padrão `My Tasks` e quaisquer outros grupos de tarefas criados na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="f2c5d-107">The response always includes the default task group `My Tasks`, and any other task groups that have been created in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="f2c5d-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="f2c5d-108">Permissions</span></span>
<span data-ttu-id="f2c5d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2c5d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2c5d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2c5d-111">Permission type</span></span>      | <span data-ttu-id="f2c5d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f2c5d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2c5d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2c5d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f2c5d-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="f2c5d-114">Tasks.Read</span></span>    |
|<span data-ttu-id="f2c5d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2c5d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2c5d-116">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="f2c5d-116">Tasks.Read</span></span>    |
|<span data-ttu-id="f2c5d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2c5d-117">Application</span></span> | <span data-ttu-id="f2c5d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2c5d-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2c5d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2c5d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f2c5d-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f2c5d-120">Optional query parameters</span></span>
<span data-ttu-id="f2c5d-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f2c5d-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2c5d-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2c5d-122">Request headers</span></span>
| <span data-ttu-id="f2c5d-123">Nome</span><span class="sxs-lookup"><span data-stu-id="f2c5d-123">Name</span></span>      |<span data-ttu-id="f2c5d-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2c5d-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f2c5d-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2c5d-125">Authorization</span></span>  | <span data-ttu-id="f2c5d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2c5d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2c5d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2c5d-128">Request body</span></span>
<span data-ttu-id="f2c5d-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f2c5d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2c5d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2c5d-130">Response</span></span>

<span data-ttu-id="f2c5d-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [outlookTaskGroup](../resources/outlooktaskgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2c5d-131">If successful, this method returns a `200 OK` response code and collection of [outlookTaskGroup](../resources/outlooktaskgroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f2c5d-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2c5d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f2c5d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2c5d-133">Request</span></span>
<span data-ttu-id="f2c5d-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2c5d-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_taskgroups"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups
```
##### <a name="response"></a><span data-ttu-id="f2c5d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2c5d-135">Response</span></span>
<span data-ttu-id="f2c5d-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2c5d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List TaskGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
