---
title: Atualizar synchronizationTemplate
description: Atualização (substituição) o modelo de sincronização associado a um determinado aplicativo.
localization_priority: Normal
ms.openlocfilehash: ea4dfdc418d04467a6060a8c3d7d83423ba16e38
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816734"
---
# <a name="update-synchronizationtemplate"></a><span data-ttu-id="8f770-103">Atualizar synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="8f770-103">Update synchronizationTemplate</span></span>

> <span data-ttu-id="8f770-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8f770-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f770-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8f770-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8f770-106">Atualização (substituição) o modelo de sincronização associado a um determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8f770-106">Update (override) the synchronization template associated with a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f770-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="8f770-107">Permissions</span></span>
<span data-ttu-id="8f770-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f770-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f770-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f770-110">Permission type</span></span>                        | <span data-ttu-id="8f770-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8f770-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f770-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f770-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="8f770-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f770-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="8f770-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f770-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="8f770-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f770-115">Not supported.</span></span>|
|<span data-ttu-id="8f770-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f770-116">Application</span></span>                            |<span data-ttu-id="8f770-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f770-117">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="8f770-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f770-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT application/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="8f770-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f770-119">Request headers</span></span>

| <span data-ttu-id="8f770-120">Nome</span><span class="sxs-lookup"><span data-stu-id="8f770-120">Name</span></span>           | <span data-ttu-id="8f770-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f770-121">Type</span></span>    | <span data-ttu-id="8f770-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f770-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="8f770-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f770-123">Authorization</span></span>  | <span data-ttu-id="8f770-124">string</span><span class="sxs-lookup"><span data-stu-id="8f770-124">string</span></span>  | <span data-ttu-id="8f770-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f770-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f770-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f770-127">Request body</span></span>

<span data-ttu-id="8f770-128">No corpo da solicitação, fornece o objeto [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) para substituir o modelo existente.</span><span class="sxs-lookup"><span data-stu-id="8f770-128">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to replace the existing template.</span></span> <span data-ttu-id="8f770-129">Verifique se que todas as propriedades são fornecidas.</span><span class="sxs-lookup"><span data-stu-id="8f770-129">Make sure all properties are provided.</span></span> <span data-ttu-id="8f770-130">Propriedades ausentes serão apagadas.</span><span class="sxs-lookup"><span data-stu-id="8f770-130">Missing properties will be erased.</span></span>

### <a name="response"></a><span data-ttu-id="8f770-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f770-131">Response</span></span>

<span data-ttu-id="8f770-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8f770-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="examples"></a><span data-ttu-id="8f770-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8f770-134">Examples</span></span>

##### <a name="request"></a><span data-ttu-id="8f770-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f770-135">Request</span></span>
<span data-ttu-id="8f770-136">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f770-136">The following is an example of a request.</span></span> 

><span data-ttu-id="8f770-137">**Observação:** O objeto request mostrado aqui é abreviado para fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8f770-137">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="8f770-138">Inclua todas as propriedades em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8f770-138">Include all the properties in an actual call.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_synchronizationtemplate"
}-->
```http
PUT https://graph.microsoft.com/beta/applications/{id}/synchronization/templates/{templateId}
Authorization: Bearer <token>
Content-type: application/json

{
    "id": "Slack",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM"
}
```

##### <a name="response"></a><span data-ttu-id="8f770-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f770-139">Response</span></span>
<span data-ttu-id="8f770-140">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="8f770-140">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update synchronizationtemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
