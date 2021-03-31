---
title: Criar ContactFolder
description: 'Cria uma nova contactFolder como um filho de uma pasta especificada. '
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4dea9aedecdacf6aff8e939a44d837d30928357b
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473245"
---
# <a name="create-contactfolder"></a><span data-ttu-id="961ef-103">Criar ContactFolder</span><span class="sxs-lookup"><span data-stu-id="961ef-103">Create ContactFolder</span></span>

<span data-ttu-id="961ef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="961ef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="961ef-105">Cria uma nova contactFolder como um filho de uma pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="961ef-105">Create a new contactFolder as a child of a specified folder.</span></span> 

<span data-ttu-id="961ef-106">Também é possível [criar uma nova contactFolder sob a pasta de contatos padrão do usuário](user-post-contactfolders.md).</span><span class="sxs-lookup"><span data-stu-id="961ef-106">You can also [create a new contactFolder under the user's default contact folder](user-post-contactfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="961ef-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="961ef-107">Permissions</span></span>
<span data-ttu-id="961ef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="961ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="961ef-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="961ef-110">Permission type</span></span>      | <span data-ttu-id="961ef-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="961ef-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="961ef-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="961ef-112">Delegated (work or school account)</span></span> | <span data-ttu-id="961ef-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="961ef-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="961ef-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="961ef-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="961ef-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="961ef-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="961ef-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="961ef-116">Application</span></span> | <span data-ttu-id="961ef-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="961ef-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="961ef-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="961ef-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="request-headers"></a><span data-ttu-id="961ef-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="961ef-119">Request headers</span></span>
| <span data-ttu-id="961ef-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="961ef-120">Header</span></span>       | <span data-ttu-id="961ef-121">Valor</span><span class="sxs-lookup"><span data-stu-id="961ef-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="961ef-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="961ef-122">Authorization</span></span>  | <span data-ttu-id="961ef-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="961ef-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="961ef-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="961ef-125">Content-Type</span></span>  | <span data-ttu-id="961ef-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="961ef-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="961ef-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="961ef-128">Request body</span></span>
<span data-ttu-id="961ef-129">No corpo da solicitação, forneça uma representação JSON do objeto [ContactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="961ef-129">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="961ef-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="961ef-130">Response</span></span>

<span data-ttu-id="961ef-131">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [ContactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="961ef-131">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="961ef-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="961ef-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="961ef-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="961ef-133">Request</span></span>

<span data-ttu-id="961ef-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="961ef-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_contactfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/contactFolders/{id}/childFolders
Content-type: application/json

{
  "displayName": "Family"
}
```

<span data-ttu-id="961ef-135">No corpo da solicitação, forneça uma representação JSON do objeto [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="961ef-135">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="961ef-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="961ef-136">Response</span></span>

<span data-ttu-id="961ef-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="961ef-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "parentFolderId": "AQMkADIxYjJiYgEzLTFmNjYALTRjYTMtODA1NC0wZDkxZGNmOTcxNTQALgAAA8RJzXYaLKZPlmn0ge0edZkBADa3qi2IMXRNg6RwQSHe_F8AAAIBDgAAAA==",
  "displayName": "Family",
  "id": "AAMkADIxYjJiYmIzLTFmNjYtNGNhMy04MDU0LTBkOTFkY2Y5NzE1NAAuAAAAAADESc12GiymT5Zp9IHtHnWZAQA2t6otiDF0TYOkcEEh3vhfAAAGgUC1AAA="
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create ContactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


