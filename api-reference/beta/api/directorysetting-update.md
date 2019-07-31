---
title: Atualizar uma configuração de diretório
description: Atualiza as propriedades de um objeto de configuração de diretório específico.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0a3143c9d9893a759a1f2a81b93e46132ad0c949
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957553"
---
# <a name="update-a-directory-setting"></a><span data-ttu-id="02455-103">Atualizar uma configuração de diretório</span><span class="sxs-lookup"><span data-stu-id="02455-103">Update a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02455-104">Atualiza as propriedades de um objeto de configuração de diretório específico.</span><span class="sxs-lookup"><span data-stu-id="02455-104">Update the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="02455-105">**Observação**: a versão do/beta dessa API só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="02455-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="02455-106">A versão/v1.0 dessa API foi renomeada para atualizar o *groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="02455-106">The /v1.0 version of this API has been renamed to *Update groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="02455-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="02455-107">Permissions</span></span>
<span data-ttu-id="02455-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02455-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02455-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02455-110">Permission type</span></span>      | <span data-ttu-id="02455-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02455-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02455-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02455-112">Delegated (work or school account)</span></span> | <span data-ttu-id="02455-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="02455-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="02455-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02455-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02455-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02455-115">Not supported.</span></span>    |
|<span data-ttu-id="02455-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02455-116">Application</span></span> | <span data-ttu-id="02455-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02455-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="02455-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02455-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="02455-119">Atualizar uma configuração específica de grupo ou de locatário como um todo.</span><span class="sxs-lookup"><span data-stu-id="02455-119">Update a tenant-wide or group specific setting.</span></span>
```http
PATCH /settings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="02455-120">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="02455-120">Optional request headers</span></span>
| <span data-ttu-id="02455-121">Nome</span><span class="sxs-lookup"><span data-stu-id="02455-121">Name</span></span>       | <span data-ttu-id="02455-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="02455-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="02455-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="02455-123">Authorization</span></span>  | <span data-ttu-id="02455-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02455-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="02455-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02455-126">Request body</span></span>
<span data-ttu-id="02455-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="02455-127">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="02455-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02455-128">Property</span></span>     | <span data-ttu-id="02455-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="02455-129">Type</span></span>   |<span data-ttu-id="02455-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="02455-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="02455-131">values</span><span class="sxs-lookup"><span data-stu-id="02455-131">values</span></span> | <span data-ttu-id="02455-132">[](../resources/settingvalue.md) coleção SettingValue</span><span class="sxs-lookup"><span data-stu-id="02455-132">[settingValue](../resources/settingvalue.md) collection</span></span> | <span data-ttu-id="02455-p104">O conjunto atualizado de valores.  OBSERVAÇÃO: Você deve fornecer o conjunto inteiro. Você não pode atualizar um único conjunto de valores.</span><span class="sxs-lookup"><span data-stu-id="02455-p104">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="02455-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="02455-136">Response</span></span>

<span data-ttu-id="02455-137">Se tiver êxito, este método retornará um código de resposta `204 OK`.</span><span class="sxs-lookup"><span data-stu-id="02455-137">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="02455-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02455-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="02455-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02455-139">Request</span></span>
<span data-ttu-id="02455-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02455-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="02455-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="02455-141">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="02455-142">C#</span><span class="sxs-lookup"><span data-stu-id="02455-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-directorysetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="02455-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="02455-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-directorysetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="02455-144">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="02455-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-directorysetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="02455-145">Java</span><span class="sxs-lookup"><span data-stu-id="02455-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-directorysetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="02455-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="02455-146">Response</span></span>
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
