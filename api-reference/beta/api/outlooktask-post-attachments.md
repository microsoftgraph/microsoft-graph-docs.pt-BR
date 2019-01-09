---
title: Criar anexo
description: Use essa API para adicionar um anexo a um outlookTask.
author: angelgolfer-ms
ms.openlocfilehash: 3b3cc5d6d4357e74c0b63166a492eafe97813b06
ms.sourcegitcommit: 6b1ba9b3be038cd6247de54a255bad560034fe42
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/08/2019
ms.locfileid: "27771671"
---
# <a name="create-attachment"></a><span data-ttu-id="e2a1a-103">Criar anexo</span><span class="sxs-lookup"><span data-stu-id="e2a1a-103">Create attachment</span></span>

> <span data-ttu-id="e2a1a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e2a1a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2a1a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e2a1a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e2a1a-106">Use essa API para adicionar um [anexo](../resources/attachment.md) a um [outlookTask](../resources/outlooktask.md).</span><span class="sxs-lookup"><span data-stu-id="e2a1a-106">Use this API to add an [attachment](../resources/attachment.md) to an [outlookTask](../resources/outlooktask.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e2a1a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e2a1a-107">Permissions</span></span>

<span data-ttu-id="e2a1a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2a1a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2a1a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2a1a-110">Permission type</span></span>      | <span data-ttu-id="e2a1a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e2a1a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2a1a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2a1a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e2a1a-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e2a1a-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="e2a1a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2a1a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2a1a-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e2a1a-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="e2a1a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e2a1a-116">Application</span></span> | <span data-ttu-id="e2a1a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2a1a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2a1a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2a1a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/attachments
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="request-headers"></a><span data-ttu-id="e2a1a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2a1a-119">Request headers</span></span>

| <span data-ttu-id="e2a1a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e2a1a-120">Name</span></span>       | <span data-ttu-id="e2a1a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2a1a-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e2a1a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e2a1a-122">Authorization</span></span>  | <span data-ttu-id="e2a1a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2a1a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e2a1a-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e2a1a-125">Content-Type</span></span> | <span data-ttu-id="e2a1a-126">Uma string que representa o tipo de dados no corpo de uma entidade.</span><span class="sxs-lookup"><span data-stu-id="e2a1a-126">A string that represents the type of data in the body of an entity.</span></span> <span data-ttu-id="e2a1a-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2a1a-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2a1a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2a1a-128">Request body</span></span>

<span data-ttu-id="e2a1a-129">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="e2a1a-129">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e2a1a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2a1a-130">Response</span></span>

<span data-ttu-id="e2a1a-131">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2a1a-131">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2a1a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e2a1a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2a1a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2a1a-133">Request</span></span>

<span data-ttu-id="e2a1a-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2a1a-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_attachment_from_outlooktask"
}-->

```http
POST https://graph.microsoft.com/beta/users/{id}/outlook/tasks/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true
}
```

### <a name="response"></a><span data-ttu-id="e2a1a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2a1a-135">Response</span></span>

<span data-ttu-id="e2a1a-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e2a1a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->