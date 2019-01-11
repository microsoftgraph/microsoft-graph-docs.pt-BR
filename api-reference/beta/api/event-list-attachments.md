---
title: Listar anexos
description: Recupera uma lista de objetos attachment anexados a um evento.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: d05bb4194a60346b97e6be368d6790fdebf8e12b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854702"
---
# <a name="list-attachments"></a><span data-ttu-id="46c74-103">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="46c74-103">List attachments</span></span>

> <span data-ttu-id="46c74-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="46c74-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46c74-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="46c74-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="46c74-106">Recupera uma lista de objetos [attachment](../resources/attachment.md) anexados a um evento.</span><span class="sxs-lookup"><span data-stu-id="46c74-106">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>

## <a name="permissions"></a><span data-ttu-id="46c74-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="46c74-107">Permissions</span></span>

<span data-ttu-id="46c74-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46c74-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46c74-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46c74-110">Permission type</span></span>      | <span data-ttu-id="46c74-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46c74-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46c74-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46c74-112">Delegated (work or school account)</span></span> | <span data-ttu-id="46c74-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="46c74-113">Calendars.Read</span></span>    |
|<span data-ttu-id="46c74-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46c74-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46c74-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="46c74-115">Calendars.Read</span></span>    |
|<span data-ttu-id="46c74-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46c74-116">Application</span></span> | <span data-ttu-id="46c74-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="46c74-117">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="46c74-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46c74-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/events/{id}/attachments
GET /users/{id|userPrincipalName}/events/{id}/attachments
```

<!--
GET /groups/{id}/events/{id}/attachments
-->

## <a name="optional-query-parameters"></a><span data-ttu-id="46c74-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="46c74-119">Optional query parameters</span></span>

<span data-ttu-id="46c74-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="46c74-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="46c74-121">Em particular, você pode usar o `$expand` consulta parâmetro para incluir todos os o embutido de anexos de evento com o restante das propriedades do evento.</span><span class="sxs-lookup"><span data-stu-id="46c74-121">In particular, you can use the `$expand` query parameter to include all of the event attachments inline with the rest of the event properties.</span></span> <span data-ttu-id="46c74-122">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="46c74-122">For example:</span></span>

```http
GET https://graph.microsoft.com/beta/me/events/{id}?$expand=attachments
```

## <a name="request-headers"></a><span data-ttu-id="46c74-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46c74-123">Request headers</span></span>

| <span data-ttu-id="46c74-124">Nome</span><span class="sxs-lookup"><span data-stu-id="46c74-124">Name</span></span>       | <span data-ttu-id="46c74-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="46c74-125">Type</span></span> | <span data-ttu-id="46c74-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="46c74-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="46c74-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="46c74-127">Authorization</span></span>  | <span data-ttu-id="46c74-128">string</span><span class="sxs-lookup"><span data-stu-id="46c74-128">string</span></span>  | <span data-ttu-id="46c74-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46c74-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="46c74-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46c74-131">Request body</span></span>

<span data-ttu-id="46c74-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="46c74-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46c74-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="46c74-133">Response</span></span>

<span data-ttu-id="46c74-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46c74-134">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46c74-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46c74-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="46c74-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46c74-136">Request</span></span>

<span data-ttu-id="46c74-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="46c74-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->

```http
GET https://graph.microsoft.com/beta/me/events/{id}/attachments
```

### <a name="response"></a><span data-ttu-id="46c74-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="46c74-138">Response</span></span>

<span data-ttu-id="46c74-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="46c74-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "isInline": false,
      "isContactPhoto": false,
      "name": "name-value",
      "size": 99
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
