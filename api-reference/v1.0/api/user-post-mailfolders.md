---
title: Criar MailFolder
description: Use essa API para criar uma nova pasta de email na pasta raiz da caixa de correio do usuário.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c2f845f2a332c7e9c7a637839727fe7b82e50a46
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573589"
---
# <a name="create-mailfolder"></a><span data-ttu-id="36cfd-103">Criar MailFolder</span><span class="sxs-lookup"><span data-stu-id="36cfd-103">Create MailFolder</span></span>

<span data-ttu-id="36cfd-104">Use essa API para criar uma nova pasta de email na pasta raiz da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="36cfd-104">Use this API to create a new mail folder in the root folder of the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="36cfd-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="36cfd-105">Permissions</span></span>
<span data-ttu-id="36cfd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36cfd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36cfd-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36cfd-108">Permission type</span></span>      | <span data-ttu-id="36cfd-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="36cfd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36cfd-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36cfd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="36cfd-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36cfd-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="36cfd-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36cfd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36cfd-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36cfd-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="36cfd-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36cfd-114">Application</span></span> | <span data-ttu-id="36cfd-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36cfd-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="36cfd-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36cfd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders
POST /users/{id | userPrincipalName}/mailFolders
```
## <a name="request-headers"></a><span data-ttu-id="36cfd-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36cfd-117">Request headers</span></span>
| <span data-ttu-id="36cfd-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="36cfd-118">Header</span></span>       | <span data-ttu-id="36cfd-119">Valor</span><span class="sxs-lookup"><span data-stu-id="36cfd-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="36cfd-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="36cfd-120">Authorization</span></span>  | <span data-ttu-id="36cfd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36cfd-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="36cfd-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="36cfd-123">Content-Type</span></span>  | <span data-ttu-id="36cfd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="36cfd-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="36cfd-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36cfd-125">Request body</span></span>
<span data-ttu-id="36cfd-p103">No corpo da solicitação, forneça um objeto JSON com os parâmetros a seguir. **displayName** é a única propriedade gravável para um objeto [MailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="36cfd-p103">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="36cfd-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="36cfd-128">Parameter</span></span>    | <span data-ttu-id="36cfd-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="36cfd-129">Type</span></span>   |<span data-ttu-id="36cfd-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="36cfd-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36cfd-131">displayName</span><span class="sxs-lookup"><span data-stu-id="36cfd-131">displayName</span></span>|<span data-ttu-id="36cfd-132">String</span><span class="sxs-lookup"><span data-stu-id="36cfd-132">String</span></span>|<span data-ttu-id="36cfd-133">O nome de exibição da nova pasta.</span><span class="sxs-lookup"><span data-stu-id="36cfd-133">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="36cfd-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="36cfd-134">Response</span></span>

<span data-ttu-id="36cfd-135">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [MailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36cfd-135">If successful, this method returns `201 Created` response code and a [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36cfd-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="36cfd-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36cfd-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36cfd-137">Request</span></span>
<span data-ttu-id="36cfd-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="36cfd-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value"
}
```

##### <a name="response"></a><span data-ttu-id="36cfd-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="36cfd-139">Response</span></span>
<span data-ttu-id="36cfd-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="36cfd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create MailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
