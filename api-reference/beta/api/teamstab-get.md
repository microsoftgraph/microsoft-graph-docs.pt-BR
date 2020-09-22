---
title: Obter guia
description: 'Recupere as propriedades e os relacionamentos da guia especificada. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: dc8370a7df8663293d2d2562a4dfd45928b8bed9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47999039"
---
# <a name="get-tab"></a><span data-ttu-id="aa584-103">Obter guia</span><span class="sxs-lookup"><span data-stu-id="aa584-103">Get tab</span></span>

<span data-ttu-id="aa584-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa584-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa584-105">Recupere as propriedades e os relacionamentos da [guia](../resources/teamstab.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="aa584-105">Retrieve the properties and relationships of the specified [tab](../resources/teamstab.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="aa584-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="aa584-106">Permissions</span></span>
<span data-ttu-id="aa584-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa584-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa584-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aa584-109">Permission type</span></span>      | <span data-ttu-id="aa584-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aa584-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa584-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aa584-111">Delegated (work or school account)</span></span> | <span data-ttu-id="aa584-112">TeamsTab. Read. All, TeamsTab. ReadWrite. All, Group. Read. All, Group. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="aa584-112">TeamsTab.Read.All, TeamsTab.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="aa584-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aa584-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa584-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa584-114">Not supported.</span></span>    |
|<span data-ttu-id="aa584-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aa584-115">Application</span></span> | <span data-ttu-id="aa584-116">TeamsTab. Read. Group *, TeamsTab. Edit. Group*, TeamsTab. Read. All, TeamsTab. ReadWrite. All, Group. Read. All, Group. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="aa584-116">TeamsTab.Read.Group *, TeamsTab.Edit.Group*, TeamsTab.Read.All, TeamsTab.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
> <span data-ttu-id="aa584-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="aa584-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="aa584-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="aa584-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="aa584-119">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="aa584-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="aa584-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa584-120">HTTP request</span></span>
```http
GET /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aa584-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="aa584-121">Optional query parameters</span></span>

<span data-ttu-id="aa584-122">Este método dá suporte ao $select e $expand [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="aa584-122">This method supports the $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aa584-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa584-123">Request headers</span></span>
| <span data-ttu-id="aa584-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aa584-124">Header</span></span>       | <span data-ttu-id="aa584-125">Valor</span><span class="sxs-lookup"><span data-stu-id="aa584-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="aa584-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="aa584-126">Authorization</span></span>  | <span data-ttu-id="aa584-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa584-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aa584-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa584-129">Request body</span></span>
<span data-ttu-id="aa584-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aa584-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa584-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa584-131">Response</span></span>

<span data-ttu-id="aa584-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [Tab](../resources/teamstab.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa584-132">If successful, this method returns a `200 OK` response code and a [tab](../resources/teamstab.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aa584-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aa584-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="aa584-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa584-134">Request</span></span>
<span data-ttu-id="aa584-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa584-135">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}?$expand=teamsApp
```
#### <a name="response"></a><span data-ttu-id="aa584-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa584-136">Response</span></span>
<span data-ttu-id="aa584-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="aa584-137">The following is an example of the response.</span></span> 

><span data-ttu-id="aa584-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aa584-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "tabId",
  "displayName": "My Contoso Tab - updated",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "teamsApp": {
      "id": "0d820ecd-def2-4297-adad-78056cde7c78",
      "externalId": null,
      "displayName": "Contoso",
      "distributionMethod": "store"
  },
  "sortOrderIndex": "20",
  "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a channel tab",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


