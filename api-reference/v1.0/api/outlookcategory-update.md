---
title: Atualizar a categoria do Outlook
description: 'Atualize a propriedade gravável, **color**, do objeto outlookCategory especificado. Você não pode modificar a propriedade **displayName** '
ms.openlocfilehash: 1b664ef4414a798fe3f8ee2cd517a75f96ff3dc6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007267"
---
# <a name="update-outlook-category"></a><span data-ttu-id="637ce-104">Atualizar a categoria do Outlook</span><span class="sxs-lookup"><span data-stu-id="637ce-104">Update Outlook category</span></span>


<span data-ttu-id="637ce-105">Atualize a propriedade gravável, **color**, do objeto [outlookCategory](../resources/outlookcategory.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="637ce-105">Update the writable property, **color**, of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span> <span data-ttu-id="637ce-106">Não é possível modificar a propriedade **displayName** depois de criar a categoria.</span><span class="sxs-lookup"><span data-stu-id="637ce-106">You cannot modify the **displayName** property once you have created the category.</span></span>

## <a name="permissions"></a><span data-ttu-id="637ce-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="637ce-107">Permissions</span></span>
<span data-ttu-id="637ce-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="637ce-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="637ce-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="637ce-110">Permission type</span></span>      | <span data-ttu-id="637ce-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="637ce-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="637ce-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="637ce-112">Delegated (work or school account)</span></span> | <span data-ttu-id="637ce-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="637ce-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="637ce-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="637ce-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="637ce-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="637ce-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="637ce-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="637ce-116">Application</span></span> | <span data-ttu-id="637ce-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="637ce-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="637ce-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="637ce-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/masterCategories/{id}
PATCH /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="637ce-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="637ce-119">Optional query parameters</span></span>
<span data-ttu-id="637ce-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="637ce-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="637ce-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="637ce-121">Request headers</span></span>
| <span data-ttu-id="637ce-122">Nome</span><span class="sxs-lookup"><span data-stu-id="637ce-122">Name</span></span>      |<span data-ttu-id="637ce-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="637ce-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="637ce-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="637ce-124">Authorization</span></span>  | <span data-ttu-id="637ce-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="637ce-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="637ce-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="637ce-127">Request body</span></span>
<span data-ttu-id="637ce-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="637ce-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="637ce-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="637ce-131">Property</span></span>     | <span data-ttu-id="637ce-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="637ce-132">Type</span></span>   |<span data-ttu-id="637ce-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="637ce-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="637ce-134">color</span><span class="sxs-lookup"><span data-stu-id="637ce-134">color</span></span>|<span data-ttu-id="637ce-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="637ce-135">String</span></span>|<span data-ttu-id="637ce-136">Uma constante de cor predefinida que caracteriza uma categoria e que é mapeada para uma das 25 cores predefinidas.</span><span class="sxs-lookup"><span data-stu-id="637ce-136">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> |

## <a name="response"></a><span data-ttu-id="637ce-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="637ce-137">Response</span></span>

<span data-ttu-id="637ce-138">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [outlookCategory](../resources/outlookcategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="637ce-138">If successful, this method returns a `200 OK` response code and updated [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="637ce-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="637ce-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="637ce-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="637ce-140">Request</span></span>
<span data-ttu-id="637ce-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="637ce-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["bac262b7-485d-4739-b436-e31467d64fac"],
  "name": "update_outlookcategory"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/outlook/masterCategories/bac262b7-485d-4739-b436-e31467d64fac
Content-type: application/json
Content-length: 30

{
  "color":"preset15"
}
```
##### <a name="response"></a><span data-ttu-id="637ce-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="637ce-142">Response</span></span>
<span data-ttu-id="637ce-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="637ce-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"bac262b7-485d-4739-b436-e31467d64fac",
  "displayName":"Project expenses",
  "color":"preset15"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->