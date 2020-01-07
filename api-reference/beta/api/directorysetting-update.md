---
title: Atualizar uma configuração de diretório
description: Atualiza as propriedades de um objeto de configuração de diretório específico.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e37c5b6886b5432395a9d70344d50251f1689ee5
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2020
ms.locfileid: "40951658"
---
# <a name="update-a-directory-setting"></a><span data-ttu-id="370b5-103">Atualizar uma configuração de diretório</span><span class="sxs-lookup"><span data-stu-id="370b5-103">Update a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="370b5-104">Atualiza as propriedades de um objeto de configuração de diretório específico.</span><span class="sxs-lookup"><span data-stu-id="370b5-104">Update the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="370b5-105">**Observação**: a versão do/beta desta API só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="370b5-105">**Note**: The /beta version of this API only applies to groups.</span></span> <span data-ttu-id="370b5-106">A versão/v1.0 dessa API foi renomeada para atualizar o *groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="370b5-106">The /v1.0 version of this API has been renamed to *Update groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="370b5-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="370b5-107">Permissions</span></span>
<span data-ttu-id="370b5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="370b5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="370b5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="370b5-110">Permission type</span></span>      | <span data-ttu-id="370b5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="370b5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="370b5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="370b5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="370b5-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="370b5-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="370b5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="370b5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="370b5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="370b5-115">Not supported.</span></span>    |
|<span data-ttu-id="370b5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="370b5-116">Application</span></span> | <span data-ttu-id="370b5-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="370b5-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="370b5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="370b5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="370b5-119">Atualizar uma configuração específica de grupo ou de locatário como um todo.</span><span class="sxs-lookup"><span data-stu-id="370b5-119">Update a tenant-wide or group specific setting.</span></span>
```http
PATCH /settings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="370b5-120">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="370b5-120">Optional request headers</span></span>
| <span data-ttu-id="370b5-121">Nome</span><span class="sxs-lookup"><span data-stu-id="370b5-121">Name</span></span>       | <span data-ttu-id="370b5-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="370b5-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="370b5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="370b5-123">Authorization</span></span>  | <span data-ttu-id="370b5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="370b5-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="370b5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="370b5-126">Request body</span></span>
<span data-ttu-id="370b5-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="370b5-127">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="370b5-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="370b5-128">Property</span></span>     | <span data-ttu-id="370b5-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="370b5-129">Type</span></span>   |<span data-ttu-id="370b5-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="370b5-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="370b5-131">values</span><span class="sxs-lookup"><span data-stu-id="370b5-131">values</span></span> | <span data-ttu-id="370b5-132">coleção [SettingValue](../resources/settingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="370b5-132">[settingValue](../resources/settingvalue.md) collection</span></span> | <span data-ttu-id="370b5-p104">O conjunto atualizado de valores.  OBSERVAÇÃO: Você deve fornecer o conjunto inteiro. Você não pode atualizar um único conjunto de valores.</span><span class="sxs-lookup"><span data-stu-id="370b5-p104">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="370b5-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="370b5-136">Response</span></span>

<span data-ttu-id="370b5-137">Se tiver êxito, este método retornará um código de resposta `204 OK`.</span><span class="sxs-lookup"><span data-stu-id="370b5-137">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="370b5-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="370b5-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="370b5-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="370b5-139">Request</span></span>
<span data-ttu-id="370b5-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="370b5-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="370b5-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="370b5-141">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="370b5-142">C#</span><span class="sxs-lookup"><span data-stu-id="370b5-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-directorysetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="370b5-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="370b5-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-directorysetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="370b5-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="370b5-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-directorysetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="370b5-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="370b5-145">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorysetting"
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
