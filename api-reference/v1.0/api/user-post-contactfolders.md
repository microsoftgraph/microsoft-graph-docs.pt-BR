---
title: Criar ContactFolder
description: Crie uma nova contactFolder sob a pasta de contatos padrão do usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 76f7f7592657e913322343426c07575344fc4d68
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473546"
---
# <a name="create-contactfolder"></a><span data-ttu-id="9db52-103">Criar ContactFolder</span><span class="sxs-lookup"><span data-stu-id="9db52-103">Create ContactFolder</span></span>

<span data-ttu-id="9db52-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9db52-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9db52-105">Crie uma nova contactFolder sob a pasta de contatos padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="9db52-105">Create a new contactFolder under the user's default contacts folder.</span></span>

<span data-ttu-id="9db52-106">Você também pode [criar uma nova contactfolder como um filho de qualquer pasta de contatos especificada](contactfolder-post-childfolders.md).</span><span class="sxs-lookup"><span data-stu-id="9db52-106">You can also [create a new contactfolder as a child of any specified contact folder](contactfolder-post-childfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="9db52-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="9db52-107">Permissions</span></span>
<span data-ttu-id="9db52-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9db52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9db52-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9db52-110">Permission type</span></span>      | <span data-ttu-id="9db52-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9db52-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9db52-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9db52-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9db52-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9db52-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="9db52-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9db52-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9db52-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9db52-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="9db52-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9db52-116">Application</span></span> | <span data-ttu-id="9db52-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9db52-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9db52-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9db52-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders
POST /users/{id | userPrincipalName}/contactFolders
```
## <a name="request-headers"></a><span data-ttu-id="9db52-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9db52-119">Request headers</span></span>
| <span data-ttu-id="9db52-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9db52-120">Header</span></span>       | <span data-ttu-id="9db52-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9db52-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9db52-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9db52-122">Authorization</span></span>  | <span data-ttu-id="9db52-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9db52-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9db52-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9db52-125">Content-Type</span></span>  | <span data-ttu-id="9db52-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9db52-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9db52-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9db52-127">Request body</span></span>
<span data-ttu-id="9db52-128">No corpo da solicitação, forneça uma representação JSON do objeto [ContactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="9db52-128">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9db52-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9db52-129">Response</span></span>

<span data-ttu-id="9db52-130">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [ContactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9db52-130">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9db52-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9db52-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="9db52-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9db52-132">Request</span></span>
<span data-ttu-id="9db52-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9db52-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/contactFolders
Content-type: application/json

{
  "parentFolderId": "AQMkADIxYjJiYgEzLTFmNjYALTRjYTMtODA1NC0wZDkxZGNmOTcxNTQALgAAA8RJzXYaLKZPlmn0ge0edZkBADa3qi2IMXRNg6RwQSHe_F8AAAIBDgAAAA==",
  "displayName": "Important contacts"
}
```

<span data-ttu-id="9db52-134">No corpo da solicitação, forneça uma representação JSON do objeto [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="9db52-134">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
### <a name="response"></a><span data-ttu-id="9db52-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9db52-135">Response</span></span>
<span data-ttu-id="9db52-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9db52-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "parentFolderId": "AQMkADIxYjJiYgEzLTFmNjYALTRjYTMtODA1NC0wZDkxZGNmOTcxNTQALgAAA8RJzXYaLKZPlmn0ge0edZkBADa3qi2IMXRNg6RwQSHe_F8AAAIBDgAAAA==",
  "displayName": "Important contacts",
  "id": "AAMkADIxYjJiYmIzLTFmNjYtNGNhMy04MDU0LTBkOTFkY2Y5NzE1NAAuAAAAAADESc12GiymT5Zp9IHtHnWZAQA2t6otiDF0TYOkcEEh3vhfAAAGgUC1AAA="
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ContactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

