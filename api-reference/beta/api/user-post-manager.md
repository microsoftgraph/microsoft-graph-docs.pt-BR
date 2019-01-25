---
title: Atribuir um gerente
description: Use essa API para atribuir um gerente ao usuário.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4148eb1748680458500dc5a625e6b297e0ca5099
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514548"
---
# <a name="assign-a-manager"></a><span data-ttu-id="26337-103">Atribuir um gerente</span><span class="sxs-lookup"><span data-stu-id="26337-103">Assign a manager</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26337-104">Use essa API para atribuir um gerente ao usuário.</span><span class="sxs-lookup"><span data-stu-id="26337-104">Use this API to assign a user's manager.</span></span>
> <span data-ttu-id="26337-105">Observação: não é possível atribuir subordinados diretamente; em vez disso, use essa API.</span><span class="sxs-lookup"><span data-stu-id="26337-105">Note: You cannot assign direct reports - instead use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="26337-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="26337-106">Permissions</span></span>
<span data-ttu-id="26337-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26337-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26337-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26337-109">Permission type</span></span>      | <span data-ttu-id="26337-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="26337-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26337-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26337-111">Delegated (work or school account)</span></span> | <span data-ttu-id="26337-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="26337-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="26337-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26337-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26337-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26337-114">Not supported.</span></span>    |
|<span data-ttu-id="26337-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26337-115">Application</span></span> | <span data-ttu-id="26337-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26337-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="26337-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26337-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="26337-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26337-118">Request headers</span></span>
| <span data-ttu-id="26337-119">Nome</span><span class="sxs-lookup"><span data-stu-id="26337-119">Name</span></span>       | <span data-ttu-id="26337-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="26337-120">Type</span></span> | <span data-ttu-id="26337-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="26337-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="26337-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="26337-122">Authorization</span></span>  | <span data-ttu-id="26337-123">string</span><span class="sxs-lookup"><span data-stu-id="26337-123">string</span></span>  | <span data-ttu-id="26337-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26337-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26337-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26337-126">Request body</span></span>
<span data-ttu-id="26337-127">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md) ou [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="26337-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="26337-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="26337-128">Response</span></span>

<span data-ttu-id="26337-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26337-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26337-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26337-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="26337-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26337-132">Request</span></span>
<span data-ttu-id="26337-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26337-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
PUT https://graph.microsoft.com/v1.0/users/{id}/manager/$ref
Content-type: application/json
Content-length: xxx

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
<span data-ttu-id="26337-134">No corpo da solicitação, forneça uma representação JSON de um objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="26337-134">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="26337-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="26337-135">Response</span></span>
<span data-ttu-id="26337-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="26337-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/user-post-manager.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
