---
title: 'servicePrincipal: Adicionar proprietário'
description: Use essa API para adicionar um proprietário para a entidade de serviço.
ms.openlocfilehash: 79ffb0d8d6c680b517421455cee011b3764c8f15
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039348"
---
# <a name="serviceprincipal-add-owner"></a><span data-ttu-id="e3e18-103">servicePrincipal: Adicionar proprietário</span><span class="sxs-lookup"><span data-stu-id="e3e18-103">servicePrincipal: Add owner</span></span>

> <span data-ttu-id="e3e18-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e3e18-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3e18-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e3e18-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e3e18-106">Use essa API para adicionar um proprietário para a entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="e3e18-106">Use this API to add an owner for the service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3e18-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="e3e18-107">Permissions</span></span>
<span data-ttu-id="e3e18-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3e18-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3e18-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3e18-110">Permission type</span></span>      | <span data-ttu-id="e3e18-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e3e18-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3e18-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3e18-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e3e18-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e3e18-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e3e18-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3e18-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3e18-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3e18-115">Not supported.</span></span>    |
|<span data-ttu-id="e3e18-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3e18-116">Application</span></span> | <span data-ttu-id="e3e18-117">Application.ReadWrite.OwnedBy e Directory.Read.All, Application.ReadWrite.All e Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3e18-117">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3e18-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3e18-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/owners

```
## <a name="request-headers"></a><span data-ttu-id="e3e18-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3e18-119">Request headers</span></span>
| <span data-ttu-id="e3e18-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e3e18-120">Name</span></span>       | <span data-ttu-id="e3e18-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3e18-121">Type</span></span> | <span data-ttu-id="e3e18-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3e18-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e3e18-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3e18-123">Authorization</span></span>  | <span data-ttu-id="e3e18-124">string</span><span class="sxs-lookup"><span data-stu-id="e3e18-124">string</span></span>  | <span data-ttu-id="e3e18-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3e18-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3e18-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3e18-127">Request body</span></span>
<span data-ttu-id="e3e18-128">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="e3e18-128">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e3e18-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3e18-129">Response</span></span>

<span data-ttu-id="e3e18-130">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3e18-130">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3e18-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3e18-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3e18-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3e18-132">Request</span></span>
<span data-ttu-id="e3e18-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3e18-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="e3e18-134">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="e3e18-134">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e3e18-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3e18-135">Response</span></span>
<span data-ttu-id="e3e18-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3e18-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->