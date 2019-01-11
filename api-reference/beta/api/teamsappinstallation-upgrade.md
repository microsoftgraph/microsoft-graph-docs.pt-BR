---
title: Um aplicativo em uma equipe de atualização
description: Atualiza uma instalação de aplicativo em uma equipe
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 194763ea8464dd0651c3af1cef73e479b403d083
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831371"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="806ee-103">Um aplicativo em uma equipe de atualização</span><span class="sxs-lookup"><span data-stu-id="806ee-103">Upgrade an app in a team</span></span>

> <span data-ttu-id="806ee-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="806ee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="806ee-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="806ee-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="806ee-106">Atualiza uma [instalação de aplicativo](../resources/teamsappinstallation.md) em uma [equipe](../resources/team.md) para a versão mais recente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="806ee-106">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="806ee-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="806ee-107">Permissions</span></span>

<span data-ttu-id="806ee-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="806ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="806ee-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="806ee-110">Permission type</span></span>      | <span data-ttu-id="806ee-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="806ee-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="806ee-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="806ee-112">Delegated (work or school account)</span></span> | <span data-ttu-id="806ee-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="806ee-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="806ee-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="806ee-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="806ee-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="806ee-115">Not supported.</span></span>    |
|<span data-ttu-id="806ee-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="806ee-116">Application</span></span> | <span data-ttu-id="806ee-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="806ee-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="806ee-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="806ee-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="806ee-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="806ee-119">Request headers</span></span>
| <span data-ttu-id="806ee-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="806ee-120">Header</span></span>       | <span data-ttu-id="806ee-121">Valor</span><span class="sxs-lookup"><span data-stu-id="806ee-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="806ee-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="806ee-122">Authorization</span></span>  | <span data-ttu-id="806ee-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="806ee-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="806ee-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="806ee-125">Request body</span></span>
<span data-ttu-id="806ee-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="806ee-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="806ee-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="806ee-127">Response</span></span>

<span data-ttu-id="806ee-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="806ee-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="806ee-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="806ee-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="806ee-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="806ee-131">Request</span></span>
<span data-ttu-id="806ee-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="806ee-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
#### <a name="response"></a><span data-ttu-id="806ee-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="806ee-133">Response</span></span>
<span data-ttu-id="806ee-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="806ee-134">The following is an example of the response.</span></span> 

><span data-ttu-id="806ee-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="806ee-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 204 No Content
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
