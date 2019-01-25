---
title: Obtenha o guia
description: 'Recupere as propriedades e relacionamentos da guia especificado. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 613989f2c8bd2754e6c311948342facff99be9f0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517607"
---
# <a name="get-tab"></a><span data-ttu-id="2602a-103">Obtenha o guia</span><span class="sxs-lookup"><span data-stu-id="2602a-103">Get tab</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2602a-104">Recupere as propriedades e relacionamentos da [guia](../resources/teamstab.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="2602a-104">Retrieve the properties and relationships of the specified [tab](../resources/teamstab.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="2602a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2602a-105">Permissions</span></span>
<span data-ttu-id="2602a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2602a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2602a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2602a-108">Permission type</span></span>      | <span data-ttu-id="2602a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2602a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2602a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2602a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2602a-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2602a-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2602a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2602a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2602a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2602a-113">Not supported.</span></span>    |
|<span data-ttu-id="2602a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2602a-114">Application</span></span> | <span data-ttu-id="2602a-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2602a-115">Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="2602a-116">**Observação**: Esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="2602a-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="2602a-117">Administradores globais e administradores de serviço de Teams da Microsoft podem acessar as equipes que eles não serão um membro do.</span><span class="sxs-lookup"><span data-stu-id="2602a-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="2602a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2602a-118">HTTP request</span></span>
```http
GET /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2602a-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2602a-119">Optional query parameters</span></span>

<span data-ttu-id="2602a-120">Este método oferece suporte a $select e $expand [OData parâmetros de consulta](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2602a-120">This method supports the $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2602a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2602a-121">Request headers</span></span>
| <span data-ttu-id="2602a-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2602a-122">Header</span></span>       | <span data-ttu-id="2602a-123">Valor</span><span class="sxs-lookup"><span data-stu-id="2602a-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2602a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2602a-124">Authorization</span></span>  | <span data-ttu-id="2602a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2602a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2602a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2602a-127">Request body</span></span>
<span data-ttu-id="2602a-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2602a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2602a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2602a-129">Response</span></span>

<span data-ttu-id="2602a-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [tab](../resources/teamstab.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2602a-130">If successful, this method returns a `200 OK` response code and a [tab](../resources/teamstab.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2602a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2602a-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2602a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2602a-132">Request</span></span>
<span data-ttu-id="2602a-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2602a-133">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="2602a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2602a-134">Response</span></span>
<span data-ttu-id="2602a-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2602a-135">The following is an example of the response.</span></span> 

><span data-ttu-id="2602a-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2602a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
