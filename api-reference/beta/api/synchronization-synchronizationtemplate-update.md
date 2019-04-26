---
title: Atualizar synchronizationtemplate
description: Atualizar (substituir) o modelo de sincronização associado a um determinado aplicativo.
localization_priority: Normal
ms.openlocfilehash: 12b2b2679bbe62ea6cc2842a68c64fdfdf3a5cda
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330522"
---
# <a name="update-synchronizationtemplate"></a><span data-ttu-id="04ff7-103">Atualizar synchronizationtemplate</span><span class="sxs-lookup"><span data-stu-id="04ff7-103">Update synchronizationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04ff7-104">Atualizar (substituir) o modelo de sincronização associado a um determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="04ff7-104">Update (override) the synchronization template associated with a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="04ff7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="04ff7-105">Permissions</span></span>
<span data-ttu-id="04ff7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04ff7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04ff7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04ff7-108">Permission type</span></span>                        | <span data-ttu-id="04ff7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="04ff7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="04ff7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04ff7-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="04ff7-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04ff7-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="04ff7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04ff7-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="04ff7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04ff7-113">Not supported.</span></span>|
|<span data-ttu-id="04ff7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04ff7-114">Application</span></span>                            |<span data-ttu-id="04ff7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04ff7-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="04ff7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04ff7-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT application/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="04ff7-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04ff7-117">Request headers</span></span>

| <span data-ttu-id="04ff7-118">Nome</span><span class="sxs-lookup"><span data-stu-id="04ff7-118">Name</span></span>           | <span data-ttu-id="04ff7-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="04ff7-119">Type</span></span>    | <span data-ttu-id="04ff7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="04ff7-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="04ff7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="04ff7-121">Authorization</span></span>  | <span data-ttu-id="04ff7-122">string</span><span class="sxs-lookup"><span data-stu-id="04ff7-122">string</span></span>  | <span data-ttu-id="04ff7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04ff7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04ff7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04ff7-125">Request body</span></span>

<span data-ttu-id="04ff7-126">No corpo da solicitação, forneça o [](../resources/synchronization-synchronizationtemplate.md) objeto synchronizationtemplate para substituir o modelo existente.</span><span class="sxs-lookup"><span data-stu-id="04ff7-126">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to replace the existing template.</span></span> <span data-ttu-id="04ff7-127">Certifique-se de que todas as propriedades sejam fornecidas.</span><span class="sxs-lookup"><span data-stu-id="04ff7-127">Make sure all properties are provided.</span></span> <span data-ttu-id="04ff7-128">As propriedades ausentes serão apagadas.</span><span class="sxs-lookup"><span data-stu-id="04ff7-128">Missing properties will be erased.</span></span>

### <a name="response"></a><span data-ttu-id="04ff7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="04ff7-129">Response</span></span>

<span data-ttu-id="04ff7-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04ff7-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="examples"></a><span data-ttu-id="04ff7-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="04ff7-132">Examples</span></span>

##### <a name="request"></a><span data-ttu-id="04ff7-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04ff7-133">Request</span></span>
<span data-ttu-id="04ff7-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="04ff7-134">The following is an example of a request.</span></span> 

><span data-ttu-id="04ff7-135">**Observação:** O objeto Request mostrado aqui é reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="04ff7-135">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="04ff7-136">Incluir todas as propriedades em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="04ff7-136">Include all the properties in an actual call.</span></span>
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

##### <a name="response"></a><span data-ttu-id="04ff7-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="04ff7-137">Response</span></span>
<span data-ttu-id="04ff7-138">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="04ff7-138">The following is an example of a response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update synchronizationtemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
