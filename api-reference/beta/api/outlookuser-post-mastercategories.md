---
title: Criar categoria do Outlook
description: Cria um objeto outlookCategory na lista mestra de categorias do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e76f6ddc0f733bd2e50b3aac62707acbed370ee3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984700"
---
# <a name="create-outlook-category"></a><span data-ttu-id="6db00-103">Criar categoria do Outlook</span><span class="sxs-lookup"><span data-stu-id="6db00-103">Create Outlook category</span></span>

> <span data-ttu-id="6db00-104">**Importante**: APIs sob a versão /beta no Microsoft Graph estiver em Visualizar e estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="6db00-104">**Important**: APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6db00-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6db00-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6db00-106">Cria um objeto [outlookCategory](../resources/outlookcategory.md) na lista mestra de categorias do usuário.</span><span class="sxs-lookup"><span data-stu-id="6db00-106">Create an [outlookCategory](../resources/outlookcategory.md) object in the user's master list of categories.</span></span>

## <a name="permissions"></a><span data-ttu-id="6db00-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="6db00-107">Permissions</span></span>
<span data-ttu-id="6db00-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6db00-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6db00-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6db00-110">Permission type</span></span>      | <span data-ttu-id="6db00-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6db00-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6db00-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6db00-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6db00-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6db00-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="6db00-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6db00-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6db00-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6db00-115">MailboxSettings.ReadWrite</span></span>   |
|<span data-ttu-id="6db00-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6db00-116">Application</span></span> | <span data-ttu-id="6db00-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6db00-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6db00-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6db00-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/masterCategories
POST /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="request-headers"></a><span data-ttu-id="6db00-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6db00-119">Request headers</span></span>
| <span data-ttu-id="6db00-120">Nome</span><span class="sxs-lookup"><span data-stu-id="6db00-120">Name</span></span>       | <span data-ttu-id="6db00-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6db00-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6db00-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6db00-122">Authorization</span></span>  | <span data-ttu-id="6db00-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6db00-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="6db00-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6db00-125">Request body</span></span>
<span data-ttu-id="6db00-126">No corpo da solicitação, forneça uma representação JSON do objeto [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="6db00-126">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6db00-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="6db00-127">Response</span></span>

<span data-ttu-id="6db00-128">Se tiver êxito, este método retornará um código de resposta `201 Created` e o objeto [outlookCategory](../resources/outlookcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6db00-128">If successful, this method returns `201 Created` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6db00-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6db00-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6db00-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6db00-130">Request</span></span>
<span data-ttu-id="6db00-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6db00-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlookcategory_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/masterCategories
Content-type: application/json
Content-Length: 70

{
      "displayName":"Project expenses",
      "color":"preset9"
}
```
<span data-ttu-id="6db00-132">No corpo da solicitação, forneça uma representação JSON do objeto [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="6db00-132">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="6db00-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6db00-133">Response</span></span>
<span data-ttu-id="6db00-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6db00-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 250

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"bac262b7-485d-4739-b436-e31467d64fac",
  "displayName":"Project expenses",
  "color":"preset9"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
