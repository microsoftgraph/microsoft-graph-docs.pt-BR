---
title: Obter guia
description: 'Recupere as propriedades e os relacionamentos da guia especificada. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c8c860caa538699635a5b5d92595664b700124cd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544595"
---
# <a name="get-tab"></a><span data-ttu-id="ce21f-103">Obter guia</span><span class="sxs-lookup"><span data-stu-id="ce21f-103">Get tab</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce21f-104">Recupere as propriedades e os relacionamentos da [guia](../resources/teamstab.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="ce21f-104">Retrieve the properties and relationships of the specified [tab](../resources/teamstab.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="ce21f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ce21f-105">Permissions</span></span>
<span data-ttu-id="ce21f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce21f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce21f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce21f-108">Permission type</span></span>      | <span data-ttu-id="ce21f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ce21f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce21f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce21f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ce21f-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce21f-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ce21f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce21f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce21f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce21f-113">Not supported.</span></span>    |
|<span data-ttu-id="ce21f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce21f-114">Application</span></span> | <span data-ttu-id="ce21f-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce21f-115">Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="ce21f-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="ce21f-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="ce21f-117">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="ce21f-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="ce21f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce21f-118">HTTP request</span></span>
```http
GET /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ce21f-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ce21f-119">Optional query parameters</span></span>

<span data-ttu-id="ce21f-120">Este método dá suporte ao $select e $expand [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ce21f-120">This method supports the $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ce21f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce21f-121">Request headers</span></span>
| <span data-ttu-id="ce21f-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ce21f-122">Header</span></span>       | <span data-ttu-id="ce21f-123">Valor</span><span class="sxs-lookup"><span data-stu-id="ce21f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ce21f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce21f-124">Authorization</span></span>  | <span data-ttu-id="ce21f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce21f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ce21f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce21f-127">Request body</span></span>
<span data-ttu-id="ce21f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ce21f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce21f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce21f-129">Response</span></span>

<span data-ttu-id="ce21f-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Tab](../resources/teamstab.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce21f-130">If successful, this method returns a `200 OK` response code and a [tab](../resources/teamstab.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ce21f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ce21f-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ce21f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce21f-132">Request</span></span>
<span data-ttu-id="ce21f-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce21f-133">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}?$expand=teamsApp
```
#### <a name="response"></a><span data-ttu-id="ce21f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce21f-134">Response</span></span>
<span data-ttu-id="ce21f-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ce21f-135">The following is an example of the response.</span></span> 

><span data-ttu-id="ce21f-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ce21f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/teamstab-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
