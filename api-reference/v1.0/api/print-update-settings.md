---
title: Atualizar printSettings
description: Atualize as configurações de todo o locatário para o serviço de Impressão Universal.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: cc1af332871ef5d527bff235ef25906c4a739540
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516877"
---
# <a name="update-printsettings"></a><span data-ttu-id="e8576-103">Atualizar printSettings</span><span class="sxs-lookup"><span data-stu-id="e8576-103">Update printSettings</span></span>
<span data-ttu-id="e8576-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8576-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="e8576-105">Atualize as configurações de todo o locatário para o serviço de Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="e8576-105">Update tenant-wide settings for the Universal Print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8576-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8576-106">Permissions</span></span>
<span data-ttu-id="e8576-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8576-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e8576-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="e8576-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="e8576-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="e8576-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="e8576-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8576-111">Permission type</span></span> | <span data-ttu-id="e8576-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8576-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e8576-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8576-113">Delegated (work or school account)</span></span>| <span data-ttu-id="e8576-114">PrintSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8576-114">PrintSettings.ReadWrite.All</span></span> |
|<span data-ttu-id="e8576-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8576-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8576-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8576-116">Not Supported.</span></span>|
|<span data-ttu-id="e8576-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8576-117">Application</span></span>|<span data-ttu-id="e8576-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8576-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8576-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8576-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/settings
```

## <a name="request-headers"></a><span data-ttu-id="e8576-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8576-120">Request headers</span></span>
|<span data-ttu-id="e8576-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e8576-121">Name</span></span>|<span data-ttu-id="e8576-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8576-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e8576-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8576-123">Authorization</span></span>|<span data-ttu-id="e8576-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8576-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e8576-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e8576-126">Content-Type</span></span>|<span data-ttu-id="e8576-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8576-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8576-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8576-129">Request body</span></span>
<span data-ttu-id="e8576-130">No corpo da solicitação, fornece os valores dos campos [printSettings relevantes](../resources/printsettings.md) que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="e8576-130">In the request body, supply the values for the relevant [printSettings](../resources/printsettings.md) fields that should be updated.</span></span> <span data-ttu-id="e8576-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="e8576-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e8576-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="e8576-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e8576-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8576-133">Property</span></span>     | <span data-ttu-id="e8576-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8576-134">Type</span></span>        | <span data-ttu-id="e8576-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8576-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e8576-136">documentConversionEnabled</span><span class="sxs-lookup"><span data-stu-id="e8576-136">documentConversionEnabled</span></span>|<span data-ttu-id="e8576-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="e8576-137">Boolean</span></span>|<span data-ttu-id="e8576-138">Especifica se a conversão de documento está habilitada para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e8576-138">Specifies whether document conversion is enabled for the tenant.</span></span> <span data-ttu-id="e8576-139">Se a conversão de documento estiver habilitada, o serviço de Impressão Universal converterá automaticamente documentos em um formato compatível com a impressora (por exemplo, XPS em PDF) quando necessário.</span><span class="sxs-lookup"><span data-stu-id="e8576-139">If document conversion is enabled, Universal Print service will automatically convert documents into a format compatible with the printer (for example, XPS to PDF) when needed.</span></span>|

## <a name="response"></a><span data-ttu-id="e8576-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8576-140">Response</span></span>

<span data-ttu-id="e8576-141">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta vazio.</span><span class="sxs-lookup"><span data-stu-id="e8576-141">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e8576-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e8576-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e8576-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8576-143">Request</span></span>
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

### <a name="response"></a><span data-ttu-id="e8576-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8576-144">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printSettings"
}
-->
``` http
HTTP/1.1 204 No Content
```

