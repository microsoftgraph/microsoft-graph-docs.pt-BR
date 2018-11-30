---
title: Excluir o aplicativo da equipe
description: Desinstala um aplicativo da equipe do especificado.
ms.openlocfilehash: e126dca3812e6b6323820eaf1d230243aebc93e8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039568"
---
# <a name="delete-app-from-team"></a><span data-ttu-id="f8f8d-103">Excluir o aplicativo da equipe</span><span class="sxs-lookup"><span data-stu-id="f8f8d-103">Delete app from team</span></span>

> <span data-ttu-id="f8f8d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f8f8d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8f8d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f8f8d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f8f8d-106">Desinstala um [aplicativo](../resources/teamsappinstallation.md) da [equipe](../resources/team.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="f8f8d-106">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f8f8d-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="f8f8d-107">Permissions</span></span>
<span data-ttu-id="f8f8d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8f8d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8f8d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8f8d-110">Permission type</span></span>      | <span data-ttu-id="f8f8d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f8f8d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8f8d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8f8d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f8f8d-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8f8d-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f8f8d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8f8d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8f8d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8f8d-115">Not supported.</span></span>    |
|<span data-ttu-id="f8f8d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8f8d-116">Application</span></span> | <span data-ttu-id="f8f8d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8f8d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8f8d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8f8d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f8f8d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8f8d-119">Request headers</span></span>
| <span data-ttu-id="f8f8d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f8f8d-120">Header</span></span>       | <span data-ttu-id="f8f8d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f8f8d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f8f8d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8f8d-122">Authorization</span></span>  | <span data-ttu-id="f8f8d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8f8d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f8f8d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8f8d-125">Request body</span></span>
<span data-ttu-id="f8f8d-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f8f8d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8f8d-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8f8d-127">Response</span></span>

<span data-ttu-id="f8f8d-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8f8d-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8f8d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f8f8d-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f8f8d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8f8d-131">Request</span></span>
<span data-ttu-id="f8f8d-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8f8d-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/installedApps/{id}
```
#### <a name="response"></a><span data-ttu-id="f8f8d-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8f8d-133">Response</span></span>
<span data-ttu-id="f8f8d-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f8f8d-134">The following is an example of the response.</span></span> <span data-ttu-id="f8f8d-135">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="f8f8d-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f8f8d-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f8f8d-136">All of the properties will be returned from an actual call.</span></span>
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
