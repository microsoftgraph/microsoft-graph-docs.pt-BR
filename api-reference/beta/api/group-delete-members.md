---
title: Remover membro
description: Use esta API para remover um membro de um grupo do Office 365, de um grupo de segurança ou de um grupo de segurança habilitado para email através da propriedade de navegação **membros**. É possível remover usuários ou outros grupos.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 0b985a5bc7c70e55a4e5ecfcc395595b7041fa30
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329612"
---
# <a name="remove-member"></a><span data-ttu-id="42070-104">Remover membro</span><span class="sxs-lookup"><span data-stu-id="42070-104">Remove member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42070-p102">Use esta API para remover um membro de um grupo do Office 365, de um grupo de segurança ou de um grupo de segurança habilitado para email através da propriedade de navegação **membros**. É possível remover usuários ou outros grupos.</span><span class="sxs-lookup"><span data-stu-id="42070-p102">Use this API to remove a member from an Office 365 group, a security group, or a mail-enabled security group through the **members** navigation property. You can remove users or other groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="42070-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="42070-107">Permissions</span></span>
<span data-ttu-id="42070-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42070-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42070-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42070-110">Permission type</span></span>      | <span data-ttu-id="42070-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="42070-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42070-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42070-112">Delegated (work or school account)</span></span> | <span data-ttu-id="42070-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="42070-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="42070-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42070-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42070-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42070-115">Not supported.</span></span>    |
|<span data-ttu-id="42070-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42070-116">Application</span></span> | <span data-ttu-id="42070-117">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42070-117">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="42070-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42070-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="42070-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42070-119">Request headers</span></span>
| <span data-ttu-id="42070-120">Nome</span><span class="sxs-lookup"><span data-stu-id="42070-120">Name</span></span>       | <span data-ttu-id="42070-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="42070-121">Type</span></span> | <span data-ttu-id="42070-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="42070-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="42070-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="42070-123">Authorization</span></span>  | <span data-ttu-id="42070-124">string</span><span class="sxs-lookup"><span data-stu-id="42070-124">string</span></span>  | <span data-ttu-id="42070-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42070-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42070-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42070-127">Request body</span></span>
<span data-ttu-id="42070-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="42070-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42070-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="42070-129">Response</span></span>
<span data-ttu-id="42070-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42070-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42070-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42070-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="42070-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42070-133">Request</span></span>
<span data-ttu-id="42070-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="42070-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/members/{id}/$ref
```
<span data-ttu-id="42070-135">Na solicitação, especifique a `id` do objeto diretório que deseja remover após o segmento $ref.</span><span class="sxs-lookup"><span data-stu-id="42070-135">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="42070-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="42070-136">Response</span></span>
<span data-ttu-id="42070-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="42070-137">The following is an example of the response.</span></span>
><span data-ttu-id="42070-138">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="42070-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="42070-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42070-139">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
