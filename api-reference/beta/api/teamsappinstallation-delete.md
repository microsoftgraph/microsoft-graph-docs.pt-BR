---
title: Excluir o aplicativo da equipe
description: Desinstala um aplicativo da equipe do especificado.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: b0d1c7d8344218d6eba4165e94b09158d60846ec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852490"
---
# <a name="delete-app-from-team"></a><span data-ttu-id="f5f9a-103">Excluir o aplicativo da equipe</span><span class="sxs-lookup"><span data-stu-id="f5f9a-103">Delete app from team</span></span>

> <span data-ttu-id="f5f9a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f5f9a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5f9a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f5f9a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f5f9a-106">Desinstala um [aplicativo](../resources/teamsappinstallation.md) da [equipe](../resources/team.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="f5f9a-106">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f5f9a-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="f5f9a-107">Permissions</span></span>
<span data-ttu-id="f5f9a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5f9a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5f9a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5f9a-110">Permission type</span></span>      | <span data-ttu-id="f5f9a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f5f9a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5f9a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5f9a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f5f9a-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5f9a-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f5f9a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5f9a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5f9a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5f9a-115">Not supported.</span></span>    |
|<span data-ttu-id="f5f9a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5f9a-116">Application</span></span> | <span data-ttu-id="f5f9a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5f9a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5f9a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5f9a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f5f9a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5f9a-119">Request headers</span></span>
| <span data-ttu-id="f5f9a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f5f9a-120">Header</span></span>       | <span data-ttu-id="f5f9a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f5f9a-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f5f9a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5f9a-122">Authorization</span></span>  | <span data-ttu-id="f5f9a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5f9a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f5f9a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5f9a-125">Request body</span></span>
<span data-ttu-id="f5f9a-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f5f9a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5f9a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5f9a-127">Response</span></span>

<span data-ttu-id="f5f9a-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5f9a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5f9a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5f9a-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f5f9a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5f9a-131">Request</span></span>
<span data-ttu-id="f5f9a-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5f9a-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/installedApps/{id}
```
#### <a name="response"></a><span data-ttu-id="f5f9a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5f9a-133">Response</span></span>
<span data-ttu-id="f5f9a-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f5f9a-134">The following is an example of the response.</span></span> <span data-ttu-id="f5f9a-135">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="f5f9a-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f5f9a-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5f9a-136">All of the properties will be returned from an actual call.</span></span>
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
