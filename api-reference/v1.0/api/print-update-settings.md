---
title: Atualizar printSettings
description: Atualize as configurações de todo o locatário para o serviço de Impressão Universal.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 2d68bed903409fcc20b333e95245e8e15764b348
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787611"
---
# <a name="update-printsettings"></a><span data-ttu-id="a5cbd-103">Atualizar printSettings</span><span class="sxs-lookup"><span data-stu-id="a5cbd-103">Update printSettings</span></span>
<span data-ttu-id="a5cbd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5cbd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="a5cbd-105">Atualize as configurações de todo o locatário para o serviço de Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="a5cbd-105">Update tenant-wide settings for the Universal Print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5cbd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a5cbd-106">Permissions</span></span>
<span data-ttu-id="a5cbd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5cbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a5cbd-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="a5cbd-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="a5cbd-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="a5cbd-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="a5cbd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5cbd-111">Permission type</span></span> | <span data-ttu-id="a5cbd-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a5cbd-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="a5cbd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5cbd-113">Delegated (work or school account)</span></span>| <span data-ttu-id="a5cbd-114">PrintSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5cbd-114">PrintSettings.ReadWrite.All</span></span> |
|<span data-ttu-id="a5cbd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5cbd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5cbd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5cbd-116">Not Supported.</span></span>|
|<span data-ttu-id="a5cbd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5cbd-117">Application</span></span>|<span data-ttu-id="a5cbd-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5cbd-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5cbd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5cbd-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/settings
```

## <a name="request-headers"></a><span data-ttu-id="a5cbd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5cbd-120">Request headers</span></span>
|<span data-ttu-id="a5cbd-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a5cbd-121">Name</span></span>|<span data-ttu-id="a5cbd-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5cbd-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a5cbd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5cbd-123">Authorization</span></span>|<span data-ttu-id="a5cbd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5cbd-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a5cbd-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a5cbd-126">Content-Type</span></span>|<span data-ttu-id="a5cbd-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5cbd-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5cbd-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5cbd-129">Request body</span></span>
<span data-ttu-id="a5cbd-130">No corpo da solicitação, fornece os valores dos campos [printSettings relevantes](../resources/printsettings.md) que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="a5cbd-130">In the request body, supply the values for the relevant [printSettings](../resources/printsettings.md) fields that should be updated.</span></span> <span data-ttu-id="a5cbd-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="a5cbd-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a5cbd-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="a5cbd-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a5cbd-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a5cbd-133">Property</span></span>     | <span data-ttu-id="a5cbd-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5cbd-134">Type</span></span>        | <span data-ttu-id="a5cbd-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5cbd-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a5cbd-136">documentConversionEnabled</span><span class="sxs-lookup"><span data-stu-id="a5cbd-136">documentConversionEnabled</span></span>|<span data-ttu-id="a5cbd-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5cbd-137">Boolean</span></span>|<span data-ttu-id="a5cbd-138">Especifica se a conversão de documento está habilitada para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a5cbd-138">Specifies whether document conversion is enabled for the tenant.</span></span> <span data-ttu-id="a5cbd-139">Se a conversão de documento estiver habilitada, o serviço de Impressão Universal converterá automaticamente documentos em um formato compatível com a impressora (por exemplo, XPS em PDF) quando necessário.</span><span class="sxs-lookup"><span data-stu-id="a5cbd-139">If document conversion is enabled, Universal Print service will automatically convert documents into a format compatible with the printer (for example, XPS to PDF) when needed.</span></span>|

## <a name="response"></a><span data-ttu-id="a5cbd-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5cbd-140">Response</span></span>

<span data-ttu-id="a5cbd-141">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta vazio.</span><span class="sxs-lookup"><span data-stu-id="a5cbd-141">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a5cbd-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a5cbd-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a5cbd-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5cbd-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a5cbd-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5cbd-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_printsettings"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/print/settings
Content-type: application/json

{
  "documentConversionEnabled": true
}
```
# <a name="c"></a>[<span data-ttu-id="a5cbd-145">C#</span><span class="sxs-lookup"><span data-stu-id="a5cbd-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-printsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5cbd-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5cbd-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-printsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5cbd-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5cbd-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-printsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a5cbd-148">Java</span><span class="sxs-lookup"><span data-stu-id="a5cbd-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-printsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a5cbd-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5cbd-149">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

