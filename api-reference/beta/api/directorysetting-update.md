---
title: Atualizar uma configuração de diretório
description: Atualize as propriedades de um objeto de configuração do diretório específico.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: baaf6994f7052155173dd58b2c6b021939dc7ba7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529093"
---
# <a name="update-a-directory-setting"></a><span data-ttu-id="dc1ba-103">Atualizar uma configuração de diretório</span><span class="sxs-lookup"><span data-stu-id="dc1ba-103">Update a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc1ba-104">Atualize as propriedades de um objeto de configuração do diretório específico.</span><span class="sxs-lookup"><span data-stu-id="dc1ba-104">Update the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="dc1ba-105">**Observação**: A versão de /beta desse API é só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="dc1ba-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="dc1ba-106">A versão de /v1.0 desse API foi renomeada para *Atualizar groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="dc1ba-106">The /v1.0 version of this API has been renamed to *Update groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc1ba-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="dc1ba-107">Permissions</span></span>
<span data-ttu-id="dc1ba-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc1ba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc1ba-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc1ba-110">Permission type</span></span>      | <span data-ttu-id="dc1ba-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dc1ba-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc1ba-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc1ba-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dc1ba-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dc1ba-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dc1ba-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc1ba-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc1ba-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc1ba-115">Not supported.</span></span>    |
|<span data-ttu-id="dc1ba-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc1ba-116">Application</span></span> | <span data-ttu-id="dc1ba-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc1ba-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc1ba-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc1ba-118">HTTP request</span></span>
<span data-ttu-id="dc1ba-119"><!-- { "blockType": "ignored" } -->Atualize a todo um locatário ou configuração específica de grupo.</span><span class="sxs-lookup"><span data-stu-id="dc1ba-119"><!-- { "blockType": "ignored" } --> Update a tenant-wide or group specific setting.</span></span>
```http
PATCH /settings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="dc1ba-120">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="dc1ba-120">Optional request headers</span></span>
| <span data-ttu-id="dc1ba-121">Nome</span><span class="sxs-lookup"><span data-stu-id="dc1ba-121">Name</span></span>       | <span data-ttu-id="dc1ba-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc1ba-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="dc1ba-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc1ba-123">Authorization</span></span>  | <span data-ttu-id="dc1ba-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc1ba-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc1ba-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc1ba-126">Request body</span></span>
<span data-ttu-id="dc1ba-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="dc1ba-127">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="dc1ba-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dc1ba-128">Property</span></span>     | <span data-ttu-id="dc1ba-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc1ba-129">Type</span></span>   |<span data-ttu-id="dc1ba-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc1ba-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dc1ba-131">values</span><span class="sxs-lookup"><span data-stu-id="dc1ba-131">values</span></span> | <span data-ttu-id="dc1ba-132">settingValue</span><span class="sxs-lookup"><span data-stu-id="dc1ba-132">settingValue</span></span> | <span data-ttu-id="dc1ba-p104">O conjunto atualizado de valores.  OBSERVAÇÃO: Você deve fornecer o conjunto inteiro. Você não pode atualizar um único conjunto de valores.</span><span class="sxs-lookup"><span data-stu-id="dc1ba-p104">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="dc1ba-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc1ba-136">Response</span></span>

<span data-ttu-id="dc1ba-137">Se tiver êxito, este método retornará um código de resposta `204 OK`.</span><span class="sxs-lookup"><span data-stu-id="dc1ba-137">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="dc1ba-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dc1ba-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dc1ba-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc1ba-139">Request</span></span>
<span data-ttu-id="dc1ba-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc1ba-140">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="dc1ba-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc1ba-141">Response</span></span>
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
