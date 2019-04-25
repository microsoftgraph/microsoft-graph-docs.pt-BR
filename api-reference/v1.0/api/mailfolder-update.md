---
title: Atualizar mailfolder
description: Atualize as propriedades do objeto mailfolder.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 849b5e99f96b3ca891ef719e6ae45e8a2bcdd372
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561415"
---
# <a name="update-mailfolder"></a><span data-ttu-id="683da-103">Atualizar mailfolder</span><span class="sxs-lookup"><span data-stu-id="683da-103">Update mailfolder</span></span>

<span data-ttu-id="683da-104">Atualize as propriedades do objeto mailfolder.</span><span class="sxs-lookup"><span data-stu-id="683da-104">Update the properties of mailfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="683da-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="683da-105">Permissions</span></span>
<span data-ttu-id="683da-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="683da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="683da-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="683da-108">Permission type</span></span>      | <span data-ttu-id="683da-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="683da-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="683da-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="683da-110">Delegated (work or school account)</span></span> | <span data-ttu-id="683da-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="683da-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="683da-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="683da-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="683da-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="683da-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="683da-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="683da-114">Application</span></span> | <span data-ttu-id="683da-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="683da-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="683da-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="683da-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="683da-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="683da-117">Request headers</span></span>
| <span data-ttu-id="683da-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="683da-118">Header</span></span>       | <span data-ttu-id="683da-119">Valor</span><span class="sxs-lookup"><span data-stu-id="683da-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="683da-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="683da-120">Authorization</span></span>  | <span data-ttu-id="683da-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="683da-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="683da-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="683da-123">Content-Type</span></span>  | <span data-ttu-id="683da-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="683da-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="683da-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="683da-126">Request body</span></span>
<span data-ttu-id="683da-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="683da-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="683da-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="683da-130">Property</span></span>     | <span data-ttu-id="683da-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="683da-131">Type</span></span>   |<span data-ttu-id="683da-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="683da-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="683da-133">displayName</span><span class="sxs-lookup"><span data-stu-id="683da-133">displayName</span></span>|<span data-ttu-id="683da-134">String</span><span class="sxs-lookup"><span data-stu-id="683da-134">String</span></span>|<span data-ttu-id="683da-135">O nome de exibição da mailFolder.</span><span class="sxs-lookup"><span data-stu-id="683da-135">The mailFolder's display name.</span></span>|

## <a name="response"></a><span data-ttu-id="683da-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="683da-136">Response</span></span>

<span data-ttu-id="683da-137">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [mailFolder](../resources/mailfolder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="683da-137">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="683da-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="683da-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="683da-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="683da-139">Request</span></span>
<span data-ttu-id="683da-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="683da-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_mailfolder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailFolders/{id}
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```
##### <a name="response"></a><span data-ttu-id="683da-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="683da-141">Response</span></span>
<span data-ttu-id="683da-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="683da-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
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
