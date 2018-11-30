---
title: Criar categoria do Outlook
description: Cria um objeto outlookCategory na lista mestra de categorias do usuário.
ms.openlocfilehash: a3b948b7996a54676e98d348b5777e831c92d298
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033367"
---
# <a name="create-outlook-category"></a><span data-ttu-id="a1d59-103">Criar categoria do Outlook</span><span class="sxs-lookup"><span data-stu-id="a1d59-103">Create Outlook category</span></span>

> <span data-ttu-id="a1d59-104">**Importante**: APIs sob a versão /beta no Microsoft Graph estiver em Visualizar e estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="a1d59-104">**Important**: APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1d59-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a1d59-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a1d59-106">Cria um objeto [outlookCategory](../resources/outlookcategory.md) na lista mestra de categorias do usuário.</span><span class="sxs-lookup"><span data-stu-id="a1d59-106">Create an [outlookCategory](../resources/outlookcategory.md) object in the user's master list of categories.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1d59-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a1d59-107">Permissions</span></span>
<span data-ttu-id="a1d59-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1d59-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1d59-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1d59-110">Permission type</span></span>      | <span data-ttu-id="a1d59-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a1d59-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1d59-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1d59-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a1d59-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1d59-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="a1d59-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1d59-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1d59-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1d59-115">MailboxSettings.ReadWrite</span></span>   |
|<span data-ttu-id="a1d59-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1d59-116">Application</span></span> | <span data-ttu-id="a1d59-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1d59-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1d59-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1d59-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/masterCategories
POST /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="request-headers"></a><span data-ttu-id="a1d59-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1d59-119">Request headers</span></span>
| <span data-ttu-id="a1d59-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a1d59-120">Name</span></span>       | <span data-ttu-id="a1d59-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1d59-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a1d59-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1d59-122">Authorization</span></span>  | <span data-ttu-id="a1d59-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1d59-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="a1d59-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1d59-125">Request body</span></span>
<span data-ttu-id="a1d59-126">No corpo da solicitação, forneça uma representação JSON do objeto [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="a1d59-126">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a1d59-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1d59-127">Response</span></span>

<span data-ttu-id="a1d59-128">Se tiver êxito, este método retornará um código de resposta `201 Created` e o objeto [outlookCategory](../resources/outlookcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1d59-128">If successful, this method returns `201 Created` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1d59-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1d59-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a1d59-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1d59-130">Request</span></span>
<span data-ttu-id="a1d59-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1d59-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="a1d59-132">No corpo da solicitação, forneça uma representação JSON do objeto [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="a1d59-132">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a1d59-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1d59-133">Response</span></span>
<span data-ttu-id="a1d59-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1d59-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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