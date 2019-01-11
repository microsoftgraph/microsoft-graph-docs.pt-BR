---
title: 'servicePrincipal: Adicionar proprietário'
description: Use essa API para adicionar um proprietário para a entidade de serviço.
localization_priority: Normal
ms.openlocfilehash: 1bfb82589c730512ba877a94b55d565a6a44d4b9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887154"
---
# <a name="serviceprincipal-add-owner"></a><span data-ttu-id="6ecdc-103">servicePrincipal: Adicionar proprietário</span><span class="sxs-lookup"><span data-stu-id="6ecdc-103">servicePrincipal: Add owner</span></span>

> <span data-ttu-id="6ecdc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6ecdc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ecdc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6ecdc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6ecdc-106">Use essa API para adicionar um proprietário para a entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="6ecdc-106">Use this API to add an owner for the service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ecdc-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="6ecdc-107">Permissions</span></span>
<span data-ttu-id="6ecdc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ecdc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ecdc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ecdc-110">Permission type</span></span>      | <span data-ttu-id="6ecdc-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6ecdc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ecdc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ecdc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6ecdc-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6ecdc-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6ecdc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ecdc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ecdc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ecdc-115">Not supported.</span></span>    |
|<span data-ttu-id="6ecdc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ecdc-116">Application</span></span> | <span data-ttu-id="6ecdc-117">Application.ReadWrite.OwnedBy e Directory.Read.All, Application.ReadWrite.All e Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ecdc-117">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ecdc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ecdc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/owners

```
## <a name="request-headers"></a><span data-ttu-id="6ecdc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6ecdc-119">Request headers</span></span>
| <span data-ttu-id="6ecdc-120">Nome</span><span class="sxs-lookup"><span data-stu-id="6ecdc-120">Name</span></span>       | <span data-ttu-id="6ecdc-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ecdc-121">Type</span></span> | <span data-ttu-id="6ecdc-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ecdc-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6ecdc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6ecdc-123">Authorization</span></span>  | <span data-ttu-id="6ecdc-124">string</span><span class="sxs-lookup"><span data-stu-id="6ecdc-124">string</span></span>  | <span data-ttu-id="6ecdc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ecdc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6ecdc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6ecdc-127">Request body</span></span>
<span data-ttu-id="6ecdc-128">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="6ecdc-128">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6ecdc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ecdc-129">Response</span></span>

<span data-ttu-id="6ecdc-130">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ecdc-130">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ecdc-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6ecdc-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6ecdc-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ecdc-132">Request</span></span>
<span data-ttu-id="6ecdc-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6ecdc-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="6ecdc-134">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="6ecdc-134">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="6ecdc-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ecdc-135">Response</span></span>
<span data-ttu-id="6ecdc-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6ecdc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
