---
title: Adicionar o aplicativo à equipe
description: Instala um aplicativo para a equipe especificada.
author: nkramer
ms.openlocfilehash: ed38f809c784c4178f7be2b028dc4c71a6206b1b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349165"
---
# <a name="add-app-to-team"></a><span data-ttu-id="18fa0-103">Adicionar o aplicativo à equipe</span><span class="sxs-lookup"><span data-stu-id="18fa0-103">Add app to team</span></span>

> <span data-ttu-id="18fa0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="18fa0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18fa0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="18fa0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="18fa0-106">Instala um [aplicativo](../resources/teamsapp.md) para a [equipe](../resources/team.md)de especificado.</span><span class="sxs-lookup"><span data-stu-id="18fa0-106">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="18fa0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="18fa0-107">Permissions</span></span>
<span data-ttu-id="18fa0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18fa0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18fa0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18fa0-110">Permission type</span></span>      | <span data-ttu-id="18fa0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="18fa0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18fa0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18fa0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="18fa0-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18fa0-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="18fa0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18fa0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18fa0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18fa0-115">Not supported.</span></span>    |
|<span data-ttu-id="18fa0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18fa0-116">Application</span></span> | <span data-ttu-id="18fa0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18fa0-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="18fa0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18fa0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="18fa0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18fa0-119">Request headers</span></span>
| <span data-ttu-id="18fa0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="18fa0-120">Header</span></span>       | <span data-ttu-id="18fa0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="18fa0-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="18fa0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="18fa0-122">Authorization</span></span>  | <span data-ttu-id="18fa0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18fa0-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="18fa0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18fa0-125">Request body</span></span>

| <span data-ttu-id="18fa0-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18fa0-126">Property</span></span>     | <span data-ttu-id="18fa0-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="18fa0-127">Type</span></span>   |<span data-ttu-id="18fa0-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="18fa0-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18fa0-129">teamsApp</span><span class="sxs-lookup"><span data-stu-id="18fa0-129">teamsApp</span></span>|<span data-ttu-id="18fa0-130">String</span><span class="sxs-lookup"><span data-stu-id="18fa0-130">String</span></span>|<span data-ttu-id="18fa0-131">A id do aplicativo para adicionar.</span><span class="sxs-lookup"><span data-stu-id="18fa0-131">The id of the app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="18fa0-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="18fa0-132">Response</span></span>

<span data-ttu-id="18fa0-133">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="18fa0-133">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="18fa0-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="18fa0-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="18fa0-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18fa0-135">Request</span></span>
<span data-ttu-id="18fa0-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="18fa0-136">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="18fa0-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="18fa0-137">Response</span></span>
<span data-ttu-id="18fa0-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="18fa0-138">The following is an example of the response.</span></span> <span data-ttu-id="18fa0-139">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="18fa0-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="18fa0-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="18fa0-140">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="18fa0-141">Veja também</span><span class="sxs-lookup"><span data-stu-id="18fa0-141">See also</span></span>

