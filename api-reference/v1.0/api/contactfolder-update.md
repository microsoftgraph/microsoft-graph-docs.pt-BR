---
title: Atualizar contactfolder
description: Atualizar as propriedades do objeto contactfolder.
author: angelgolfer-ms
ms.openlocfilehash: 1bed74aa9efd6f8d82677d3c50feedc03fa34fe3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310714"
---
# <a name="update-contactfolder"></a><span data-ttu-id="0cce2-103">Atualizar contactfolder</span><span class="sxs-lookup"><span data-stu-id="0cce2-103">Update contactfolder</span></span>

<span data-ttu-id="0cce2-104">Atualizar as propriedades do objeto contactfolder.</span><span class="sxs-lookup"><span data-stu-id="0cce2-104">Update the properties of contactfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0cce2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0cce2-105">Permissions</span></span>
<span data-ttu-id="0cce2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cce2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cce2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0cce2-108">Permission type</span></span>      | <span data-ttu-id="0cce2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0cce2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0cce2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0cce2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0cce2-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0cce2-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0cce2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0cce2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0cce2-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0cce2-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0cce2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0cce2-114">Application</span></span> | <span data-ttu-id="0cce2-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0cce2-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0cce2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0cce2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/contactFolders/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0cce2-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0cce2-117">Request headers</span></span>
| <span data-ttu-id="0cce2-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0cce2-118">Header</span></span>       | <span data-ttu-id="0cce2-119">Valor</span><span class="sxs-lookup"><span data-stu-id="0cce2-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0cce2-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="0cce2-120">Authorization</span></span>  | <span data-ttu-id="0cce2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0cce2-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0cce2-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0cce2-123">Content-Type</span></span>  | <span data-ttu-id="0cce2-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0cce2-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0cce2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0cce2-126">Request body</span></span>
<span data-ttu-id="0cce2-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="0cce2-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0cce2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0cce2-130">Property</span></span>     | <span data-ttu-id="0cce2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0cce2-131">Type</span></span>   |<span data-ttu-id="0cce2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cce2-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0cce2-133">displayName</span><span class="sxs-lookup"><span data-stu-id="0cce2-133">displayName</span></span>|<span data-ttu-id="0cce2-134">String</span><span class="sxs-lookup"><span data-stu-id="0cce2-134">String</span></span>|<span data-ttu-id="0cce2-135">O nome de exibição da pasta.</span><span class="sxs-lookup"><span data-stu-id="0cce2-135">The folder's display name.</span></span>|
|<span data-ttu-id="0cce2-136">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="0cce2-136">parentFolderId</span></span>|<span data-ttu-id="0cce2-137">String</span><span class="sxs-lookup"><span data-stu-id="0cce2-137">String</span></span>|<span data-ttu-id="0cce2-138">A ID da pasta pai da pasta.</span><span class="sxs-lookup"><span data-stu-id="0cce2-138">The ID of the folder's parent folder.</span></span>|

## <a name="response"></a><span data-ttu-id="0cce2-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cce2-139">Response</span></span>

<span data-ttu-id="0cce2-140">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [contactFolder](../resources/contactfolder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0cce2-140">If successful, this method returns a `200 OK` response code and updated [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0cce2-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0cce2-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0cce2-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0cce2-142">Request</span></span>
<span data-ttu-id="0cce2-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0cce2-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_contactfolder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/contactFolders/{id}
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
##### <a name="response"></a><span data-ttu-id="0cce2-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cce2-144">Response</span></span>
<span data-ttu-id="0cce2-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0cce2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 104

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update contactfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
