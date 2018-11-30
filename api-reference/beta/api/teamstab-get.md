---
title: Obtenha o guia
description: 'Recupere as propriedades e relacionamentos da guia especificado. '
ms.openlocfilehash: 57bd7d8b11b0bf20d54bf8da16cdd41220320fcd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033415"
---
# <a name="get-tab"></a><span data-ttu-id="16df0-103">Obtenha o guia</span><span class="sxs-lookup"><span data-stu-id="16df0-103">Get tab</span></span>

> <span data-ttu-id="16df0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="16df0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16df0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="16df0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="16df0-106">Recupere as propriedades e relacionamentos da [guia](../resources/teamstab.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="16df0-106">Retrieve the properties and relationships of the specified [tab](../resources/teamstab.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="16df0-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="16df0-107">Permissions</span></span>
<span data-ttu-id="16df0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16df0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16df0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16df0-110">Permission type</span></span>      | <span data-ttu-id="16df0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="16df0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16df0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16df0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="16df0-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16df0-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="16df0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16df0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16df0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16df0-115">Not supported.</span></span>    |
|<span data-ttu-id="16df0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16df0-116">Application</span></span> | <span data-ttu-id="16df0-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16df0-117">Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="16df0-118">Atualmente, somente [permissões delegadas](/graph/permissions-reference) têm suporte para esta operação.</span><span class="sxs-lookup"><span data-stu-id="16df0-118">Currently, only [delegated permissions](/graph/permissions-reference) are supported for this operation.</span></span>

## <a name="http-request"></a><span data-ttu-id="16df0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16df0-119">HTTP request</span></span>
```http
GET /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="16df0-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="16df0-120">Optional query parameters</span></span>

<span data-ttu-id="16df0-121">Este método oferece suporte a $select e $expand [OData parâmetros de consulta](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="16df0-121">This method supports the $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="16df0-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16df0-122">Request headers</span></span>
| <span data-ttu-id="16df0-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="16df0-123">Header</span></span>       | <span data-ttu-id="16df0-124">Valor</span><span class="sxs-lookup"><span data-stu-id="16df0-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="16df0-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="16df0-125">Authorization</span></span>  | <span data-ttu-id="16df0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16df0-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="16df0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16df0-128">Request body</span></span>
<span data-ttu-id="16df0-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="16df0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16df0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="16df0-130">Response</span></span>

<span data-ttu-id="16df0-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [tab](../resources/teamstab.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16df0-131">If successful, this method returns a `200 OK` response code and a [tab](../resources/teamstab.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="16df0-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="16df0-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="16df0-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16df0-133">Request</span></span>
<span data-ttu-id="16df0-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="16df0-134">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="16df0-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="16df0-135">Response</span></span>
<span data-ttu-id="16df0-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="16df0-136">The following is an example of the response.</span></span> 

><span data-ttu-id="16df0-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="16df0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "tabId",
  "name": "My Contoso Tab - updated",
  "teamsAppId": "06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "sortOrderIndex": 20,
  "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get a channel tab",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
