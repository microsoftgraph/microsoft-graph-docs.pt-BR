---
title: Atualizar foto
description: Atualize as propriedades do objeto de foto.
ms.openlocfilehash: 8071c9e331f9af72c9a288239206f396d9ad3fcb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033418"
---
# <a name="update-photo"></a><span data-ttu-id="87289-103">Atualizar foto</span><span class="sxs-lookup"><span data-stu-id="87289-103">Update photo</span></span>

> <span data-ttu-id="87289-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="87289-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87289-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="87289-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="87289-106">Atualize as propriedades do objeto de foto.</span><span class="sxs-lookup"><span data-stu-id="87289-106">Update the properties of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="87289-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="87289-107">Permissions</span></span>
<span data-ttu-id="87289-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87289-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87289-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87289-110">Permission type</span></span>      | <span data-ttu-id="87289-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="87289-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87289-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87289-112">Delegated (work or school account)</span></span> | <span data-ttu-id="87289-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87289-113">Not supported.</span></span>    |
|<span data-ttu-id="87289-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87289-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87289-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87289-115">Not supported.</span></span>    |
|<span data-ttu-id="87289-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87289-116">Application</span></span> | <span data-ttu-id="87289-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87289-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="87289-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87289-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/photo
PATCH /groups/{id}/photo
PATCH /drive/root/createdByUser/photo
```

## <a name="request-headers"></a><span data-ttu-id="87289-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87289-119">Request headers</span></span>
| <span data-ttu-id="87289-120">Nome</span><span class="sxs-lookup"><span data-stu-id="87289-120">Name</span></span>       | <span data-ttu-id="87289-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="87289-121">Type</span></span> | <span data-ttu-id="87289-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="87289-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="87289-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="87289-123">Authorization</span></span>  | <span data-ttu-id="87289-124">string</span><span class="sxs-lookup"><span data-stu-id="87289-124">string</span></span>  | <span data-ttu-id="87289-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87289-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="87289-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87289-127">Request body</span></span>
<span data-ttu-id="87289-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="87289-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="87289-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87289-131">Property</span></span>     | <span data-ttu-id="87289-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="87289-132">Type</span></span>   |<span data-ttu-id="87289-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="87289-133">Description</span></span>|
|:---------------|:--------|:----------|

## <a name="response"></a><span data-ttu-id="87289-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="87289-134">Response</span></span>

<span data-ttu-id="87289-135">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [photo](../resources/photo.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87289-135">If successful, this method returns a `200 OK` response code and updated [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="87289-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87289-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="87289-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87289-137">Request</span></span>
<span data-ttu-id="87289-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="87289-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_photo"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```
##### <a name="response"></a><span data-ttu-id="87289-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="87289-139">Response</span></span>
<span data-ttu-id="87289-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87289-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
