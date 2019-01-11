---
title: Adicionar membro
description: Use esta API para adicionar um membro a um grupo do Office 365, a um grupo de segurança ou a um grupo de segurança habilitado para email através da propriedade de navegação **owners**.
localization_priority: Normal
ms.openlocfilehash: 74ad07ea9012385f896ba4c6c6aa18f44758e5bb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832862"
---
# <a name="add-member"></a><span data-ttu-id="cafd4-103">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="cafd4-103">Add member</span></span>

> <span data-ttu-id="cafd4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cafd4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cafd4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cafd4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cafd4-106">Use esta API para adicionar um membro a um grupo do Office 365, a um grupo de segurança ou a um grupo de segurança habilitado para email através da propriedade de navegação **owners**.</span><span class="sxs-lookup"><span data-stu-id="cafd4-106">Use this API to add a member to an Office 365 Group, a security group, or a mail-enabled security group through the **members** navigation property.</span></span>

<span data-ttu-id="cafd4-107">É possível adicionar usuários ou outros grupos.</span><span class="sxs-lookup"><span data-stu-id="cafd4-107">You can add users or other groups.</span></span> <span data-ttu-id="cafd4-108">Importante: só é possível adicionar usuários a grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="cafd4-108">Important: You can add only users to Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="cafd4-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="cafd4-109">Permissions</span></span>
<span data-ttu-id="cafd4-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cafd4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cafd4-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cafd4-112">Permission type</span></span>      | <span data-ttu-id="cafd4-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cafd4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cafd4-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cafd4-114">Delegated (work or school account)</span></span> | <span data-ttu-id="cafd4-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cafd4-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cafd4-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cafd4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cafd4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cafd4-117">Not supported.</span></span>    |
|<span data-ttu-id="cafd4-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cafd4-118">Application</span></span> | <span data-ttu-id="cafd4-119">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cafd4-119">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cafd4-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cafd4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="cafd4-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cafd4-121">Request headers</span></span>
| <span data-ttu-id="cafd4-122">Nome</span><span class="sxs-lookup"><span data-stu-id="cafd4-122">Name</span></span>       | <span data-ttu-id="cafd4-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="cafd4-123">Type</span></span> | <span data-ttu-id="cafd4-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="cafd4-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cafd4-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="cafd4-125">Authorization</span></span>  | <span data-ttu-id="cafd4-126">string</span><span class="sxs-lookup"><span data-stu-id="cafd4-126">string</span></span>  | <span data-ttu-id="cafd4-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cafd4-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cafd4-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cafd4-129">Request body</span></span>
<span data-ttu-id="cafd4-130">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) ou [group](../resources/group.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="cafd4-130">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="cafd4-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="cafd4-131">Response</span></span>
<span data-ttu-id="cafd4-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cafd4-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cafd4-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cafd4-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="cafd4-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cafd4-135">Request</span></span>
<span data-ttu-id="cafd4-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cafd4-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "add_group_member"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}
```
<span data-ttu-id="cafd4-137">No corpo da solicitação, fornecer uma representação JSON do `id` do objeto [directoryObject](../resources/directoryobject.md), [usuário](../resources/user.md)ou [grupo](../resources/group.md) que você deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="cafd4-137">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), or [group](../resources/group.md) object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="cafd4-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="cafd4-138">Response</span></span>
<span data-ttu-id="cafd4-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cafd4-139">The following is an example of the response.</span></span>
><span data-ttu-id="cafd4-140">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cafd4-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cafd4-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cafd4-141">All the properties will be returned from an actual call.</span></span>
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
