---
title: Atualizar printSettings
description: Atualize as configurações de todo o locatário para o serviço de impressão universal.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 52e1c7a830da06309a8701df4bb0a6e2c14f4bb6
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313825"
---
# <a name="update-printsettings"></a><span data-ttu-id="1f425-103">Atualizar printSettings</span><span class="sxs-lookup"><span data-stu-id="1f425-103">Update printSettings</span></span>

<span data-ttu-id="1f425-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f425-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f425-105">Atualize as configurações de todo o locatário para o serviço de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="1f425-105">Update tenant-wide settings for the Universal Print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f425-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1f425-106">Permissions</span></span>
<span data-ttu-id="1f425-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f425-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="1f425-109">Para usar o serviço de impressão universal, o usuário ou o locatário do aplicativo deve ter uma assinatura de impressão universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="1f425-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="1f425-110">O usuário conectado deve ser um [administrador da impressora](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="1f425-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="1f425-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f425-111">Permission type</span></span> | <span data-ttu-id="1f425-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1f425-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="1f425-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f425-113">Delegated (work or school account)</span></span>| <span data-ttu-id="1f425-114">User.Read</span><span class="sxs-lookup"><span data-stu-id="1f425-114">User.Read</span></span> |
|<span data-ttu-id="1f425-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f425-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f425-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f425-116">Not Supported.</span></span>|
|<span data-ttu-id="1f425-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f425-117">Application</span></span>|<span data-ttu-id="1f425-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f425-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f425-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f425-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/settings
```

## <a name="optional-request-headers"></a><span data-ttu-id="1f425-120">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="1f425-120">Optional request headers</span></span>
| <span data-ttu-id="1f425-121">Nome</span><span class="sxs-lookup"><span data-stu-id="1f425-121">Name</span></span>       | <span data-ttu-id="1f425-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f425-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1f425-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f425-123">Authorization</span></span> | <span data-ttu-id="1f425-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f425-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1f425-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="1f425-126">Content-type</span></span>  | <span data-ttu-id="1f425-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f425-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f425-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f425-129">Request body</span></span>
<span data-ttu-id="1f425-130">No corpo da solicitação, forneça os valores para os campos de [configurações](../resources/printsettings.md) relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="1f425-130">In the request body, supply the values for the relevant [printSettings](../resources/printsettings.md) fields that should be updated.</span></span> <span data-ttu-id="1f425-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="1f425-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="1f425-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="1f425-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1f425-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1f425-133">Property</span></span>     | <span data-ttu-id="1f425-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f425-134">Type</span></span>        | <span data-ttu-id="1f425-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f425-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1f425-136">documentConversionEnabled</span><span class="sxs-lookup"><span data-stu-id="1f425-136">documentConversionEnabled</span></span>|<span data-ttu-id="1f425-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="1f425-137">Boolean</span></span>|<span data-ttu-id="1f425-138">Especifica se a conversão de documentos está habilitada para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1f425-138">Specifies whether document conversion is enabled for the tenant.</span></span> <span data-ttu-id="1f425-139">Se a conversão de documentos estiver habilitada, o serviço de impressão universal converterá automaticamente os documentos em um formato compatível com a impressora (por exemplo, XPS para PDF), quando necessário.</span><span class="sxs-lookup"><span data-stu-id="1f425-139">If document conversion is enabled, Universal Print service will automatically convert documents into a format compatible with the printer (for example, XPS to PDF) when needed.</span></span>|

## <a name="response"></a><span data-ttu-id="1f425-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f425-140">Response</span></span>
<span data-ttu-id="1f425-141">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta vazio.</span><span class="sxs-lookup"><span data-stu-id="1f425-141">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f425-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1f425-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1f425-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f425-143">Request</span></span>
<span data-ttu-id="1f425-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1f425-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1f425-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f425-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_settings"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/settings
Content-type: application/json

{
  "documentConversionEnabled": true
}
```
# <a name="c"></a>[<span data-ttu-id="1f425-146">C#</span><span class="sxs-lookup"><span data-stu-id="1f425-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f425-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f425-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f425-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f425-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1f425-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f425-149">Response</span></span>
<span data-ttu-id="1f425-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1f425-150">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printSettings"
} -->
```http
HTTP/1.1 204 NoContent
Content-length: 0
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->