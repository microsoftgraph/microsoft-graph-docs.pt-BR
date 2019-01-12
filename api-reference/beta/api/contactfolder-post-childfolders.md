---
title: Criar ContactFolder
description: 'Cria uma nova contactFolder como um filho de uma pasta especificada. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 66061d86b3c3894c165788cd408b22b8824b34f9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991766"
---
# <a name="create-contactfolder"></a><span data-ttu-id="3b584-103">Criar ContactFolder</span><span class="sxs-lookup"><span data-stu-id="3b584-103">Create ContactFolder</span></span>

> <span data-ttu-id="3b584-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3b584-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b584-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3b584-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3b584-106">Cria uma nova contactFolder como um filho de uma pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="3b584-106">Create a new contactFolder as a child of a specified folder.</span></span> 

<span data-ttu-id="3b584-107">Também é possível [criar uma nova contactFolder sob a pasta de contatos padrão do usuário](user-post-contactfolders.md).</span><span class="sxs-lookup"><span data-stu-id="3b584-107">You can also [create a new contactFolder under the user's default contact folder](user-post-contactfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="3b584-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="3b584-108">Permissions</span></span>
<span data-ttu-id="3b584-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b584-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b584-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b584-111">Permission type</span></span>      | <span data-ttu-id="3b584-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3b584-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b584-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b584-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3b584-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3b584-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="3b584-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b584-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b584-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3b584-116">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="3b584-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b584-117">Application</span></span> | <span data-ttu-id="3b584-118">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3b584-118">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b584-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b584-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="request-headers"></a><span data-ttu-id="3b584-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b584-120">Request headers</span></span>
| <span data-ttu-id="3b584-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3b584-121">Header</span></span>       | <span data-ttu-id="3b584-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3b584-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3b584-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b584-123">Authorization</span></span>  | <span data-ttu-id="3b584-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b584-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3b584-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3b584-126">Content-Type</span></span>  | <span data-ttu-id="3b584-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b584-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3b584-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b584-129">Request body</span></span>
<span data-ttu-id="3b584-130">No corpo da solicitação, forneça uma representação JSON do objeto [ContactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="3b584-130">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3b584-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b584-131">Response</span></span>

<span data-ttu-id="3b584-132">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [ContactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b584-132">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b584-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b584-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3b584-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b584-134">Request</span></span>
<span data-ttu-id="3b584-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b584-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_contactfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/contactFolders/{id}/childFolders
Content-type: application/json
Content-length: 84

{
  "displayName": "displayName-value"
}
```
<span data-ttu-id="3b584-136">No corpo da solicitação, forneça uma representação JSON do objeto [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="3b584-136">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3b584-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b584-137">Response</span></span>
<span data-ttu-id="3b584-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b584-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
