---
title: Atualizar eventMessage
description: Atualize as propriedades de um objeto eventMessage.
author: angelgolfer-ms
ms.openlocfilehash: 922f17528b864c8cdfae39a4df475a0a61f40103
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302468"
---
# <a name="update-eventmessage"></a><span data-ttu-id="dd21b-103">Atualizar eventMessage</span><span class="sxs-lookup"><span data-stu-id="dd21b-103">Update eventMessage</span></span>

> <span data-ttu-id="dd21b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="dd21b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd21b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dd21b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dd21b-106">Atualize as propriedades de um objeto [eventMessage](../resources/eventmessage.md).</span><span class="sxs-lookup"><span data-stu-id="dd21b-106">Update the properties of an [eventMessage](../resources/eventmessage.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="dd21b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="dd21b-107">Permissions</span></span>
<span data-ttu-id="dd21b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd21b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd21b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd21b-110">Permission type</span></span>      | <span data-ttu-id="dd21b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dd21b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd21b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd21b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dd21b-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd21b-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="dd21b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd21b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd21b-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd21b-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="dd21b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd21b-116">Application</span></span> | <span data-ttu-id="dd21b-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd21b-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd21b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd21b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}

PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="dd21b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd21b-119">Request headers</span></span>
| <span data-ttu-id="dd21b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="dd21b-120">Name</span></span>       | <span data-ttu-id="dd21b-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd21b-121">Type</span></span> | <span data-ttu-id="dd21b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd21b-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="dd21b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd21b-123">Authorization</span></span>  | <span data-ttu-id="dd21b-124">string</span><span class="sxs-lookup"><span data-stu-id="dd21b-124">string</span></span>  | <span data-ttu-id="dd21b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd21b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dd21b-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dd21b-127">Content-Type</span></span> | <span data-ttu-id="dd21b-128">string</span><span class="sxs-lookup"><span data-stu-id="dd21b-128">string</span></span>  | <span data-ttu-id="dd21b-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd21b-p104">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="dd21b-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dd21b-131">Request body</span></span>
<span data-ttu-id="dd21b-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados. As propriedades graváveis/atualizáveis são</span><span class="sxs-lookup"><span data-stu-id="dd21b-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="dd21b-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd21b-136">Property</span></span>     | <span data-ttu-id="dd21b-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd21b-137">Type</span></span>   |<span data-ttu-id="dd21b-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd21b-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd21b-139">categories</span><span class="sxs-lookup"><span data-stu-id="dd21b-139">categories</span></span>|<span data-ttu-id="dd21b-140">String</span><span class="sxs-lookup"><span data-stu-id="dd21b-140">String</span></span>|<span data-ttu-id="dd21b-141">As categorias associadas à mensagem.</span><span class="sxs-lookup"><span data-stu-id="dd21b-141">The categories associated with the message.</span></span>|
|<span data-ttu-id="dd21b-142">importance</span><span class="sxs-lookup"><span data-stu-id="dd21b-142">importance</span></span>|<span data-ttu-id="dd21b-143">String</span><span class="sxs-lookup"><span data-stu-id="dd21b-143">String</span></span>|<span data-ttu-id="dd21b-p106">A importância da mensagem. Os valores possíveis são: `Low`, `Normal` e `High`.</span><span class="sxs-lookup"><span data-stu-id="dd21b-p106">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="dd21b-146">isAllDay</span><span class="sxs-lookup"><span data-stu-id="dd21b-146">isAllDay</span></span> |<span data-ttu-id="dd21b-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd21b-147">Boolean</span></span>|<span data-ttu-id="dd21b-148">Indica se o evento durar o dia inteiro.</span><span class="sxs-lookup"><span data-stu-id="dd21b-148">Indicates whether the event lasts the entire day.</span></span> <span data-ttu-id="dd21b-149">Ajustar essa propriedade requer ajustando as propriedades **startDateTime** e **endDateTime** do evento também.</span><span class="sxs-lookup"><span data-stu-id="dd21b-149">Adjusting this property requires adjusting the **startDateTime** and **endDateTime** properties of the event as well.</span></span>|
|<span data-ttu-id="dd21b-150">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="dd21b-150">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="dd21b-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd21b-151">Boolean</span></span>|<span data-ttu-id="dd21b-152">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="dd21b-152">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="dd21b-153">isRead</span><span class="sxs-lookup"><span data-stu-id="dd21b-153">isRead</span></span>|<span data-ttu-id="dd21b-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd21b-154">Boolean</span></span>|<span data-ttu-id="dd21b-155">Indica se a mensagem foi lida.</span><span class="sxs-lookup"><span data-stu-id="dd21b-155">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="dd21b-156">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="dd21b-156">isReadReceiptRequested</span></span>|<span data-ttu-id="dd21b-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd21b-157">Boolean</span></span>|<span data-ttu-id="dd21b-158">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="dd21b-158">Indicates whether a read receipt is requested for the message.</span></span>|

## <a name="response"></a><span data-ttu-id="dd21b-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd21b-159">Response</span></span>

<span data-ttu-id="dd21b-160">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [eventMessage](../resources/eventmessage.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd21b-160">If successful, this method returns a `200 OK` response code and updated [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dd21b-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dd21b-161">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dd21b-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd21b-162">Request</span></span>
<span data-ttu-id="dd21b-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd21b-163">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_eventmessage"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "isRead": "true",
}
```
##### <a name="response"></a><span data-ttu-id="dd21b-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd21b-164">Response</span></span>
<span data-ttu-id="dd21b-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dd21b-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "2016-10-19T10:37:00Z",
  "sentDateTime": "2016-10-19T10:37:00Z",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value",
  "meetingMessageType": "meetingMessageType-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update eventmessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
