---
title: Guia de atualização
description: Atualize as propriedades da guia especificada.
ms.openlocfilehash: fb2346fbadcb9794e05f8bb583596536a5710052
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006605"
---
# <a name="update-tab"></a><span data-ttu-id="cad70-103">Guia de atualização</span><span class="sxs-lookup"><span data-stu-id="cad70-103">Update tab</span></span>



<span data-ttu-id="cad70-104">Atualize as propriedades da [guia](../resources/teamstab.md)especificado. Isso pode ser usado para configurar o conteúdo da guia.</span><span class="sxs-lookup"><span data-stu-id="cad70-104">Update the properties of the specified [tab](../resources/teamstab.md). This can be used to configure the content of the tab.</span></span>

## <a name="permissions"></a><span data-ttu-id="cad70-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="cad70-105">Permissions</span></span>
<span data-ttu-id="cad70-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cad70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cad70-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cad70-108">Permission type</span></span>      | <span data-ttu-id="cad70-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cad70-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cad70-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cad70-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cad70-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cad70-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cad70-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cad70-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cad70-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cad70-113">Not supported.</span></span>    |
|<span data-ttu-id="cad70-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cad70-114">Application</span></span>                            | <span data-ttu-id="cad70-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cad70-115">Group.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="cad70-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cad70-116">HTTP request</span></span>
```http
PATCH /teams/{id}/channels/{id}/tabs/{id}
```
## <a name="request-headers"></a><span data-ttu-id="cad70-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cad70-117">Request headers</span></span>
| <span data-ttu-id="cad70-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cad70-118">Header</span></span>       | <span data-ttu-id="cad70-119">Valor</span><span class="sxs-lookup"><span data-stu-id="cad70-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cad70-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="cad70-120">Authorization</span></span>  | <span data-ttu-id="cad70-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cad70-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cad70-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cad70-123">Content-Type</span></span>  | <span data-ttu-id="cad70-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cad70-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cad70-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cad70-125">Request body</span></span>
<span data-ttu-id="cad70-126">No corpo da solicitação, fornece uma representação de JSON do objeto [tab](../resources/teamstab.md) .</span><span class="sxs-lookup"><span data-stu-id="cad70-126">In the request body, supply a JSON representation of [tab](../resources/teamstab.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cad70-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="cad70-127">Response</span></span>

<span data-ttu-id="cad70-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cad70-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cad70-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cad70-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="cad70-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cad70-130">Request</span></span>
<span data-ttu-id="cad70-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cad70-131">The following is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
Content-type: application/json
Content-length: 211

{
  "name": "My Contoso Tab - updated"
}
```
#### <a name="response"></a><span data-ttu-id="cad70-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="cad70-132">Response</span></span>
```http
HTTP/1.1 200 Success
Content-type: application/json

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

## <a name="see-also"></a><span data-ttu-id="cad70-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="cad70-133">See also</span></span>

[<span data-ttu-id="cad70-134">Configurando os tipos de guia interna</span><span class="sxs-lookup"><span data-stu-id="cad70-134">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tab in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
