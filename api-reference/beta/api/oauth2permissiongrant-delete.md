---
title: Excluir oAuth2PermissionGrant
description: Exclua um oAuth2PermissionGrant.
localization_priority: Normal
ms.openlocfilehash: 8eed0c8d2179af6fe199137cfeb7e386a97f733c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813815"
---
# <a name="delete-oauth2permissiongrant"></a><span data-ttu-id="e67b0-103">Excluir oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="e67b0-103">Delete oAuth2PermissionGrant</span></span>

> <span data-ttu-id="e67b0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e67b0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e67b0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e67b0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e67b0-106">Exclua um oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="e67b0-106">Delete an oAuth2PermissionGrant.</span></span>

## <a name="permissions"></a><span data-ttu-id="e67b0-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="e67b0-107">Permissions</span></span>
<span data-ttu-id="e67b0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e67b0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e67b0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e67b0-110">Permission type</span></span>      | <span data-ttu-id="e67b0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e67b0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e67b0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e67b0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e67b0-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e67b0-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e67b0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e67b0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e67b0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e67b0-115">Not supported.</span></span>    |
|<span data-ttu-id="e67b0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e67b0-116">Application</span></span> | <span data-ttu-id="e67b0-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e67b0-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e67b0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e67b0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /oAuth2Permissiongrants/{id}
DELETE /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
DELETE /drive/root/createdByUser/oAuth2Permissiongrants/{id}

```
## <a name="request-headers"></a><span data-ttu-id="e67b0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e67b0-119">Request headers</span></span>
| <span data-ttu-id="e67b0-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e67b0-120">Name</span></span>       | <span data-ttu-id="e67b0-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="e67b0-121">Type</span></span> | <span data-ttu-id="e67b0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e67b0-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e67b0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e67b0-123">Authorization</span></span>  | <span data-ttu-id="e67b0-124">string</span><span class="sxs-lookup"><span data-stu-id="e67b0-124">string</span></span>  | <span data-ttu-id="e67b0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e67b0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e67b0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e67b0-127">Request body</span></span>
<span data-ttu-id="e67b0-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e67b0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e67b0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e67b0-129">Response</span></span>

<span data-ttu-id="e67b0-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e67b0-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e67b0-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e67b0-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e67b0-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e67b0-133">Request</span></span>
<span data-ttu-id="e67b0-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e67b0-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_oAuth2Permissiongrant"
}-->
```http
DELETE https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
```
##### <a name="response"></a><span data-ttu-id="e67b0-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e67b0-135">Response</span></span>
<span data-ttu-id="e67b0-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e67b0-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete oAuth2Permissiongrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
