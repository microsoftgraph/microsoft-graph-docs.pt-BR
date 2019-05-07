---
title: 'servicePrincipalName: Adicionar proprietário'
description: Use esta API para adicionar um proprietário para a entidade de serviço.
localization_priority: Normal
ms.openlocfilehash: 6da4b2b7b9ae83aae5bd818454047cdb31166484
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638589"
---
# <a name="serviceprincipal-add-owner"></a><span data-ttu-id="962bf-103">servicePrincipalName: Adicionar proprietário</span><span class="sxs-lookup"><span data-stu-id="962bf-103">servicePrincipal: Add owner</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="962bf-104">Use esta API para adicionar um proprietário para a entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="962bf-104">Use this API to add an owner for the service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="962bf-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="962bf-105">Permissions</span></span>
<span data-ttu-id="962bf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="962bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="962bf-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="962bf-108">Permission type</span></span>      | <span data-ttu-id="962bf-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="962bf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="962bf-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="962bf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="962bf-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="962bf-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="962bf-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="962bf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="962bf-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="962bf-113">Not supported.</span></span>    |
|<span data-ttu-id="962bf-114">Application</span><span class="sxs-lookup"><span data-stu-id="962bf-114">Application</span></span> | <span data-ttu-id="962bf-115">Application. ReadWrite. OwnedBy e Directory. Read. All, Application. ReadWrite. All e Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="962bf-115">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="962bf-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="962bf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/owners

```
## <a name="request-headers"></a><span data-ttu-id="962bf-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="962bf-117">Request headers</span></span>
| <span data-ttu-id="962bf-118">Nome</span><span class="sxs-lookup"><span data-stu-id="962bf-118">Name</span></span>       | <span data-ttu-id="962bf-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="962bf-119">Type</span></span> | <span data-ttu-id="962bf-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="962bf-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="962bf-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="962bf-121">Authorization</span></span>  | <span data-ttu-id="962bf-122">string</span><span class="sxs-lookup"><span data-stu-id="962bf-122">string</span></span>  | <span data-ttu-id="962bf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="962bf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="962bf-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="962bf-125">Request body</span></span>
<span data-ttu-id="962bf-126">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="962bf-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="962bf-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="962bf-127">Response</span></span>

<span data-ttu-id="962bf-128">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="962bf-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="962bf-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="962bf-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="962bf-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="962bf-130">Request</span></span>
<span data-ttu-id="962bf-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="962bf-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_serviceprincipal"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/owners
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
<span data-ttu-id="962bf-132">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="962bf-132">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="962bf-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="962bf-133">Response</span></span>
<span data-ttu-id="962bf-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="962bf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "directoryObject": {
    "id": "id-value"
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="962bf-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="962bf-137">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="962bf-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="962bf-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_serviceprincipal-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-post-owners.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
