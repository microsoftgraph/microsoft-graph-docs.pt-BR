---
title: Obtenha o guia
description: 'Recupere as propriedades e relacionamentos da guia especificado. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9bf9a41154b57a5f76f3cce3c8754e27e34c0837
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571181"
---
# <a name="get-tab"></a><span data-ttu-id="55f1c-103">Obtenha o guia</span><span class="sxs-lookup"><span data-stu-id="55f1c-103">Get tab</span></span>



<span data-ttu-id="55f1c-104">Recupere as propriedades e relacionamentos da [guia](../resources/teamstab.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="55f1c-104">Retrieve the properties and relationships of the specified [tab](../resources/teamstab.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="55f1c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="55f1c-105">Permissions</span></span>
<span data-ttu-id="55f1c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55f1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55f1c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55f1c-108">Permission type</span></span>      | <span data-ttu-id="55f1c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="55f1c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55f1c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55f1c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="55f1c-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55f1c-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="55f1c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55f1c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55f1c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55f1c-113">Not supported.</span></span>    |
|<span data-ttu-id="55f1c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55f1c-114">Application</span></span> | <span data-ttu-id="55f1c-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55f1c-115">Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="55f1c-116">**Observação**: Esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="55f1c-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="55f1c-117">Administradores globais e administradores de serviço de Teams da Microsoft podem acessar as equipes que eles não serão um membro do.</span><span class="sxs-lookup"><span data-stu-id="55f1c-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="55f1c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55f1c-118">HTTP request</span></span>
```http
GET /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="55f1c-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="55f1c-119">Optional query parameters</span></span>

<span data-ttu-id="55f1c-120">Este método oferece suporte a $select e $expand [OData parâmetros de consulta](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="55f1c-120">This method supports the $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="55f1c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55f1c-121">Request headers</span></span>
| <span data-ttu-id="55f1c-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="55f1c-122">Header</span></span>       | <span data-ttu-id="55f1c-123">Valor</span><span class="sxs-lookup"><span data-stu-id="55f1c-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="55f1c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="55f1c-124">Authorization</span></span>  | <span data-ttu-id="55f1c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55f1c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="55f1c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55f1c-127">Request body</span></span>
<span data-ttu-id="55f1c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="55f1c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55f1c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="55f1c-129">Response</span></span>

<span data-ttu-id="55f1c-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [tab](../resources/teamstab.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55f1c-130">If successful, this method returns a `200 OK` response code and a [tab](../resources/teamstab.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="55f1c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55f1c-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="55f1c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55f1c-132">Request</span></span>
<span data-ttu-id="55f1c-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="55f1c-133">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="55f1c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="55f1c-134">Response</span></span>
<span data-ttu-id="55f1c-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="55f1c-135">The following is an example of the response.</span></span> 

><span data-ttu-id="55f1c-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="55f1c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
