---
title: Adicionar o aplicativo à equipe
description: Instala um aplicativo para a equipe especificada.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: d3f67b8ea49f9940b60bcf0aec7eea15a59388b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855857"
---
# <a name="add-app-to-team"></a><span data-ttu-id="d1e99-103">Adicionar o aplicativo à equipe</span><span class="sxs-lookup"><span data-stu-id="d1e99-103">Add app to team</span></span>

> <span data-ttu-id="d1e99-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d1e99-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1e99-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d1e99-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d1e99-106">Instala um [aplicativo](../resources/teamsapp.md) para a [equipe](../resources/team.md)de especificado.</span><span class="sxs-lookup"><span data-stu-id="d1e99-106">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d1e99-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="d1e99-107">Permissions</span></span>
<span data-ttu-id="d1e99-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1e99-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1e99-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1e99-110">Permission type</span></span>      | <span data-ttu-id="d1e99-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d1e99-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1e99-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1e99-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d1e99-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1e99-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d1e99-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1e99-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1e99-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1e99-115">Not supported.</span></span>    |
|<span data-ttu-id="d1e99-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1e99-116">Application</span></span> | <span data-ttu-id="d1e99-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1e99-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1e99-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1e99-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="d1e99-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1e99-119">Request headers</span></span>
| <span data-ttu-id="d1e99-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d1e99-120">Header</span></span>       | <span data-ttu-id="d1e99-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d1e99-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d1e99-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1e99-122">Authorization</span></span>  | <span data-ttu-id="d1e99-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1e99-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d1e99-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1e99-125">Request body</span></span>

| <span data-ttu-id="d1e99-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d1e99-126">Property</span></span>     | <span data-ttu-id="d1e99-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1e99-127">Type</span></span>   |<span data-ttu-id="d1e99-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1e99-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1e99-129">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d1e99-129">teamsApp</span></span>|<span data-ttu-id="d1e99-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d1e99-130">String</span></span>|<span data-ttu-id="d1e99-131">A id do aplicativo para adicionar.</span><span class="sxs-lookup"><span data-stu-id="d1e99-131">The id of the app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="d1e99-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1e99-132">Response</span></span>

<span data-ttu-id="d1e99-133">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="d1e99-133">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="d1e99-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1e99-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d1e99-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1e99-135">Request</span></span>
<span data-ttu-id="d1e99-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1e99-136">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="d1e99-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1e99-137">Response</span></span>
<span data-ttu-id="d1e99-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d1e99-138">The following is an example of the response.</span></span> <span data-ttu-id="d1e99-139">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="d1e99-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d1e99-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d1e99-140">All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="d1e99-141">Veja também</span><span class="sxs-lookup"><span data-stu-id="d1e99-141">See also</span></span>

