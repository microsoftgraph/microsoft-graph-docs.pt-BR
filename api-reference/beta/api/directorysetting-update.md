---
title: Atualizar uma configuração de diretório
description: Atualiza as propriedades de um objeto de configuração de diretório específico.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 65519a4bd4ae9e4640ec3d5b3abc604096bcd4b6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260533"
---
# <a name="update-a-directory-setting"></a><span data-ttu-id="15ed2-103">Atualizar uma configuração de diretório</span><span class="sxs-lookup"><span data-stu-id="15ed2-103">Update a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15ed2-104">Atualiza as propriedades de um objeto de configuração de diretório específico.</span><span class="sxs-lookup"><span data-stu-id="15ed2-104">Update the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="15ed2-105">**Observação**: a versão do/beta dessa API só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="15ed2-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="15ed2-106">A versão/v1.0 dessa API foi renomeada para atualizar o *groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="15ed2-106">The /v1.0 version of this API has been renamed to *Update groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="15ed2-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="15ed2-107">Permissions</span></span>
<span data-ttu-id="15ed2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15ed2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15ed2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15ed2-110">Permission type</span></span>      | <span data-ttu-id="15ed2-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="15ed2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15ed2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15ed2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="15ed2-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="15ed2-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="15ed2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15ed2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15ed2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15ed2-115">Not supported.</span></span>    |
|<span data-ttu-id="15ed2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15ed2-116">Application</span></span> | <span data-ttu-id="15ed2-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15ed2-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="15ed2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15ed2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="15ed2-119">Atualizar uma configuração específica de grupo ou de locatário como um todo.</span><span class="sxs-lookup"><span data-stu-id="15ed2-119">Update a tenant-wide or group specific setting.</span></span>
```http
PATCH /settings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="15ed2-120">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="15ed2-120">Optional request headers</span></span>
| <span data-ttu-id="15ed2-121">Nome</span><span class="sxs-lookup"><span data-stu-id="15ed2-121">Name</span></span>       | <span data-ttu-id="15ed2-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="15ed2-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="15ed2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="15ed2-123">Authorization</span></span>  | <span data-ttu-id="15ed2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15ed2-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="15ed2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15ed2-126">Request body</span></span>
<span data-ttu-id="15ed2-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="15ed2-127">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="15ed2-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="15ed2-128">Property</span></span>     | <span data-ttu-id="15ed2-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="15ed2-129">Type</span></span>   |<span data-ttu-id="15ed2-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="15ed2-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="15ed2-131">values</span><span class="sxs-lookup"><span data-stu-id="15ed2-131">values</span></span> | <span data-ttu-id="15ed2-132">[](../resources/settingvalue.md) coleção SettingValue</span><span class="sxs-lookup"><span data-stu-id="15ed2-132">[settingValue](../resources/settingvalue.md) collection</span></span> | <span data-ttu-id="15ed2-p104">O conjunto atualizado de valores.  OBSERVAÇÃO: Você deve fornecer o conjunto inteiro. Você não pode atualizar um único conjunto de valores.</span><span class="sxs-lookup"><span data-stu-id="15ed2-p104">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="15ed2-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="15ed2-136">Response</span></span>

<span data-ttu-id="15ed2-137">Se tiver êxito, este método retornará um código de resposta `204 OK`.</span><span class="sxs-lookup"><span data-stu-id="15ed2-137">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="15ed2-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15ed2-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="15ed2-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15ed2-139">Request</span></span>
<span data-ttu-id="15ed2-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="15ed2-140">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="15ed2-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="15ed2-141">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorysetting"
} -->
```http
HTTP/1.1 204 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="15ed2-142">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="15ed2-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="15ed2-143">C#</span><span class="sxs-lookup"><span data-stu-id="15ed2-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_directorysetting-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="15ed2-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="15ed2-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_directorysetting-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="15ed2-145">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="15ed2-145">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_directorysetting-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/directorysetting-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/directorysetting-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directorysetting-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
