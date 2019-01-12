---
title: Criar ContactFolder
description: Crie uma nova contactFolder sob a pasta de contatos padrão do usuário.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2e76da12d152a28f5f8579d41f1cf3e159b0e078
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921672"
---
# <a name="create-contactfolder"></a><span data-ttu-id="fc847-103">Criar ContactFolder</span><span class="sxs-lookup"><span data-stu-id="fc847-103">Create ContactFolder</span></span>

<span data-ttu-id="fc847-104">Crie uma nova contactFolder sob a pasta de contatos padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="fc847-104">Create a new contactFolder under the user's default contacts folder.</span></span>

<span data-ttu-id="fc847-105">Você também pode [criar uma nova contactfolder como um filho de qualquer pasta de contatos especificada](contactfolder-post-childfolders.md).</span><span class="sxs-lookup"><span data-stu-id="fc847-105">You can also [create a new contactfolder as a child of any specified contact folder](contactfolder-post-childfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="fc847-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fc847-106">Permissions</span></span>
<span data-ttu-id="fc847-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc847-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc847-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc847-109">Permission type</span></span>      | <span data-ttu-id="fc847-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fc847-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc847-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc847-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fc847-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc847-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="fc847-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc847-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc847-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc847-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="fc847-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc847-115">Application</span></span> | <span data-ttu-id="fc847-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc847-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc847-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc847-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/contactFolders
```
## <a name="request-headers"></a><span data-ttu-id="fc847-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc847-118">Request headers</span></span>
| <span data-ttu-id="fc847-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fc847-119">Header</span></span>       | <span data-ttu-id="fc847-120">Valor</span><span class="sxs-lookup"><span data-stu-id="fc847-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fc847-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc847-121">Authorization</span></span>  | <span data-ttu-id="fc847-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc847-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fc847-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fc847-124">Content-Type</span></span>  | <span data-ttu-id="fc847-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fc847-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fc847-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc847-126">Request body</span></span>
<span data-ttu-id="fc847-127">No corpo da solicitação, forneça uma representação JSON do objeto [ContactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="fc847-127">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fc847-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc847-128">Response</span></span>

<span data-ttu-id="fc847-129">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [ContactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc847-129">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc847-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fc847-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fc847-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc847-131">Request</span></span>
<span data-ttu-id="fc847-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc847-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/contactFolders
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
<span data-ttu-id="fc847-133">No corpo da solicitação, forneça uma representação JSON do objeto [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="fc847-133">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="fc847-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc847-134">Response</span></span>
<span data-ttu-id="fc847-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fc847-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 104

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ContactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
