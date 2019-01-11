---
title: Atualizar mailFolder
description: Atualize as propriedades do objeto mailFolder.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: f9b0af67b4fdedbf6ecbbcfe591057a4aeb86351
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873893"
---
# <a name="update-mailfolder"></a><span data-ttu-id="9f168-103">Atualizar mailFolder</span><span class="sxs-lookup"><span data-stu-id="9f168-103">Update mailFolder</span></span>

> <span data-ttu-id="9f168-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9f168-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f168-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9f168-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9f168-106">Atualize as propriedades do objeto [mailFolder](../resources/mailfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="9f168-106">Update the properties of [mailFolder](../resources/mailfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f168-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="9f168-107">Permissions</span></span>
<span data-ttu-id="9f168-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f168-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f168-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f168-110">Permission type</span></span>      | <span data-ttu-id="9f168-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9f168-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f168-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f168-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9f168-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f168-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9f168-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9f168-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f168-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f168-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9f168-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9f168-116">Application</span></span> | <span data-ttu-id="9f168-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f168-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f168-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f168-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9f168-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f168-119">Request headers</span></span>
| <span data-ttu-id="9f168-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9f168-120">Header</span></span>       | <span data-ttu-id="9f168-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9f168-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9f168-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9f168-122">Authorization</span></span>  | <span data-ttu-id="9f168-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f168-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9f168-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9f168-125">Content-Type</span></span>  | <span data-ttu-id="9f168-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f168-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9f168-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9f168-128">Request body</span></span>
<span data-ttu-id="9f168-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="9f168-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9f168-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9f168-132">Property</span></span>     | <span data-ttu-id="9f168-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f168-133">Type</span></span>   |<span data-ttu-id="9f168-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f168-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f168-135">displayName</span><span class="sxs-lookup"><span data-stu-id="9f168-135">displayName</span></span>|<span data-ttu-id="9f168-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f168-136">String</span></span>|<span data-ttu-id="9f168-137">O nome de exibição da mailFolder.</span><span class="sxs-lookup"><span data-stu-id="9f168-137">The mailFolder's display name.</span></span>|

## <a name="response"></a><span data-ttu-id="9f168-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f168-138">Response</span></span>
<span data-ttu-id="9f168-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [mailFolder](../resources/mailfolder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9f168-139">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f168-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9f168-140">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9f168-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f168-141">Request</span></span>
<span data-ttu-id="9f168-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9f168-142">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_mailfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```

#### <a name="response"></a><span data-ttu-id="9f168-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f168-143">Response</span></span>
<span data-ttu-id="9f168-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9f168-144">The following is an example of the response.</span></span>
><span data-ttu-id="9f168-145">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9f168-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9f168-146">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9f168-146">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
    "id": "AAMkAGVmMDEzM",
    "displayName": "displayName-value",
    "parentFolderId": "AAMkAGVmMDEzI",
    "childFolderCount": 2,
    "unreadItemCount": 59,
    "totalItemCount": 60,
    "wellKnownName": "inbox"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update mailfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
