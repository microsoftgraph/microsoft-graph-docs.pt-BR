---
title: Atualizar eventMessage
description: Atualize as propriedades de um objeto eventMessage.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a906dbbdb9a82e78a49ea41399e3791c9d52645b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584226"
---
# <a name="update-eventmessage"></a><span data-ttu-id="1f882-103">Atualizar eventMessage</span><span class="sxs-lookup"><span data-stu-id="1f882-103">Update eventMessage</span></span>

<span data-ttu-id="1f882-104">Atualize as propriedades de um objeto [eventMessage](../resources/eventmessage.md).</span><span class="sxs-lookup"><span data-stu-id="1f882-104">Update the properties of an [eventMessage](../resources/eventmessage.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1f882-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1f882-105">Permissions</span></span>
<span data-ttu-id="1f882-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f882-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f882-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f882-108">Permission type</span></span>      | <span data-ttu-id="1f882-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1f882-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f882-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f882-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1f882-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1f882-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1f882-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f882-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f882-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1f882-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1f882-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f882-114">Application</span></span> | <span data-ttu-id="1f882-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1f882-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f882-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f882-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}

PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1f882-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f882-117">Request headers</span></span>
| <span data-ttu-id="1f882-118">Nome</span><span class="sxs-lookup"><span data-stu-id="1f882-118">Name</span></span>       | <span data-ttu-id="1f882-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f882-119">Type</span></span> | <span data-ttu-id="1f882-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f882-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1f882-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f882-121">Authorization</span></span>  | <span data-ttu-id="1f882-122">string</span><span class="sxs-lookup"><span data-stu-id="1f882-122">string</span></span>  | <span data-ttu-id="1f882-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f882-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1f882-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1f882-125">Content-Type</span></span> | <span data-ttu-id="1f882-126">string</span><span class="sxs-lookup"><span data-stu-id="1f882-126">string</span></span>  | <span data-ttu-id="1f882-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f882-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="1f882-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f882-129">Request body</span></span>
<span data-ttu-id="1f882-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados. As propriedades graváveis/atualizáveis são</span><span class="sxs-lookup"><span data-stu-id="1f882-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="1f882-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1f882-134">Property</span></span>     | <span data-ttu-id="1f882-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f882-135">Type</span></span>   |<span data-ttu-id="1f882-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f882-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f882-137">categories</span><span class="sxs-lookup"><span data-stu-id="1f882-137">categories</span></span>|<span data-ttu-id="1f882-138">String</span><span class="sxs-lookup"><span data-stu-id="1f882-138">String</span></span>|<span data-ttu-id="1f882-139">As categorias associadas à mensagem.</span><span class="sxs-lookup"><span data-stu-id="1f882-139">The categories associated with the message.</span></span>|
|<span data-ttu-id="1f882-140">importance</span><span class="sxs-lookup"><span data-stu-id="1f882-140">importance</span></span>|<span data-ttu-id="1f882-141">String</span><span class="sxs-lookup"><span data-stu-id="1f882-141">String</span></span>|<span data-ttu-id="1f882-142">A importância da mensagem.</span><span class="sxs-lookup"><span data-stu-id="1f882-142">The importance of the message.</span></span> <span data-ttu-id="1f882-143">Os valores possíveis são: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="1f882-143">The possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="1f882-144">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="1f882-144">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="1f882-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f882-145">Boolean</span></span>|<span data-ttu-id="1f882-146">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="1f882-146">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="1f882-147">isRead</span><span class="sxs-lookup"><span data-stu-id="1f882-147">isRead</span></span>|<span data-ttu-id="1f882-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f882-148">Boolean</span></span>|<span data-ttu-id="1f882-149">Indica se a mensagem foi lida.</span><span class="sxs-lookup"><span data-stu-id="1f882-149">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="1f882-150">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="1f882-150">isReadReceiptRequested</span></span>|<span data-ttu-id="1f882-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f882-151">Boolean</span></span>|<span data-ttu-id="1f882-152">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="1f882-152">Indicates whether a read receipt is requested for the message.</span></span>|

## <a name="response"></a><span data-ttu-id="1f882-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f882-153">Response</span></span>

<span data-ttu-id="1f882-154">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [eventMessage](../resources/eventmessage.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f882-154">If successful, this method returns a `200 OK` response code and updated [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1f882-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1f882-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1f882-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f882-156">Request</span></span>
<span data-ttu-id="1f882-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1f882-157">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_eventmessage"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "isRead": "true",
}
```
##### <a name="response"></a><span data-ttu-id="1f882-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f882-158">Response</span></span>
<span data-ttu-id="1f882-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1f882-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
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
