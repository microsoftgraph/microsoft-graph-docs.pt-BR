---
title: Obtenha o guia
description: 'Recupere as propriedades e relacionamentos da guia especificado. '
ms.openlocfilehash: 7bef495fbb37a878a291f2aac6004d386e932cbd
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2018
ms.locfileid: "27222405"
---
# <a name="get-tab"></a><span data-ttu-id="ff3ca-103">Obtenha o guia</span><span class="sxs-lookup"><span data-stu-id="ff3ca-103">Get tab</span></span>

> <span data-ttu-id="ff3ca-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ff3ca-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff3ca-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ff3ca-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ff3ca-106">Recupere as propriedades e relacionamentos da [guia](../resources/teamstab.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="ff3ca-106">Retrieve the properties and relationships of the specified [tab](../resources/teamstab.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="ff3ca-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="ff3ca-107">Permissions</span></span>
<span data-ttu-id="ff3ca-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff3ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff3ca-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff3ca-110">Permission type</span></span>      | <span data-ttu-id="ff3ca-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ff3ca-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff3ca-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff3ca-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ff3ca-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff3ca-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ff3ca-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff3ca-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff3ca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff3ca-115">Not supported.</span></span>    |
|<span data-ttu-id="ff3ca-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff3ca-116">Application</span></span> | <span data-ttu-id="ff3ca-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff3ca-117">Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="ff3ca-118">**Observação**: Esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="ff3ca-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="ff3ca-119">Administradores globais e administradores de serviço de Teams da Microsoft podem acessar as equipes que eles não serão um membro do.</span><span class="sxs-lookup"><span data-stu-id="ff3ca-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="ff3ca-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff3ca-120">HTTP request</span></span>
```http
GET /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ff3ca-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ff3ca-121">Optional query parameters</span></span>

<span data-ttu-id="ff3ca-122">Este método oferece suporte a $select e $expand [OData parâmetros de consulta](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ff3ca-122">This method supports the $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ff3ca-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff3ca-123">Request headers</span></span>
| <span data-ttu-id="ff3ca-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ff3ca-124">Header</span></span>       | <span data-ttu-id="ff3ca-125">Valor</span><span class="sxs-lookup"><span data-stu-id="ff3ca-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ff3ca-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff3ca-126">Authorization</span></span>  | <span data-ttu-id="ff3ca-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff3ca-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ff3ca-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff3ca-129">Request body</span></span>
<span data-ttu-id="ff3ca-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ff3ca-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff3ca-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff3ca-131">Response</span></span>

<span data-ttu-id="ff3ca-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [tab](../resources/teamstab.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff3ca-132">If successful, this method returns a `200 OK` response code and a [tab](../resources/teamstab.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ff3ca-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff3ca-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ff3ca-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff3ca-134">Request</span></span>
<span data-ttu-id="ff3ca-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff3ca-135">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="ff3ca-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff3ca-136">Response</span></span>
<span data-ttu-id="ff3ca-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ff3ca-137">The following is an example of the response.</span></span> 

><span data-ttu-id="ff3ca-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff3ca-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
