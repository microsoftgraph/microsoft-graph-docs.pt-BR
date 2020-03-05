---
title: 'servicePrincipalName: Adicionar proprietário'
description: Use esta API para adicionar um proprietário para a entidade de serviço.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 7379c07d7ba3704fc2e44f2a46744418be54b4af
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453344"
---
# <a name="serviceprincipal-add-owner"></a><span data-ttu-id="671c5-103">servicePrincipalName: Adicionar proprietário</span><span class="sxs-lookup"><span data-stu-id="671c5-103">servicePrincipal: Add owner</span></span>

<span data-ttu-id="671c5-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="671c5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="671c5-105">Use esta API para adicionar um proprietário para a entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="671c5-105">Use this API to add an owner for the service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="671c5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="671c5-106">Permissions</span></span>
<span data-ttu-id="671c5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="671c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="671c5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="671c5-109">Permission type</span></span>      | <span data-ttu-id="671c5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="671c5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="671c5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="671c5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="671c5-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="671c5-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="671c5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="671c5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="671c5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="671c5-114">Not supported.</span></span>    |
|<span data-ttu-id="671c5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="671c5-115">Application</span></span> | <span data-ttu-id="671c5-116">Application. ReadWrite. OwnedBy e Directory. Read. All, Application. ReadWrite. All e Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="671c5-116">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="671c5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="671c5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/owners

```
## <a name="request-headers"></a><span data-ttu-id="671c5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="671c5-118">Request headers</span></span>
| <span data-ttu-id="671c5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="671c5-119">Name</span></span>       | <span data-ttu-id="671c5-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="671c5-120">Type</span></span> | <span data-ttu-id="671c5-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="671c5-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="671c5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="671c5-122">Authorization</span></span>  | <span data-ttu-id="671c5-123">string</span><span class="sxs-lookup"><span data-stu-id="671c5-123">string</span></span>  | <span data-ttu-id="671c5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="671c5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="671c5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="671c5-126">Request body</span></span>
<span data-ttu-id="671c5-127">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="671c5-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="671c5-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="671c5-128">Response</span></span>

<span data-ttu-id="671c5-129">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="671c5-129">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="671c5-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="671c5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="671c5-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="671c5-131">Request</span></span>
<span data-ttu-id="671c5-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="671c5-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="671c5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="671c5-133">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="671c5-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="671c5-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="671c5-135">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="671c5-135">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="671c5-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="671c5-136">Response</span></span>
<span data-ttu-id="671c5-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="671c5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
