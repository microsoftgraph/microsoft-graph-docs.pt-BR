---
title: Atualizar uma configuração de diretório
description: Atualiza as propriedades de um objeto de configuração de diretório específico.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5d17abb40c6cf020b23be4fc0c319ebdee2684aa
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33590254"
---
# <a name="update-a-directory-setting"></a><span data-ttu-id="0663f-103">Atualizar uma configuração de diretório</span><span class="sxs-lookup"><span data-stu-id="0663f-103">Update a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0663f-104">Atualiza as propriedades de um objeto de configuração de diretório específico.</span><span class="sxs-lookup"><span data-stu-id="0663f-104">Update the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="0663f-105">**Observação**: a versão do/beta dessa API só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="0663f-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="0663f-106">A versão/v1.0 dessa API foi renomeada para atualizar o *groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="0663f-106">The /v1.0 version of this API has been renamed to *Update groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="0663f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="0663f-107">Permissions</span></span>
<span data-ttu-id="0663f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0663f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0663f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0663f-110">Permission type</span></span>      | <span data-ttu-id="0663f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0663f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0663f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0663f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0663f-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0663f-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0663f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0663f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0663f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0663f-115">Not supported.</span></span>    |
|<span data-ttu-id="0663f-116">Application</span><span class="sxs-lookup"><span data-stu-id="0663f-116">Application</span></span> | <span data-ttu-id="0663f-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0663f-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0663f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0663f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="0663f-119">Atualizar uma configuração específica de grupo ou de locatário como um todo.</span><span class="sxs-lookup"><span data-stu-id="0663f-119">Update a tenant-wide or group specific setting.</span></span>
```http
PATCH /settings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="0663f-120">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="0663f-120">Optional request headers</span></span>
| <span data-ttu-id="0663f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0663f-121">Name</span></span>       | <span data-ttu-id="0663f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0663f-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0663f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0663f-123">Authorization</span></span>  | <span data-ttu-id="0663f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0663f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0663f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0663f-126">Request body</span></span>
<span data-ttu-id="0663f-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="0663f-127">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="0663f-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0663f-128">Property</span></span>     | <span data-ttu-id="0663f-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="0663f-129">Type</span></span>   |<span data-ttu-id="0663f-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="0663f-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0663f-131">values</span><span class="sxs-lookup"><span data-stu-id="0663f-131">values</span></span> | <span data-ttu-id="0663f-132">[](../resources/settingvalue.md) coleção SettingValue</span><span class="sxs-lookup"><span data-stu-id="0663f-132">[settingValue](../resources/settingvalue.md) collection</span></span> | <span data-ttu-id="0663f-p104">O conjunto atualizado de valores.  OBSERVAÇÃO: Você deve fornecer o conjunto inteiro. Você não pode atualizar um único conjunto de valores.</span><span class="sxs-lookup"><span data-stu-id="0663f-p104">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="0663f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0663f-136">Response</span></span>

<span data-ttu-id="0663f-137">Se tiver êxito, este método retornará um código de resposta `204 OK`.</span><span class="sxs-lookup"><span data-stu-id="0663f-137">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0663f-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0663f-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0663f-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0663f-139">Request</span></span>
<span data-ttu-id="0663f-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0663f-140">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="0663f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="0663f-141">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorysetting"
} -->
```http
HTTP/1.1 204 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0663f-142">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="0663f-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0663f-143">Basic</span><span class="sxs-lookup"><span data-stu-id="0663f-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_directorysetting-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0663f-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0663f-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_directorysetting-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/directorysetting-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directorysetting-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
