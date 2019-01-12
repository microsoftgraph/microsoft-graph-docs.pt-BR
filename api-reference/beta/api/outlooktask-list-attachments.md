---
title: Listar anexos
description: Obtenha uma lista de objetos attachment anexado a uma tarefa do Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 6b65a6eabb0e002930253886b6799df54ab43f02
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924444"
---
# <a name="list-attachments"></a><span data-ttu-id="d1c78-103">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="d1c78-103">List attachments</span></span>

> <span data-ttu-id="d1c78-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d1c78-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1c78-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d1c78-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d1c78-106">Obtenha uma lista de objetos [attachment](../resources/attachment.md) anexado a uma tarefa do Outlook.</span><span class="sxs-lookup"><span data-stu-id="d1c78-106">Get a list of [attachment](../resources/attachment.md) objects attached to an Outlook task.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1c78-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="d1c78-107">Permissions</span></span>

<span data-ttu-id="d1c78-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1c78-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1c78-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1c78-110">Permission type</span></span>      | <span data-ttu-id="d1c78-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d1c78-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1c78-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1c78-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d1c78-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="d1c78-113">Tasks.Read</span></span>    |
|<span data-ttu-id="d1c78-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1c78-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1c78-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="d1c78-115">Tasks.Read</span></span>    |
|<span data-ttu-id="d1c78-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1c78-116">Application</span></span> | <span data-ttu-id="d1c78-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1c78-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1c78-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1c78-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}/attachments
GET /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d1c78-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d1c78-119">Optional query parameters</span></span>

<span data-ttu-id="d1c78-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d1c78-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1c78-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1c78-121">Request headers</span></span>

| <span data-ttu-id="d1c78-122">Nome</span><span class="sxs-lookup"><span data-stu-id="d1c78-122">Name</span></span>      |<span data-ttu-id="d1c78-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1c78-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d1c78-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1c78-124">Authorization</span></span>  | <span data-ttu-id="d1c78-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1c78-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1c78-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1c78-127">Request body</span></span>

<span data-ttu-id="d1c78-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d1c78-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1c78-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1c78-129">Response</span></span>

<span data-ttu-id="d1c78-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos de [anexo](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1c78-130">If successful, this method returns a `200 OK` response code and collection of [attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1c78-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1c78-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1c78-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1c78-132">Request</span></span>

<span data-ttu-id="d1c78-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1c78-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->

```http
GET https://graph.microsoft.com/beta/users/{id}/outlook/tasks/{id}/attachments
```

### <a name="response"></a><span data-ttu-id="d1c78-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1c78-134">Response</span></span>

<span data-ttu-id="d1c78-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d1c78-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "lastModifiedDateTime": "datetime-value",
      "name": "name-value",
      "contentType": "contentType-value",
      "size": 99,
      "isInline": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
