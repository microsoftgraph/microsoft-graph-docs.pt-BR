---
title: Criar anexo
description: Use esta API para adicionar um anexo a um outlookTask.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: ae6c420c9c0ccf10df4d2d62a27f4b8c0d857c32
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539785"
---
# <a name="create-attachment"></a><span data-ttu-id="af8d5-103">Criar anexo</span><span class="sxs-lookup"><span data-stu-id="af8d5-103">Create attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af8d5-104">Use esta API para adicionar um [anexo](../resources/attachment.md) a um [outlookTask](../resources/outlooktask.md).</span><span class="sxs-lookup"><span data-stu-id="af8d5-104">Use this API to add an [attachment](../resources/attachment.md) to an [outlookTask](../resources/outlooktask.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="af8d5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="af8d5-105">Permissions</span></span>

<span data-ttu-id="af8d5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af8d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af8d5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af8d5-108">Permission type</span></span>      | <span data-ttu-id="af8d5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="af8d5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af8d5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af8d5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="af8d5-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="af8d5-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="af8d5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af8d5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af8d5-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="af8d5-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="af8d5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af8d5-114">Application</span></span> | <span data-ttu-id="af8d5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af8d5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="af8d5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af8d5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/attachments
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="request-headers"></a><span data-ttu-id="af8d5-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af8d5-117">Request headers</span></span>

| <span data-ttu-id="af8d5-118">Nome</span><span class="sxs-lookup"><span data-stu-id="af8d5-118">Name</span></span>       | <span data-ttu-id="af8d5-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="af8d5-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="af8d5-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="af8d5-120">Authorization</span></span>  | <span data-ttu-id="af8d5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af8d5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="af8d5-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="af8d5-123">Content-Type</span></span> | <span data-ttu-id="af8d5-124">Uma cadeia de caracteres que representa o tipo de dados no corpo de uma entidade.</span><span class="sxs-lookup"><span data-stu-id="af8d5-124">A string that represents the type of data in the body of an entity.</span></span> <span data-ttu-id="af8d5-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af8d5-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="af8d5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af8d5-126">Request body</span></span>

<span data-ttu-id="af8d5-127">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="af8d5-127">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="af8d5-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="af8d5-128">Response</span></span>

<span data-ttu-id="af8d5-129">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af8d5-129">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af8d5-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="af8d5-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="af8d5-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af8d5-131">Request</span></span>

<span data-ttu-id="af8d5-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="af8d5-132">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="af8d5-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="af8d5-133">Response</span></span>

<span data-ttu-id="af8d5-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="af8d5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktask-post-attachments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
