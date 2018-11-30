---
title: Criar MailFolder
description: Use essa API para criar uma nova pasta de email na pasta raiz da caixa de correio do usuário.
ms.openlocfilehash: 6e6b42197dcb5b968a59303d2e9c8c8b1ddf6feb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039588"
---
# <a name="create-mailfolder"></a><span data-ttu-id="63f43-103">Criar MailFolder</span><span class="sxs-lookup"><span data-stu-id="63f43-103">Create MailFolder</span></span>

> <span data-ttu-id="63f43-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="63f43-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="63f43-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="63f43-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="63f43-106">Use essa API para criar uma nova pasta de email na pasta raiz da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="63f43-106">Use this API to create a new mail folder in the root folder of the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="63f43-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="63f43-107">Permissions</span></span>
<span data-ttu-id="63f43-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63f43-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63f43-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63f43-110">Permission type</span></span>      | <span data-ttu-id="63f43-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="63f43-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63f43-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63f43-112">Delegated (work or school account)</span></span> | <span data-ttu-id="63f43-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="63f43-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="63f43-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63f43-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63f43-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="63f43-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="63f43-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63f43-116">Application</span></span> | <span data-ttu-id="63f43-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="63f43-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="63f43-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63f43-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/mailFolders
```
## <a name="request-headers"></a><span data-ttu-id="63f43-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63f43-119">Request headers</span></span>
| <span data-ttu-id="63f43-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="63f43-120">Header</span></span>       | <span data-ttu-id="63f43-121">Valor</span><span class="sxs-lookup"><span data-stu-id="63f43-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="63f43-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="63f43-122">Authorization</span></span>  | <span data-ttu-id="63f43-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63f43-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="63f43-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="63f43-125">Content-Type</span></span>  | <span data-ttu-id="63f43-126">application/json</span><span class="sxs-lookup"><span data-stu-id="63f43-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="63f43-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63f43-127">Request body</span></span>
<span data-ttu-id="63f43-p104">No corpo da solicitação, forneça um objeto JSON com os parâmetros a seguir. **displayName** é a única propriedade gravável para um objeto [MailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="63f43-p104">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="63f43-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="63f43-130">Parameter</span></span>    | <span data-ttu-id="63f43-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="63f43-131">Type</span></span>   |<span data-ttu-id="63f43-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="63f43-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63f43-133">displayName</span><span class="sxs-lookup"><span data-stu-id="63f43-133">displayName</span></span>|<span data-ttu-id="63f43-134">String</span><span class="sxs-lookup"><span data-stu-id="63f43-134">String</span></span>|<span data-ttu-id="63f43-135">O nome de exibição da nova pasta.</span><span class="sxs-lookup"><span data-stu-id="63f43-135">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="63f43-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="63f43-136">Response</span></span>

<span data-ttu-id="63f43-137">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [MailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63f43-137">If successful, this method returns `201 Created` response code and a [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63f43-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63f43-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="63f43-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63f43-139">Request</span></span>
<span data-ttu-id="63f43-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63f43-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/mailFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value"
}
```

##### <a name="response"></a><span data-ttu-id="63f43-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="63f43-141">Response</span></span>
<span data-ttu-id="63f43-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="63f43-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
