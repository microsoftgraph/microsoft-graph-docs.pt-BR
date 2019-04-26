---
title: Adicionar aplicativo à equipe
description: Instala um aplicativo para a equipe especificada.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 837528e20da88496ab4d9b1133e461cbc462df37
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330051"
---
# <a name="add-app-to-team"></a><span data-ttu-id="378f3-103">Adicionar aplicativo à equipe</span><span class="sxs-lookup"><span data-stu-id="378f3-103">Add app to team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="378f3-104">Instala um [aplicativo](../resources/teamsapp.md) para a [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="378f3-104">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="378f3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="378f3-105">Permissions</span></span>
<span data-ttu-id="378f3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="378f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="378f3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="378f3-108">Permission type</span></span>      | <span data-ttu-id="378f3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="378f3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="378f3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="378f3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="378f3-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="378f3-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="378f3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="378f3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="378f3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="378f3-113">Not supported.</span></span>    |
|<span data-ttu-id="378f3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="378f3-114">Application</span></span> | <span data-ttu-id="378f3-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="378f3-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="378f3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="378f3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="378f3-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="378f3-117">Request headers</span></span>
| <span data-ttu-id="378f3-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="378f3-118">Header</span></span>       | <span data-ttu-id="378f3-119">Valor</span><span class="sxs-lookup"><span data-stu-id="378f3-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="378f3-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="378f3-120">Authorization</span></span>  | <span data-ttu-id="378f3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="378f3-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="378f3-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="378f3-123">Request body</span></span>

| <span data-ttu-id="378f3-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="378f3-124">Property</span></span>     | <span data-ttu-id="378f3-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="378f3-125">Type</span></span>   |<span data-ttu-id="378f3-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="378f3-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="378f3-127">teamsApp</span><span class="sxs-lookup"><span data-stu-id="378f3-127">teamsApp</span></span>|<span data-ttu-id="378f3-128">String</span><span class="sxs-lookup"><span data-stu-id="378f3-128">String</span></span>|<span data-ttu-id="378f3-129">A ID do aplicativo a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="378f3-129">The id of the app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="378f3-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="378f3-130">Response</span></span>

<span data-ttu-id="378f3-131">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="378f3-131">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="378f3-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="378f3-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="378f3-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="378f3-133">Request</span></span>
<span data-ttu-id="378f3-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="378f3-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/installedApps
{
   "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
#### <a name="response"></a><span data-ttu-id="378f3-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="378f3-135">Response</span></span>
<span data-ttu-id="378f3-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="378f3-136">The following is an example of the response.</span></span> <span data-ttu-id="378f3-137">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="378f3-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="378f3-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="378f3-138">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

## <a name="see-also"></a><span data-ttu-id="378f3-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="378f3-139">See also</span></span>

