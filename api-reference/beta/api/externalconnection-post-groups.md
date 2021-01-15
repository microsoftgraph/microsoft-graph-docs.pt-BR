---
title: Criar externalGroup
description: Criar um novo objeto externalGroup.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 6ca8968daf3abb98bba66a4146fc3b41c9d54441
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873042"
---
# <a name="create-externalgroup"></a><span data-ttu-id="5c637-103">Criar externalGroup</span><span class="sxs-lookup"><span data-stu-id="5c637-103">Create externalGroup</span></span>

<span data-ttu-id="5c637-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c637-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c637-105">Criar um novo [objeto externalGroup.](../resources/externalgroup.md)</span><span class="sxs-lookup"><span data-stu-id="5c637-105">Create a new [externalGroup](../resources/externalgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c637-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c637-106">Permissions</span></span>

<span data-ttu-id="5c637-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c637-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5c637-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c637-109">Permission type</span></span>                        | <span data-ttu-id="5c637-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c637-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5c637-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c637-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5c637-112">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5c637-112">Not supported</span></span>                               |
| <span data-ttu-id="5c637-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c637-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c637-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5c637-114">Not supported</span></span>                               |
| <span data-ttu-id="5c637-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c637-115">Application</span></span>                            | <span data-ttu-id="5c637-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c637-116">ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="5c637-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c637-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /external/connections/{connectionId}/groups
```

## <a name="request-headers"></a><span data-ttu-id="5c637-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c637-118">Request headers</span></span>

| <span data-ttu-id="5c637-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5c637-119">Name</span></span>          | <span data-ttu-id="5c637-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c637-120">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="5c637-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c637-121">Authorization</span></span> | <span data-ttu-id="5c637-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c637-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="5c637-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5c637-124">Content-Type</span></span>  | <span data-ttu-id="5c637-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c637-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c637-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c637-127">Request body</span></span>

<span data-ttu-id="5c637-128">No corpo da solicitação, fornece uma representação JSON do [objeto externalGroup.](../resources/externalgroup.md)</span><span class="sxs-lookup"><span data-stu-id="5c637-128">In the request body, supply a JSON representation of the [externalGroup](../resources/externalgroup.md) object.</span></span>

<span data-ttu-id="5c637-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [externalGroup](../resources/externalgroup.md).</span><span class="sxs-lookup"><span data-stu-id="5c637-129">The following table shows the properties that are required when you create the [externalGroup](../resources/externalgroup.md).</span></span>

| <span data-ttu-id="5c637-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5c637-130">Property</span></span>    | <span data-ttu-id="5c637-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c637-131">Type</span></span>   | <span data-ttu-id="5c637-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c637-132">Description</span></span>                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="5c637-133">id</span><span class="sxs-lookup"><span data-stu-id="5c637-133">id</span></span>          | <span data-ttu-id="5c637-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c637-134">String</span></span> | <span data-ttu-id="5c637-135">A ID exclusiva do grupo externo dentro de uma conexão.</span><span class="sxs-lookup"><span data-stu-id="5c637-135">The unique ID of the external group within a connection.</span></span> <span data-ttu-id="5c637-136">Ele deve ser alfanumérico e ter até 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="5c637-136">It must be alphanumeric and can be up to 128 characters long.</span></span> |
| <span data-ttu-id="5c637-137">displayName</span><span class="sxs-lookup"><span data-stu-id="5c637-137">displayName</span></span> | <span data-ttu-id="5c637-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c637-138">String</span></span> | <span data-ttu-id="5c637-139">O nome amigável do grupo externo.</span><span class="sxs-lookup"><span data-stu-id="5c637-139">The friendly name of the external group.</span></span> <span data-ttu-id="5c637-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5c637-140">Optional.</span></span>                                                                      |
| <span data-ttu-id="5c637-141">description</span><span class="sxs-lookup"><span data-stu-id="5c637-141">description</span></span> | <span data-ttu-id="5c637-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c637-142">String</span></span> | <span data-ttu-id="5c637-143">A descrição do grupo externo.</span><span class="sxs-lookup"><span data-stu-id="5c637-143">The description of the external group.</span></span> <span data-ttu-id="5c637-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5c637-144">Optional.</span></span>                                                                         |

## <a name="response"></a><span data-ttu-id="5c637-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c637-145">Response</span></span>

<span data-ttu-id="5c637-146">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um objeto [externalGroup](../resources/externalgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c637-146">If successful, this method returns a `201 Created` response code and an [externalGroup](../resources/externalgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5c637-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5c637-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5c637-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c637-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5c637-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c637-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalgroup_from_connection"
}
-->

``` http
POST https://graph.microsoft.com/beta/external/connections/contosohr/groups
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroup",
  "id": "31bea3d537902000",
  "displayName": "Contoso Marketing",
  "description": "The product marketing team"
}
```
# <a name="c"></a>[<span data-ttu-id="5c637-150">C#</span><span class="sxs-lookup"><span data-stu-id="5c637-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalgroup-from-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c637-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c637-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalgroup-from-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c637-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c637-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalgroup-from-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c637-153">Java</span><span class="sxs-lookup"><span data-stu-id="5c637-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-externalgroup-from-connection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="5c637-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c637-154">Response</span></span>

<span data-ttu-id="5c637-155">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5c637-155">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalGroup"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroup",
  "id": "31bea3d537902000",
  "displayName": "Contoso Marketing",
  "description": "The product marketing team"
}
```
