---
title: Obter outlookTaskGroup
description: Obtenha as propriedades e relacionamentos do grupo de tarefas especificado do Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 00abd783f8fa9ff726f5ada8f286529beddc9073
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816769"
---
# <a name="get-outlooktaskgroup"></a><span data-ttu-id="5d653-103">Obter outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="5d653-103">Get outlookTaskGroup</span></span>

> <span data-ttu-id="5d653-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5d653-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5d653-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5d653-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5d653-106">Obtenha as propriedades e relacionamentos do grupo de tarefas especificado do Outlook.</span><span class="sxs-lookup"><span data-stu-id="5d653-106">Get the properties and relationships of the specified Outlook task group.</span></span>
## <a name="permissions"></a><span data-ttu-id="5d653-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="5d653-107">Permissions</span></span>
<span data-ttu-id="5d653-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d653-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d653-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d653-110">Permission type</span></span>      | <span data-ttu-id="5d653-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5d653-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d653-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d653-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5d653-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="5d653-113">Tasks.Read</span></span>    |
|<span data-ttu-id="5d653-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d653-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d653-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="5d653-115">Tasks.Read</span></span>    |
|<span data-ttu-id="5d653-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d653-116">Application</span></span> | <span data-ttu-id="5d653-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d653-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d653-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d653-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5d653-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5d653-119">Optional query parameters</span></span>
<span data-ttu-id="5d653-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5d653-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5d653-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d653-121">Request headers</span></span>
| <span data-ttu-id="5d653-122">Nome</span><span class="sxs-lookup"><span data-stu-id="5d653-122">Name</span></span>      |<span data-ttu-id="5d653-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d653-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5d653-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5d653-124">Authorization</span></span>  | <span data-ttu-id="5d653-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d653-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d653-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d653-127">Request body</span></span>
<span data-ttu-id="5d653-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5d653-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d653-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d653-129">Response</span></span>

<span data-ttu-id="5d653-130">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [outlookTaskGroup](../resources/outlooktaskgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d653-130">If successful, this method returns a `200 OK` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5d653-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5d653-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5d653-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d653-132">Request</span></span>
<span data-ttu-id="5d653-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d653-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskgroup"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups('AAMkADIyAAAhrbe-AAA=')
```
##### <a name="response"></a><span data-ttu-id="5d653-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d653-134">Response</span></span>
<span data-ttu-id="5d653-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5d653-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 138

{
    "id": "AAMkADIyAAAhrbe-AAA=",
    "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAInHxKw==",
    "isDefaultGroup": false,
    "name": "Leisure Tasks",
    "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get outlookTaskGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
