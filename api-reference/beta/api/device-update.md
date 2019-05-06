---
title: Atualizar dispositivo
description: Atualizar as propriedades de um dispositivo.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6b7fd867545ad499378e76295795858e3b7d3da2
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33590732"
---
# <a name="update-device"></a><span data-ttu-id="089d2-103">Atualizar dispositivo</span><span class="sxs-lookup"><span data-stu-id="089d2-103">Update device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="089d2-104">Atualizar as propriedades de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="089d2-104">Update the properties of a device.</span></span>

<span data-ttu-id="089d2-105">Somente algumas propriedades de um dispositivo podem ser atualizadas por meio de aplicativos de gerenciamento de dispositivo móvel aprovados(MDM).</span><span class="sxs-lookup"><span data-stu-id="089d2-105">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="089d2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="089d2-106">Permissions</span></span>
<span data-ttu-id="089d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="089d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="089d2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="089d2-109">Permission type</span></span>      | <span data-ttu-id="089d2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="089d2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="089d2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="089d2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="089d2-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="089d2-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="089d2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="089d2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="089d2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="089d2-114">Not supported.</span></span> |
|<span data-ttu-id="089d2-115">Application</span><span class="sxs-lookup"><span data-stu-id="089d2-115">Application</span></span> | <span data-ttu-id="089d2-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="089d2-116">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="089d2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="089d2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```

> <span data-ttu-id="089d2-118">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="089d2-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="089d2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="089d2-119">Request headers</span></span>
| <span data-ttu-id="089d2-120">Nome</span><span class="sxs-lookup"><span data-stu-id="089d2-120">Name</span></span>       | <span data-ttu-id="089d2-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="089d2-121">Type</span></span> | <span data-ttu-id="089d2-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="089d2-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="089d2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="089d2-123">Authorization</span></span>  | <span data-ttu-id="089d2-124">string</span><span class="sxs-lookup"><span data-stu-id="089d2-124">string</span></span>  | <span data-ttu-id="089d2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="089d2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="089d2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="089d2-127">Request body</span></span>

<span data-ttu-id="089d2-128">No corpo da solicitação, forneça os valores para as propriedades [device](../resources/device.md) que devem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="089d2-128">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="089d2-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="089d2-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="089d2-130">Para obter um melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="089d2-130">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="089d2-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="089d2-131">Property</span></span>     | <span data-ttu-id="089d2-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="089d2-132">Type</span></span>   |<span data-ttu-id="089d2-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="089d2-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="089d2-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="089d2-134">accountEnabled</span></span>|<span data-ttu-id="089d2-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="089d2-135">Boolean</span></span>| <span data-ttu-id="089d2-136">**true** se a conta estiver habilitada; caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="089d2-136">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="089d2-137">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="089d2-137">operatingSystem</span></span>|<span data-ttu-id="089d2-138">String</span><span class="sxs-lookup"><span data-stu-id="089d2-138">String</span></span>|<span data-ttu-id="089d2-139">O tipo de sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="089d2-139">The type of operating system on the device.</span></span>|
|<span data-ttu-id="089d2-140">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="089d2-140">operatingSystemVersion</span></span>|<span data-ttu-id="089d2-141">String</span><span class="sxs-lookup"><span data-stu-id="089d2-141">String</span></span>|<span data-ttu-id="089d2-142">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="089d2-142">The version of the operating system on the device</span></span>|
|<span data-ttu-id="089d2-143">displayName</span><span class="sxs-lookup"><span data-stu-id="089d2-143">displayName</span></span>|<span data-ttu-id="089d2-144">String</span><span class="sxs-lookup"><span data-stu-id="089d2-144">String</span></span>|<span data-ttu-id="089d2-145">O nome de exibição do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="089d2-145">The display name for the device.</span></span>|
|<span data-ttu-id="089d2-146">isCompliant</span><span class="sxs-lookup"><span data-stu-id="089d2-146">isCompliant</span></span>|<span data-ttu-id="089d2-147">Booliano</span><span class="sxs-lookup"><span data-stu-id="089d2-147">Boolean</span></span>|<span data-ttu-id="089d2-148">**True** se o dispositivo está em conformidade com políticas de MDM (Gerenciamento de Dispositivo Móvel); caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="089d2-148">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="089d2-149">Isso só pode ser atualizado pelo Intune para qualquer tipo de sistema operacional do dispositivo ou por um [aplicativo MDM aprovado](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) para dispositivos do sistema operacional Windows.</span><span class="sxs-lookup"><span data-stu-id="089d2-149">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="089d2-150">isManaged</span><span class="sxs-lookup"><span data-stu-id="089d2-150">isManaged</span></span>|<span data-ttu-id="089d2-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="089d2-151">Boolean</span></span>|<span data-ttu-id="089d2-152">**true** se o dispositivo for gerenciado por um aplicativo de gerenciamento de dispositivo móvel (MDM); caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="089d2-152">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="089d2-153">Isso só pode ser atualizado pelo Intune para qualquer tipo de sistema operacional do dispositivo ou por um [aplicativo MDM aprovado](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) para dispositivos do sistema operacional Windows.</span><span class="sxs-lookup"><span data-stu-id="089d2-153">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

<span data-ttu-id="089d2-154">Como o recurso de **dispositivo** suporta [extensões](/graph/extensibility-overview), você pode usar `PATCH` a operação para adicionar, atualizar ou excluir seus próprios dados específicos de aplicativo em Propriedades personalizadas de uma extensão em uma instância de **dispositivo** existente.</span><span class="sxs-lookup"><span data-stu-id="089d2-154">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **device** instance.</span></span>

## <a name="response"></a><span data-ttu-id="089d2-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="089d2-155">Response</span></span>

<span data-ttu-id="089d2-156">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="089d2-156">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="089d2-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="089d2-157">Example</span></span>

##### <a name="request"></a><span data-ttu-id="089d2-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="089d2-158">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_device"
}-->
```http
PATCH https://graph.microsoft.com/beta/devices/{id}
Content-type: application/json
Content-length: 31

{
  "accountEnabled": false
}
```
##### <a name="response"></a><span data-ttu-id="089d2-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="089d2-159">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="089d2-160">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="089d2-160">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="089d2-161">Basic</span><span class="sxs-lookup"><span data-stu-id="089d2-161">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_device-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="089d2-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="089d2-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_device-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="089d2-163">Confira também</span><span class="sxs-lookup"><span data-stu-id="089d2-163">See also</span></span>

- [<span data-ttu-id="089d2-164">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="089d2-164">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="089d2-165">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="089d2-165">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="089d2-166">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="089d2-166">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/device-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/device-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
