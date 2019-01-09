---
title: Listar anexos
description: Obtenha uma lista de objetos attachment anexado a uma tarefa do Outlook.
author: angelgolfer-ms
ms.openlocfilehash: b998f6f7d3356728400cc7c609dd1014467ae4d6
ms.sourcegitcommit: 6b1ba9b3be038cd6247de54a255bad560034fe42
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/08/2019
ms.locfileid: "27771790"
---
# <a name="list-attachments"></a><span data-ttu-id="66ba3-103">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="66ba3-103">List attachments</span></span>

> <span data-ttu-id="66ba3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="66ba3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66ba3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="66ba3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="66ba3-106">Obtenha uma lista de objetos [attachment](../resources/attachment.md) anexado a uma tarefa do Outlook.</span><span class="sxs-lookup"><span data-stu-id="66ba3-106">Get a list of [attachment](../resources/attachment.md) objects attached to an Outlook task.</span></span>

## <a name="permissions"></a><span data-ttu-id="66ba3-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="66ba3-107">Permissions</span></span>

<span data-ttu-id="66ba3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66ba3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66ba3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66ba3-110">Permission type</span></span>      | <span data-ttu-id="66ba3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="66ba3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66ba3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66ba3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="66ba3-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="66ba3-113">Tasks.Read</span></span>    |
|<span data-ttu-id="66ba3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66ba3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66ba3-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="66ba3-115">Tasks.Read</span></span>    |
|<span data-ttu-id="66ba3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66ba3-116">Application</span></span> | <span data-ttu-id="66ba3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66ba3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="66ba3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66ba3-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}/attachments
GET /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="66ba3-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="66ba3-119">Optional query parameters</span></span>

<span data-ttu-id="66ba3-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="66ba3-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="66ba3-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66ba3-121">Request headers</span></span>

| <span data-ttu-id="66ba3-122">Nome</span><span class="sxs-lookup"><span data-stu-id="66ba3-122">Name</span></span>      |<span data-ttu-id="66ba3-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="66ba3-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="66ba3-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="66ba3-124">Authorization</span></span>  | <span data-ttu-id="66ba3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66ba3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66ba3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66ba3-127">Request body</span></span>

<span data-ttu-id="66ba3-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="66ba3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66ba3-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="66ba3-129">Response</span></span>

<span data-ttu-id="66ba3-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos de [anexo](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66ba3-130">If successful, this method returns a `200 OK` response code and collection of [attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66ba3-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66ba3-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="66ba3-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66ba3-132">Request</span></span>

<span data-ttu-id="66ba3-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="66ba3-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->

```http
GET https://graph.microsoft.com/beta/users/{id}/outlook/tasks/{id}/attachments
```

### <a name="response"></a><span data-ttu-id="66ba3-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="66ba3-134">Response</span></span>

<span data-ttu-id="66ba3-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="66ba3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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