---
title: Excluir o aplicativo da equipe
description: Desinstala um aplicativo da equipe do especificado.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 2545ae8c0c6d0485fe4ed57f94137936fda538d6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821165"
---
# <a name="delete-app-from-team"></a><span data-ttu-id="2e56e-103">Excluir o aplicativo da equipe</span><span class="sxs-lookup"><span data-stu-id="2e56e-103">Delete app from team</span></span>



<span data-ttu-id="2e56e-104">Desinstala um [aplicativo](../resources/teamsappinstallation.md) da [equipe](../resources/team.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="2e56e-104">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2e56e-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="2e56e-105">Permissions</span></span>
<span data-ttu-id="2e56e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e56e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e56e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e56e-108">Permission type</span></span>      | <span data-ttu-id="2e56e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2e56e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e56e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e56e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2e56e-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e56e-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2e56e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e56e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e56e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e56e-113">Not supported.</span></span>    |
|<span data-ttu-id="2e56e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e56e-114">Application</span></span> | <span data-ttu-id="2e56e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e56e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e56e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e56e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2e56e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2e56e-117">Request headers</span></span>
| <span data-ttu-id="2e56e-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2e56e-118">Header</span></span>       | <span data-ttu-id="2e56e-119">Valor</span><span class="sxs-lookup"><span data-stu-id="2e56e-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2e56e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="2e56e-120">Authorization</span></span>  | <span data-ttu-id="2e56e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e56e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2e56e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2e56e-123">Request body</span></span>
<span data-ttu-id="2e56e-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2e56e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e56e-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e56e-125">Response</span></span>

<span data-ttu-id="2e56e-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e56e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e56e-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2e56e-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2e56e-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e56e-129">Request</span></span>
<span data-ttu-id="2e56e-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e56e-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE /teams/{id}/installedApps/{id}
```
#### <a name="response"></a><span data-ttu-id="2e56e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e56e-131">Response</span></span>
<span data-ttu-id="2e56e-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2e56e-132">The following is an example of the response.</span></span> <span data-ttu-id="2e56e-133">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="2e56e-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2e56e-134">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2e56e-134">All of the properties will be returned from an actual call.</span></span>
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
