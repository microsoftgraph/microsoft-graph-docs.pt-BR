---
title: Criar ContactFolder
description: 'Cria uma nova contactFolder como um filho de uma pasta especificada. '
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 879c0b642a9db22184617544f9cb9be4a7d29cce
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836292"
---
# <a name="create-contactfolder"></a><span data-ttu-id="cc0e4-103">Criar ContactFolder</span><span class="sxs-lookup"><span data-stu-id="cc0e4-103">Create ContactFolder</span></span>

<span data-ttu-id="cc0e4-104">Cria uma nova contactFolder como um filho de uma pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="cc0e4-104">Create a new contactFolder as a child of a specified folder.</span></span> 

<span data-ttu-id="cc0e4-105">Também é possível [criar uma nova contactFolder sob a pasta de contatos padrão do usuário](user-post-contactfolders.md).</span><span class="sxs-lookup"><span data-stu-id="cc0e4-105">You can also [create a new contactFolder under the user's default contact folder](user-post-contactfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="cc0e4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cc0e4-106">Permissions</span></span>
<span data-ttu-id="cc0e4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc0e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc0e4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc0e4-109">Permission type</span></span>      | <span data-ttu-id="cc0e4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cc0e4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc0e4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc0e4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cc0e4-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cc0e4-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="cc0e4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc0e4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc0e4-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cc0e4-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="cc0e4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc0e4-115">Application</span></span> | <span data-ttu-id="cc0e4-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cc0e4-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc0e4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc0e4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="request-headers"></a><span data-ttu-id="cc0e4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc0e4-118">Request headers</span></span>
| <span data-ttu-id="cc0e4-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cc0e4-119">Header</span></span>       | <span data-ttu-id="cc0e4-120">Valor</span><span class="sxs-lookup"><span data-stu-id="cc0e4-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cc0e4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc0e4-121">Authorization</span></span>  | <span data-ttu-id="cc0e4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc0e4-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cc0e4-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cc0e4-124">Content-Type</span></span>  | <span data-ttu-id="cc0e4-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc0e4-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cc0e4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc0e4-127">Request body</span></span>
<span data-ttu-id="cc0e4-128">No corpo da solicitação, forneça uma representação JSON do objeto [ContactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="cc0e4-128">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cc0e4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc0e4-129">Response</span></span>

<span data-ttu-id="cc0e4-130">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [ContactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cc0e4-130">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc0e4-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cc0e4-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cc0e4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc0e4-132">Request</span></span>
<span data-ttu-id="cc0e4-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc0e4-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_contactfolder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/contactFolders/{id}/childFolders
Content-type: application/json
Content-length: 84

{
  "displayName": "displayName-value"
}
```
<span data-ttu-id="cc0e4-134">No corpo da solicitação, forneça uma representação JSON do objeto [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="cc0e4-134">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="cc0e4-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc0e4-135">Response</span></span>
<span data-ttu-id="cc0e4-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cc0e4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
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
