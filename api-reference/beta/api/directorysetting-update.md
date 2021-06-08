---
title: Atualizar uma configuração de diretório
description: Atualize as propriedades de um objeto de configuração de diretório específico.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 08f6c51413f751a0ce5a2818969e253d32f5e2fe
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786829"
---
# <a name="update-a-directory-setting"></a><span data-ttu-id="1dd3d-103">Atualizar uma configuração de diretório</span><span class="sxs-lookup"><span data-stu-id="1dd3d-103">Update a directory setting</span></span>

<span data-ttu-id="1dd3d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1dd3d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1dd3d-105">Atualize as propriedades de um objeto de configuração de diretório específico.</span><span class="sxs-lookup"><span data-stu-id="1dd3d-105">Update the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="1dd3d-106">**Observação**: a versão /beta dessa API só se aplica a grupos.</span><span class="sxs-lookup"><span data-stu-id="1dd3d-106">**Note**: The /beta version of this API only applies to groups.</span></span> <span data-ttu-id="1dd3d-107">A versão /v1.0 desta API foi renomeada para *Update groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="1dd3d-107">The /v1.0 version of this API has been renamed to *Update groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="1dd3d-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="1dd3d-108">Permissions</span></span>
<span data-ttu-id="1dd3d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1dd3d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dd3d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1dd3d-111">Permission type</span></span>      | <span data-ttu-id="1dd3d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1dd3d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1dd3d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1dd3d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1dd3d-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1dd3d-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1dd3d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1dd3d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1dd3d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1dd3d-116">Not supported.</span></span>    |
|<span data-ttu-id="1dd3d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1dd3d-117">Application</span></span> | <span data-ttu-id="1dd3d-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dd3d-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1dd3d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1dd3d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="1dd3d-120">Atualizar uma configuração específica de grupo ou de locatário como um todo.</span><span class="sxs-lookup"><span data-stu-id="1dd3d-120">Update a tenant-wide or group specific setting.</span></span>
```http
PATCH /settings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="1dd3d-121">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="1dd3d-121">Optional request headers</span></span>
| <span data-ttu-id="1dd3d-122">Nome</span><span class="sxs-lookup"><span data-stu-id="1dd3d-122">Name</span></span>       | <span data-ttu-id="1dd3d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1dd3d-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1dd3d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1dd3d-124">Authorization</span></span>  | <span data-ttu-id="1dd3d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1dd3d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1dd3d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1dd3d-127">Request body</span></span>
<span data-ttu-id="1dd3d-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="1dd3d-128">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="1dd3d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1dd3d-129">Property</span></span>     | <span data-ttu-id="1dd3d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1dd3d-130">Type</span></span>   |<span data-ttu-id="1dd3d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1dd3d-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1dd3d-132">values</span><span class="sxs-lookup"><span data-stu-id="1dd3d-132">values</span></span> | <span data-ttu-id="1dd3d-133">[coleção settingValue](../resources/settingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="1dd3d-133">[settingValue](../resources/settingvalue.md) collection</span></span> | <span data-ttu-id="1dd3d-p104">O conjunto atualizado de valores.  OBSERVAÇÃO: Você deve fornecer o conjunto inteiro. Você não pode atualizar um único conjunto de valores.</span><span class="sxs-lookup"><span data-stu-id="1dd3d-p104">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="1dd3d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dd3d-137">Response</span></span>

<span data-ttu-id="1dd3d-138">Se tiver êxito, este método retornará um código de resposta `204 OK`.</span><span class="sxs-lookup"><span data-stu-id="1dd3d-138">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1dd3d-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1dd3d-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1dd3d-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1dd3d-140">Request</span></span>
<span data-ttu-id="1dd3d-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1dd3d-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1dd3d-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="1dd3d-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_directorysetting"
}-->
```http
PATCH https://graph.microsoft.com/beta/settings/{id}
Content-type: application/json
Content-length: 178

{
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="1dd3d-143">C#</span><span class="sxs-lookup"><span data-stu-id="1dd3d-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-directorysetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1dd3d-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1dd3d-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-directorysetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1dd3d-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1dd3d-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-directorysetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1dd3d-146">Java</span><span class="sxs-lookup"><span data-stu-id="1dd3d-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-directorysetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1dd3d-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dd3d-147">Response</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update directorysetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


