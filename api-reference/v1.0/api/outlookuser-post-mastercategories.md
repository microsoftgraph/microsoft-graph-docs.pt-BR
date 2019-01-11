---
title: Criar categoria do Outlook
description: Cria um objeto outlookCategory na lista mestra de categorias do usuário.
localization_priority: Normal
ms.openlocfilehash: 71bb00d96119b06fda624b02fa9b64be67313f6e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815376"
---
# <a name="create-outlook-category"></a><span data-ttu-id="e7dcd-103">Criar categoria do Outlook</span><span class="sxs-lookup"><span data-stu-id="e7dcd-103">Create Outlook category</span></span>


<span data-ttu-id="e7dcd-104">Cria um objeto [outlookCategory](../resources/outlookcategory.md) na lista mestra de categorias do usuário.</span><span class="sxs-lookup"><span data-stu-id="e7dcd-104">Create an [outlookCategory](../resources/outlookcategory.md) object in the user's master list of categories.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7dcd-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e7dcd-105">Permissions</span></span>
<span data-ttu-id="e7dcd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7dcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7dcd-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7dcd-108">Permission type</span></span>      | <span data-ttu-id="e7dcd-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e7dcd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7dcd-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7dcd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e7dcd-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7dcd-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="e7dcd-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7dcd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7dcd-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7dcd-113">MailboxSettings.ReadWrite</span></span>   |
|<span data-ttu-id="e7dcd-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7dcd-114">Application</span></span> | <span data-ttu-id="e7dcd-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7dcd-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7dcd-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7dcd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/masterCategories
POST /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="request-headers"></a><span data-ttu-id="e7dcd-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7dcd-117">Request headers</span></span>
| <span data-ttu-id="e7dcd-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e7dcd-118">Name</span></span>       | <span data-ttu-id="e7dcd-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7dcd-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e7dcd-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7dcd-120">Authorization</span></span>  | <span data-ttu-id="e7dcd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7dcd-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="e7dcd-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7dcd-123">Request body</span></span>
<span data-ttu-id="e7dcd-124">No corpo da solicitação, forneça uma representação JSON do objeto [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="e7dcd-124">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e7dcd-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7dcd-125">Response</span></span>

<span data-ttu-id="e7dcd-126">Se tiver êxito, este método retornará um código de resposta `201 Created` e o objeto [outlookCategory](../resources/outlookcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7dcd-126">If successful, this method returns `201 Created` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7dcd-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7dcd-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e7dcd-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7dcd-128">Request</span></span>
<span data-ttu-id="e7dcd-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7dcd-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlookcategory_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/outlook/masterCategories
Content-type: application/json
Content-Length: 70

{
      "displayName":"Project expenses",
      "color":"preset9"
}
```
<span data-ttu-id="e7dcd-130">No corpo da solicitação, forneça uma representação JSON do objeto [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="e7dcd-130">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e7dcd-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7dcd-131">Response</span></span>
<span data-ttu-id="e7dcd-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7dcd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
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
