---
title: Atualizar uma configuração de diretório
description: Atualiza as propriedades de um objeto de configuração de diretório específico.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1337527b7be6c8cc7f2b52f37a1698d61fa9b842
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454796"
---
# <a name="update-a-directory-setting"></a><span data-ttu-id="a78bb-103">Atualizar uma configuração de diretório</span><span class="sxs-lookup"><span data-stu-id="a78bb-103">Update a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a78bb-104">Atualiza as propriedades de um objeto de configuração de diretório específico.</span><span class="sxs-lookup"><span data-stu-id="a78bb-104">Update the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="a78bb-105">**Observação**: a versão do/beta dessa API só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="a78bb-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="a78bb-106">A versão/v1.0 dessa API foi renomeada para atualizar o *groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="a78bb-106">The /v1.0 version of this API has been renamed to *Update groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="a78bb-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a78bb-107">Permissions</span></span>
<span data-ttu-id="a78bb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a78bb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a78bb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a78bb-110">Permission type</span></span>      | <span data-ttu-id="a78bb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a78bb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a78bb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a78bb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a78bb-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a78bb-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a78bb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a78bb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a78bb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a78bb-115">Not supported.</span></span>    |
|<span data-ttu-id="a78bb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a78bb-116">Application</span></span> | <span data-ttu-id="a78bb-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a78bb-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a78bb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a78bb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="a78bb-119">Atualizar uma configuração específica de grupo ou de locatário como um todo.</span><span class="sxs-lookup"><span data-stu-id="a78bb-119">Update a tenant-wide or group specific setting.</span></span>
```http
PATCH /settings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="a78bb-120">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="a78bb-120">Optional request headers</span></span>
| <span data-ttu-id="a78bb-121">Name</span><span class="sxs-lookup"><span data-stu-id="a78bb-121">Name</span></span>       | <span data-ttu-id="a78bb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a78bb-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a78bb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a78bb-123">Authorization</span></span>  | <span data-ttu-id="a78bb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a78bb-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a78bb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a78bb-126">Request body</span></span>
<span data-ttu-id="a78bb-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="a78bb-127">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="a78bb-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a78bb-128">Property</span></span>     | <span data-ttu-id="a78bb-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="a78bb-129">Type</span></span>   |<span data-ttu-id="a78bb-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="a78bb-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a78bb-131">values</span><span class="sxs-lookup"><span data-stu-id="a78bb-131">values</span></span> | <span data-ttu-id="a78bb-132">[](../resources/settingvalue.md) coleção SettingValue</span><span class="sxs-lookup"><span data-stu-id="a78bb-132">[settingValue](../resources/settingvalue.md) collection</span></span> | <span data-ttu-id="a78bb-p104">O conjunto atualizado de valores.  OBSERVAÇÃO: Você deve fornecer o conjunto inteiro. Você não pode atualizar um único conjunto de valores.</span><span class="sxs-lookup"><span data-stu-id="a78bb-p104">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="a78bb-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a78bb-136">Response</span></span>

<span data-ttu-id="a78bb-137">Se tiver êxito, este método retornará um código de resposta `204 OK`.</span><span class="sxs-lookup"><span data-stu-id="a78bb-137">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a78bb-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a78bb-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a78bb-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a78bb-139">Request</span></span>
<span data-ttu-id="a78bb-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a78bb-140">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="a78bb-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="a78bb-141">Response</span></span>
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
    "Error: /api-reference/beta/api/directorysetting-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
