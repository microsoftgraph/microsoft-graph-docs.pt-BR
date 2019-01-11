---
title: Criar thread de bate-papo
description: Crie um novo segmento de bate-papo no canal especificado, fornecendo as mensagens de raiz.
author: nkramer
localization_priority: Priority
ms.openlocfilehash: edd3c99376a93b2c4405d97b6435cfd9a128ae8b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809069"
---
# <a name="create-chat-thread"></a><span data-ttu-id="3e627-103">Criar thread de bate-papo</span><span class="sxs-lookup"><span data-stu-id="3e627-103">Create chat thread</span></span>

> <span data-ttu-id="3e627-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3e627-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e627-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3e627-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3e627-106">Crie um novo segmento de bate-papo no [canal](../resources/channel.md) especificado, fornecendo as mensagens de raiz.</span><span class="sxs-lookup"><span data-stu-id="3e627-106">Create a new chat thread in the specified [channel](../resources/channel.md) by supplying the root messages.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e627-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="3e627-107">Permissions</span></span>
<span data-ttu-id="3e627-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e627-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e627-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e627-110">Permission type</span></span>      | <span data-ttu-id="3e627-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3e627-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e627-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e627-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3e627-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e627-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3e627-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e627-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e627-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e627-115">Not supported.</span></span>    |
|<span data-ttu-id="3e627-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e627-116">Application</span></span> | <span data-ttu-id="3e627-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e627-117">Not supported.</span></span> |

> <span data-ttu-id="3e627-118">Atualmente, somente [permissões delegadas](/graph/permissions-reference) têm suporte para esta operação.</span><span class="sxs-lookup"><span data-stu-id="3e627-118">Currently, only [delegated permissions](/graph/permissions-reference) are supported for this operation.</span></span>  <span data-ttu-id="3e627-119">Permissões de aplicativo dará suporte a versões futuras.</span><span class="sxs-lookup"><span data-stu-id="3e627-119">Future releases will support application permissions.</span></span> 

## <a name="http-request"></a><span data-ttu-id="3e627-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e627-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/chatThreads
```
## <a name="request-headers"></a><span data-ttu-id="3e627-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e627-121">Request headers</span></span>
| <span data-ttu-id="3e627-122">Nome</span><span class="sxs-lookup"><span data-stu-id="3e627-122">Name</span></span>       | <span data-ttu-id="3e627-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e627-123">Type</span></span> | <span data-ttu-id="3e627-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e627-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3e627-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e627-125">Authorization</span></span>  | <span data-ttu-id="3e627-126">string</span><span class="sxs-lookup"><span data-stu-id="3e627-126">string</span></span>  | <span data-ttu-id="3e627-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e627-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e627-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e627-129">Request body</span></span>
<span data-ttu-id="3e627-130">No corpo da solicitação, fornece uma representação JSON de um objeto [chatThread](../resources/chatthread.md) que contém a propriedade rootMessage.</span><span class="sxs-lookup"><span data-stu-id="3e627-130">In the request body, supply a JSON representation of a [chatThread](../resources/chatthread.md) object that contains the rootMessage property.</span></span>

## <a name="response"></a><span data-ttu-id="3e627-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e627-131">Response</span></span>

<span data-ttu-id="3e627-132">Se tiver êxito, este método retornará `201 Created` código de resposta com o corpo de uma resposta vazia.</span><span class="sxs-lookup"><span data-stu-id="3e627-132">If successful, this method returns `201 Created` response code with an empty reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="3e627-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3e627-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e627-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e627-134">Request</span></span>
<span data-ttu-id="3e627-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e627-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chatthread_from_channel"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/chatThreads
Content-type: application/json

{
  "rootMessage": {
      "body": {
        "contentType": 1,
        "content": "<h1>Hello world</h1>"
      }
  }
}
```

> <span data-ttu-id="3e627-136">Atualmente, o contentType deve ser especificado como um inteiro, em vez de uma cadeia de caracteres: 0 para "text" ou 1 para "html".</span><span class="sxs-lookup"><span data-stu-id="3e627-136">Currently, the contentType must be specified as an integer rather than a string: 0 for "text" or 1 for "html".</span></span>  <span data-ttu-id="3e627-137">Versões futuras do API corrigirá.</span><span class="sxs-lookup"><span data-stu-id="3e627-137">Future API releases will fix this.</span></span>

##### <a name="response"></a><span data-ttu-id="3e627-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e627-138">Response</span></span>

<span data-ttu-id="3e627-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e627-139">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatThread"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 160

{
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
