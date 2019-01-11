---
title: Atribuir um gerente
description: Use essa API para atribuir um gerente ao usuário.
localization_priority: Normal
ms.openlocfilehash: 7391cef6b632df00a65f683855a5d088f69a43bb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811953"
---
# <a name="assign-a-manager"></a><span data-ttu-id="dbefb-103">Atribuir um gerente</span><span class="sxs-lookup"><span data-stu-id="dbefb-103">Assign a manager</span></span>

> <span data-ttu-id="dbefb-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="dbefb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dbefb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dbefb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dbefb-106">Use essa API para atribuir um gerente ao usuário.</span><span class="sxs-lookup"><span data-stu-id="dbefb-106">Use this API to assign a user's manager.</span></span>
> <span data-ttu-id="dbefb-107">Observação: não é possível atribuir subordinados diretamente; em vez disso, use essa API.</span><span class="sxs-lookup"><span data-stu-id="dbefb-107">Note: You cannot assign direct reports - instead use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="dbefb-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="dbefb-108">Permissions</span></span>
<span data-ttu-id="dbefb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbefb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbefb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dbefb-111">Permission type</span></span>      | <span data-ttu-id="dbefb-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dbefb-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dbefb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dbefb-113">Delegated (work or school account)</span></span> | <span data-ttu-id="dbefb-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dbefb-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dbefb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dbefb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbefb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbefb-116">Not supported.</span></span>    |
|<span data-ttu-id="dbefb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dbefb-117">Application</span></span> | <span data-ttu-id="dbefb-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbefb-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dbefb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dbefb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="dbefb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dbefb-120">Request headers</span></span>
| <span data-ttu-id="dbefb-121">Nome</span><span class="sxs-lookup"><span data-stu-id="dbefb-121">Name</span></span>       | <span data-ttu-id="dbefb-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbefb-122">Type</span></span> | <span data-ttu-id="dbefb-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbefb-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dbefb-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="dbefb-124">Authorization</span></span>  | <span data-ttu-id="dbefb-125">string</span><span class="sxs-lookup"><span data-stu-id="dbefb-125">string</span></span>  | <span data-ttu-id="dbefb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dbefb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dbefb-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dbefb-128">Request body</span></span>
<span data-ttu-id="dbefb-129">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md) ou [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="dbefb-129">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="dbefb-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbefb-130">Response</span></span>

<span data-ttu-id="dbefb-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dbefb-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbefb-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dbefb-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dbefb-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dbefb-134">Request</span></span>
<span data-ttu-id="dbefb-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dbefb-135">Here is an example of the request.</span></span>
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
<span data-ttu-id="dbefb-136">No corpo da solicitação, forneça uma representação JSON de um objeto [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="dbefb-136">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="dbefb-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbefb-137">Response</span></span>
<span data-ttu-id="dbefb-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dbefb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
