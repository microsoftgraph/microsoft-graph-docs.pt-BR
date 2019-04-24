---
title: Adicionar membro
description: Use esta API para adicionar um membro a um grupo do Office 365, a um grupo de segurança ou a um grupo de segurança habilitado para email através da propriedade de navegação **owners**.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: ac21262858137074ed92978f0ab6530052fcc2de
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32502153"
---
# <a name="add-member"></a><span data-ttu-id="d8336-103">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="d8336-103">Add member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8336-104">Use esta API para adicionar um membro a um grupo do Office 365, a um grupo de segurança ou a um grupo de segurança habilitado para email através da propriedade de navegação **owners**.</span><span class="sxs-lookup"><span data-stu-id="d8336-104">Use this API to add a member to an Office 365 Group, a security group, or a mail-enabled security group through the **members** navigation property.</span></span>

<span data-ttu-id="d8336-105">É possível adicionar usuários ou outros grupos.</span><span class="sxs-lookup"><span data-stu-id="d8336-105">You can add users or other groups.</span></span> <span data-ttu-id="d8336-106">Importante: só é possível adicionar usuários a grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="d8336-106">Important: You can add only users to Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8336-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d8336-107">Permissions</span></span>
<span data-ttu-id="d8336-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8336-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8336-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8336-110">Permission type</span></span>      | <span data-ttu-id="d8336-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d8336-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8336-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8336-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d8336-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d8336-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d8336-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8336-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8336-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8336-115">Not supported.</span></span>    |
|<span data-ttu-id="d8336-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8336-116">Application</span></span> | <span data-ttu-id="d8336-117">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8336-117">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8336-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8336-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="d8336-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8336-119">Request headers</span></span>
| <span data-ttu-id="d8336-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d8336-120">Name</span></span>       | <span data-ttu-id="d8336-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8336-121">Type</span></span> | <span data-ttu-id="d8336-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8336-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d8336-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8336-123">Authorization</span></span>  | <span data-ttu-id="d8336-124">string</span><span class="sxs-lookup"><span data-stu-id="d8336-124">string</span></span>  | <span data-ttu-id="d8336-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8336-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8336-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8336-127">Request body</span></span>
<span data-ttu-id="d8336-128">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) ou [group](../resources/group.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="d8336-128">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="d8336-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8336-129">Response</span></span>
<span data-ttu-id="d8336-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8336-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8336-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8336-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d8336-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8336-133">Request</span></span>
<span data-ttu-id="d8336-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8336-134">The following is an example of the request.</span></span>
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
<span data-ttu-id="d8336-135">No corpo da solicitação, forneça uma representação JSON `id` do objeto [directoryobject](../resources/directoryobject.md), [User](../resources/user.md)ou [Group](../resources/group.md) que você deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="d8336-135">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), or [group](../resources/group.md) object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="d8336-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8336-136">Response</span></span>
<span data-ttu-id="d8336-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d8336-137">The following is an example of the response.</span></span>
><span data-ttu-id="d8336-138">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d8336-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d8336-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d8336-139">All the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/group-post-members.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
