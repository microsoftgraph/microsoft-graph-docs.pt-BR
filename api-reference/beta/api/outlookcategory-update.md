---
title: Atualizar a categoria do Outlook
description: 'Atualize a propriedade gravável, **color**, do objeto outlookCategory especificado. Você não pode modificar a propriedade **displayName** '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: f6440708f7083e0b129e48aa0f455b892fd4d157
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965093"
---
# <a name="update-outlook-category"></a><span data-ttu-id="1dfdf-104">Atualizar a categoria do Outlook</span><span class="sxs-lookup"><span data-stu-id="1dfdf-104">Update Outlook category</span></span>

> <span data-ttu-id="1dfdf-105">**Importante**: APIs sob a versão /beta no Microsoft Graph estiver em Visualizar e estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="1dfdf-105">**Important**: APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1dfdf-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1dfdf-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1dfdf-107">Atualize a propriedade gravável, **color**, do objeto [outlookCategory](../resources/outlookcategory.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="1dfdf-107">Update the writable property, **color**, of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span> <span data-ttu-id="1dfdf-108">Não é possível modificar a propriedade **displayName** depois de criar a categoria.</span><span class="sxs-lookup"><span data-stu-id="1dfdf-108">You cannot modify the **displayName** property once you have created the category.</span></span>

## <a name="permissions"></a><span data-ttu-id="1dfdf-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="1dfdf-109">Permissions</span></span>
<span data-ttu-id="1dfdf-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1dfdf-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dfdf-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1dfdf-112">Permission type</span></span>      | <span data-ttu-id="1dfdf-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1dfdf-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1dfdf-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1dfdf-114">Delegated (work or school account)</span></span> | <span data-ttu-id="1dfdf-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1dfdf-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="1dfdf-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1dfdf-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1dfdf-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1dfdf-117">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="1dfdf-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1dfdf-118">Application</span></span> | <span data-ttu-id="1dfdf-119">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1dfdf-119">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1dfdf-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1dfdf-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/masterCategories/{id}
PATCH /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1dfdf-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1dfdf-121">Request headers</span></span>
| <span data-ttu-id="1dfdf-122">Nome</span><span class="sxs-lookup"><span data-stu-id="1dfdf-122">Name</span></span>      |<span data-ttu-id="1dfdf-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1dfdf-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1dfdf-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1dfdf-124">Authorization</span></span>  | <span data-ttu-id="1dfdf-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1dfdf-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1dfdf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1dfdf-127">Request body</span></span>
<span data-ttu-id="1dfdf-p106">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="1dfdf-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1dfdf-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1dfdf-131">Property</span></span>     | <span data-ttu-id="1dfdf-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="1dfdf-132">Type</span></span>   |<span data-ttu-id="1dfdf-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="1dfdf-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1dfdf-134">color</span><span class="sxs-lookup"><span data-stu-id="1dfdf-134">color</span></span>|<span data-ttu-id="1dfdf-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1dfdf-135">String</span></span>|<span data-ttu-id="1dfdf-136">Uma constante de cor predefinida que caracteriza uma categoria e que é mapeada para uma das 25 cores predefinidas.</span><span class="sxs-lookup"><span data-stu-id="1dfdf-136">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> |

## <a name="response"></a><span data-ttu-id="1dfdf-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dfdf-137">Response</span></span>

<span data-ttu-id="1dfdf-138">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [outlookCategory](../resources/outlookcategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1dfdf-138">If successful, this method returns a `200 OK` response code and updated [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1dfdf-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1dfdf-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1dfdf-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1dfdf-140">Request</span></span>
<span data-ttu-id="1dfdf-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1dfdf-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_outlookcategory"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/outlook/masterCategories('bac262b7-485d-4739-b436-e31467d64fac')
Content-type: application/json
Content-length: 30

{
  "color":"preset15"
}
```
##### <a name="response"></a><span data-ttu-id="1dfdf-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dfdf-142">Response</span></span>
<span data-ttu-id="1dfdf-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1dfdf-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
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
