---
title: Atribuir um gerente
description: Use essa API para atribuir um gerente ao usuário.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 770fad522e505abbd9f689540e6a28e875ba063d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912068"
---
# <a name="assign-a-manager"></a><span data-ttu-id="fdf66-103">Atribuir um gerente</span><span class="sxs-lookup"><span data-stu-id="fdf66-103">Assign a manager</span></span>

> <span data-ttu-id="fdf66-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fdf66-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fdf66-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fdf66-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fdf66-106">Use essa API para atribuir um gerente ao usuário.</span><span class="sxs-lookup"><span data-stu-id="fdf66-106">Use this API to assign a user's manager.</span></span>
> <span data-ttu-id="fdf66-107">Observação: não é possível atribuir subordinados diretamente; em vez disso, use essa API.</span><span class="sxs-lookup"><span data-stu-id="fdf66-107">Note: You cannot assign direct reports - instead use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="fdf66-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="fdf66-108">Permissions</span></span>
<span data-ttu-id="fdf66-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdf66-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdf66-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fdf66-111">Permission type</span></span>      | <span data-ttu-id="fdf66-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fdf66-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fdf66-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fdf66-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fdf66-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fdf66-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fdf66-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fdf66-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fdf66-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdf66-116">Not supported.</span></span>    |
|<span data-ttu-id="fdf66-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fdf66-117">Application</span></span> | <span data-ttu-id="fdf66-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdf66-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fdf66-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fdf66-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="fdf66-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fdf66-120">Request headers</span></span>
| <span data-ttu-id="fdf66-121">Nome</span><span class="sxs-lookup"><span data-stu-id="fdf66-121">Name</span></span>       | <span data-ttu-id="fdf66-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="fdf66-122">Type</span></span> | <span data-ttu-id="fdf66-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdf66-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fdf66-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="fdf66-124">Authorization</span></span>  | <span data-ttu-id="fdf66-125">string</span><span class="sxs-lookup"><span data-stu-id="fdf66-125">string</span></span>  | <span data-ttu-id="fdf66-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fdf66-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fdf66-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fdf66-128">Request body</span></span>
<span data-ttu-id="fdf66-129">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md) ou [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="fdf66-129">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="fdf66-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdf66-130">Response</span></span>

<span data-ttu-id="fdf66-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fdf66-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdf66-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fdf66-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fdf66-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fdf66-134">Request</span></span>
<span data-ttu-id="fdf66-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fdf66-135">Here is an example of the request.</span></span>
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
<span data-ttu-id="fdf66-136">No corpo da solicitação, forneça uma representação JSON de um objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="fdf66-136">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="fdf66-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdf66-137">Response</span></span>
<span data-ttu-id="fdf66-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fdf66-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
