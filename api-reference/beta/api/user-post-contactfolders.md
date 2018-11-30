---
title: Criar ContactFolder
description: Crie uma nova contactFolder sob a pasta de contatos padrão do usuário.
ms.openlocfilehash: 0d8e76c62d0e5265656bc953696d613d2c59675a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040285"
---
# <a name="create-contactfolder"></a><span data-ttu-id="5486d-103">Criar ContactFolder</span><span class="sxs-lookup"><span data-stu-id="5486d-103">Create ContactFolder</span></span>

> <span data-ttu-id="5486d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5486d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5486d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5486d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5486d-106">Crie uma nova contactFolder sob a pasta de contatos padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="5486d-106">Create a new contactFolder under the user's default contacts folder.</span></span>

<span data-ttu-id="5486d-107">Você também pode [criar uma nova contactfolder como um filho de qualquer pasta de contatos especificada](contactfolder-post-childfolders.md).</span><span class="sxs-lookup"><span data-stu-id="5486d-107">You can also [create a new contactfolder as a child of any specified contact folder](contactfolder-post-childfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="5486d-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="5486d-108">Permissions</span></span>
<span data-ttu-id="5486d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5486d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5486d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5486d-111">Permission type</span></span>      | <span data-ttu-id="5486d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5486d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5486d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5486d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5486d-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5486d-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="5486d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5486d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5486d-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5486d-116">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="5486d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5486d-117">Application</span></span> | <span data-ttu-id="5486d-118">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5486d-118">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5486d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5486d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/contactFolders
```
## <a name="request-headers"></a><span data-ttu-id="5486d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5486d-120">Request headers</span></span>
| <span data-ttu-id="5486d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5486d-121">Header</span></span>       | <span data-ttu-id="5486d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5486d-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5486d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5486d-123">Authorization</span></span>  | <span data-ttu-id="5486d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5486d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5486d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5486d-126">Content-Type</span></span>  | <span data-ttu-id="5486d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5486d-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5486d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5486d-128">Request body</span></span>
<span data-ttu-id="5486d-129">No corpo da solicitação, forneça uma representação JSON do objeto [ContactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="5486d-129">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5486d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5486d-130">Response</span></span>

<span data-ttu-id="5486d-131">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [ContactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5486d-131">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5486d-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5486d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5486d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5486d-133">Request</span></span>
<span data-ttu-id="5486d-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5486d-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/contactFolders
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
<span data-ttu-id="5486d-135">No corpo da solicitação, forneça uma representação JSON do objeto [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="5486d-135">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="5486d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5486d-136">Response</span></span>
<span data-ttu-id="5486d-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5486d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
