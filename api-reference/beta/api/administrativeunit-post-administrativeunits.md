---
title: Criar administrativeUnit
description: Use essa API para criar um novo administrativeUnit.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fb918d690ceaaa232b4911b5f47a2b381a79444d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917164"
---
# <a name="create-administrativeunit"></a><span data-ttu-id="df8b9-103">Criar administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="df8b9-103">Create administrativeUnit</span></span>

> <span data-ttu-id="df8b9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="df8b9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df8b9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="df8b9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="df8b9-106">Use essa API para criar um novo [administrativeUnit](../resources/administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="df8b9-106">Use this API to create a new [administrativeUnit](../resources/administrativeunit.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="df8b9-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="df8b9-107">Permissions</span></span>
<span data-ttu-id="df8b9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df8b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="df8b9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df8b9-110">Permission type</span></span>      | <span data-ttu-id="df8b9-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="df8b9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df8b9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df8b9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="df8b9-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="df8b9-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="df8b9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df8b9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df8b9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df8b9-115">Not supported.</span></span>    |
|<span data-ttu-id="df8b9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df8b9-116">Application</span></span> | <span data-ttu-id="df8b9-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df8b9-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="df8b9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df8b9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits

```
## <a name="request-headers"></a><span data-ttu-id="df8b9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df8b9-119">Request headers</span></span>
| <span data-ttu-id="df8b9-120">Nome</span><span class="sxs-lookup"><span data-stu-id="df8b9-120">Name</span></span>      |<span data-ttu-id="df8b9-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="df8b9-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="df8b9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="df8b9-122">Authorization</span></span>  | <span data-ttu-id="df8b9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df8b9-p103">Bearer {token}. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="df8b9-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df8b9-125">Request body</span></span>
<span data-ttu-id="df8b9-126">No corpo da solicitação, fornece uma representação JSON do objeto [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="df8b9-126">In the request body, supply a JSON representation of [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="df8b9-127">Desde que o recurso de **administrativeUnit** oferece suporte às [extensões](/graph/extensibility-overview), você pode usar o `POST` operação e adicionar propriedades personalizadas com seus próprios dados para a unidade administrativa ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="df8b9-127">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the administrative unit while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="df8b9-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="df8b9-128">Response</span></span>

<span data-ttu-id="df8b9-129">Se tiver êxito, este método retornará `201 Created` objeto response de código e [administrativeUnit](../resources/administrativeunit.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df8b9-129">If successful, this method returns `201 Created` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df8b9-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df8b9-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="df8b9-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df8b9-131">Request</span></span>
<span data-ttu-id="df8b9-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="df8b9-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_administrativeunit_from_administrativeunits"
}-->
```http
POST https://graph.microsoft.com/beta/administrativeUnits
Content-type: application/json
Content-length: 150

{
    "displayName": "Seattle District Technical Schools",
    "description": "Seattle district technical schools administration",
    "visibility": "true"
}
```
<span data-ttu-id="df8b9-133">No corpo da solicitação, fornece uma representação JSON do objeto [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="df8b9-133">In the request body, supply a JSON representation of [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="df8b9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="df8b9-134">Response</span></span>
<span data-ttu-id="df8b9-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df8b9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 172

{
  "administrativeUnit": {
    "displayName": "Seattle District Technical Schools",
    "description": "Seattle district technical schools administration",
    "visibility": "true",
    "id": "7a3dc8f3-b3a0-4164-9a99-ed36f3af039f"
  }
}
```

## <a name="see-also"></a><span data-ttu-id="df8b9-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="df8b9-138">See also</span></span>

- [<span data-ttu-id="df8b9-139">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="df8b9-139">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="df8b9-140">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="df8b9-140">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
