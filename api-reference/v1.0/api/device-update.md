---
title: Atualizar dispositivo
description: Atualiza as propriedades de um dispositivo registrado.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2521530b8646eab3d2966ba42a101e13f774d97f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273287"
---
# <a name="update-device"></a><span data-ttu-id="35012-103">Atualizar dispositivo</span><span class="sxs-lookup"><span data-stu-id="35012-103">Update device</span></span>

<span data-ttu-id="35012-104">Atualiza as propriedades de um dispositivo registrado.</span><span class="sxs-lookup"><span data-stu-id="35012-104">Update the properties of a registered device.</span></span>

<span data-ttu-id="35012-105">Somente algumas propriedades de um dispositivo podem ser atualizadas por meio de aplicativos de gerenciamento de dispositivo móvel aprovados(MDM).</span><span class="sxs-lookup"><span data-stu-id="35012-105">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="35012-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="35012-106">Permissions</span></span>
<span data-ttu-id="35012-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35012-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35012-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="35012-109">Permission type</span></span>      | <span data-ttu-id="35012-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="35012-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35012-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="35012-111">Delegated (work or school account)</span></span> | <span data-ttu-id="35012-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="35012-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="35012-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="35012-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35012-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35012-114">Not supported.</span></span> |
|<span data-ttu-id="35012-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="35012-115">Application</span></span> | <span data-ttu-id="35012-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="35012-116">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="35012-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="35012-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```
> <span data-ttu-id="35012-118">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="35012-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="35012-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="35012-119">Request headers</span></span>
| <span data-ttu-id="35012-120">Nome</span><span class="sxs-lookup"><span data-stu-id="35012-120">Name</span></span>       | <span data-ttu-id="35012-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="35012-121">Type</span></span> | <span data-ttu-id="35012-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="35012-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="35012-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="35012-123">Authorization</span></span>  | <span data-ttu-id="35012-124">string</span><span class="sxs-lookup"><span data-stu-id="35012-124">string</span></span>  | <span data-ttu-id="35012-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35012-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="35012-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="35012-127">Request body</span></span>

<span data-ttu-id="35012-128">No corpo da solicitação, forneça os valores para as propriedades [device](../resources/device.md) que devem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="35012-128">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="35012-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="35012-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="35012-130">Para obter um melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="35012-130">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="35012-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35012-131">Property</span></span>     | <span data-ttu-id="35012-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="35012-132">Type</span></span>   |<span data-ttu-id="35012-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="35012-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35012-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="35012-134">accountEnabled</span></span>|<span data-ttu-id="35012-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="35012-135">Boolean</span></span>| <span data-ttu-id="35012-136">**true** se a conta estiver habilitada; caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="35012-136">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="35012-137">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="35012-137">operatingSystem</span></span>|<span data-ttu-id="35012-138">String</span><span class="sxs-lookup"><span data-stu-id="35012-138">String</span></span>|<span data-ttu-id="35012-139">O tipo de sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="35012-139">The type of operating system on the device.</span></span>|
|<span data-ttu-id="35012-140">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="35012-140">operatingSystemVersion</span></span>|<span data-ttu-id="35012-141">String</span><span class="sxs-lookup"><span data-stu-id="35012-141">String</span></span>|<span data-ttu-id="35012-142">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="35012-142">The version of the operating system on the device</span></span>|
|<span data-ttu-id="35012-143">displayName</span><span class="sxs-lookup"><span data-stu-id="35012-143">displayName</span></span>|<span data-ttu-id="35012-144">String</span><span class="sxs-lookup"><span data-stu-id="35012-144">String</span></span>|<span data-ttu-id="35012-145">O nome de exibição do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="35012-145">The display name for the device.</span></span>|
|<span data-ttu-id="35012-146">isCompliant</span><span class="sxs-lookup"><span data-stu-id="35012-146">isCompliant</span></span>|<span data-ttu-id="35012-147">Booliano</span><span class="sxs-lookup"><span data-stu-id="35012-147">Boolean</span></span>|<span data-ttu-id="35012-148">**True** se o dispositivo está em conformidade com políticas de MDM (Gerenciamento de Dispositivo Móvel); caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="35012-148">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="35012-149">Isso só pode ser atualizado pelo Intune para qualquer tipo de sistema operacional do dispositivo ou por um [aplicativo MDM aprovado](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) para dispositivos do sistema operacional Windows.</span><span class="sxs-lookup"><span data-stu-id="35012-149">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="35012-150">isManaged</span><span class="sxs-lookup"><span data-stu-id="35012-150">isManaged</span></span>|<span data-ttu-id="35012-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="35012-151">Boolean</span></span>|<span data-ttu-id="35012-152">**true** se o dispositivo for gerenciado por um aplicativo de gerenciamento de dispositivo móvel (MDM); caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="35012-152">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="35012-153">Isso só pode ser atualizado pelo Intune para qualquer tipo de sistema operacional do dispositivo ou por um [aplicativo MDM aprovado](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) para dispositivos do sistema operacional Windows.</span><span class="sxs-lookup"><span data-stu-id="35012-153">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

## <a name="response"></a><span data-ttu-id="35012-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="35012-154">Response</span></span>

<span data-ttu-id="35012-155">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="35012-155">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="35012-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="35012-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="35012-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="35012-157">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_device"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/devices/{id}
Content-type: application/json
Content-length: 31

{
  "accountEnabled": false
}
```
##### <a name="response"></a><span data-ttu-id="35012-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="35012-158">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="35012-159">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="35012-159">SDK sample code</span></span>
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="35012-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="35012-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_device-Javascript-snippets.md)]

# <a name="ctabcs"></a>[<span data-ttu-id="35012-161">C#</span><span class="sxs-lookup"><span data-stu-id="35012-161">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_device-Cs-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="35012-162">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="35012-162">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_device-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/device-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/device-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/device-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
