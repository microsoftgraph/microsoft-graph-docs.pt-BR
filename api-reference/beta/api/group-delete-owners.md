---
title: Remover proprietário
description: Use esta API para remover um proprietário de um grupo do Office 365, de um grupo de segurança ou de um grupo de segurança habilitado para email através da propriedade de navegação owners.
ms.openlocfilehash: 7ed56ae78f99c583e382b25652702f4189b7842e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037667"
---
# <a name="remove-owner"></a><span data-ttu-id="4801b-103">Remover proprietário</span><span class="sxs-lookup"><span data-stu-id="4801b-103">Remove owner</span></span>

> <span data-ttu-id="4801b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4801b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4801b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4801b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4801b-106">Use esta API para remover um proprietário de um grupo do Office 365, de um grupo de segurança ou de um grupo de segurança habilitado para email através da propriedade de navegação owners.</span><span class="sxs-lookup"><span data-stu-id="4801b-106">Use this API to remove an owner from an Office 365 group, a security group, or a mail-enabled security group through the owners navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="4801b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="4801b-107">Permissions</span></span>
<span data-ttu-id="4801b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4801b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4801b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4801b-110">Permission type</span></span>      | <span data-ttu-id="4801b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4801b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4801b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4801b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4801b-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4801b-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4801b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4801b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4801b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4801b-115">Not supported.</span></span>    |
|<span data-ttu-id="4801b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4801b-116">Application</span></span> | <span data-ttu-id="4801b-117">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4801b-117">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4801b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4801b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="4801b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4801b-119">Request headers</span></span>
| <span data-ttu-id="4801b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="4801b-120">Name</span></span>       | <span data-ttu-id="4801b-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="4801b-121">Type</span></span> | <span data-ttu-id="4801b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4801b-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4801b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4801b-123">Authorization</span></span>  | <span data-ttu-id="4801b-124">string</span><span class="sxs-lookup"><span data-stu-id="4801b-124">string</span></span>  | <span data-ttu-id="4801b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4801b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4801b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4801b-127">Request body</span></span>
<span data-ttu-id="4801b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4801b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4801b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4801b-129">Response</span></span>
<span data-ttu-id="4801b-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4801b-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4801b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4801b-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4801b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4801b-133">Request</span></span>
<span data-ttu-id="4801b-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4801b-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/owners/{id}/$ref
```
<span data-ttu-id="4801b-135">Na solicitação, especifique a `id` do objeto diretório que deseja remover após o segmento $ref.</span><span class="sxs-lookup"><span data-stu-id="4801b-135">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="4801b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4801b-136">Response</span></span>
<span data-ttu-id="4801b-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4801b-137">The following is an example of the response.</span></span>
><span data-ttu-id="4801b-138">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4801b-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4801b-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4801b-139">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->