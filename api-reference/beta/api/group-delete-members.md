---
title: Remover membro
description: Use esta API para remover um membro de um grupo do Office 365, de um grupo de segurança ou de um grupo de segurança habilitado para email através da propriedade de navegação **membros**. É possível remover usuários ou outros grupos.
ms.openlocfilehash: be011101208d33293906ab7c8e79e242ca4c8f9f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034301"
---
# <a name="remove-member"></a><span data-ttu-id="f35fd-104">Remover membro</span><span class="sxs-lookup"><span data-stu-id="f35fd-104">Remove member</span></span>

> <span data-ttu-id="f35fd-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f35fd-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f35fd-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f35fd-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f35fd-p103">Use esta API para remover um membro de um grupo do Office 365, de um grupo de segurança ou de um grupo de segurança habilitado para email através da propriedade de navegação **membros**. É possível remover usuários ou outros grupos.</span><span class="sxs-lookup"><span data-stu-id="f35fd-p103">Use this API to remove a member from an Office 365 group, a security group, or a mail-enabled security group through the **members** navigation property. You can remove users or other groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="f35fd-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="f35fd-109">Permissions</span></span>
<span data-ttu-id="f35fd-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f35fd-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f35fd-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f35fd-112">Permission type</span></span>      | <span data-ttu-id="f35fd-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f35fd-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f35fd-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f35fd-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f35fd-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f35fd-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f35fd-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f35fd-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f35fd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f35fd-117">Not supported.</span></span>    |
|<span data-ttu-id="f35fd-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f35fd-118">Application</span></span> | <span data-ttu-id="f35fd-119">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f35fd-119">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f35fd-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f35fd-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="f35fd-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f35fd-121">Request headers</span></span>
| <span data-ttu-id="f35fd-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f35fd-122">Name</span></span>       | <span data-ttu-id="f35fd-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="f35fd-123">Type</span></span> | <span data-ttu-id="f35fd-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f35fd-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f35fd-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f35fd-125">Authorization</span></span>  | <span data-ttu-id="f35fd-126">string</span><span class="sxs-lookup"><span data-stu-id="f35fd-126">string</span></span>  | <span data-ttu-id="f35fd-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f35fd-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f35fd-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f35fd-129">Request body</span></span>
<span data-ttu-id="f35fd-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f35fd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f35fd-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f35fd-131">Response</span></span>
<span data-ttu-id="f35fd-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f35fd-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f35fd-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f35fd-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f35fd-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f35fd-135">Request</span></span>
<span data-ttu-id="f35fd-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f35fd-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/members/{id}/$ref
```
<span data-ttu-id="f35fd-137">Na solicitação, especifique a `id` do objeto diretório que deseja remover após o segmento $ref.</span><span class="sxs-lookup"><span data-stu-id="f35fd-137">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="f35fd-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f35fd-138">Response</span></span>
<span data-ttu-id="f35fd-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f35fd-139">The following is an example of the response.</span></span>
><span data-ttu-id="f35fd-140">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f35fd-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f35fd-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f35fd-141">All the properties will be returned from an actual call.</span></span>
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
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
