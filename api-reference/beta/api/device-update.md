---
title: Atualizar dispositivo
description: Atualizar as propriedades de um dispositivo.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e44e28ea9d496e039d2820098ec8f1ce8caae643
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42435553"
---
# <a name="update-device"></a><span data-ttu-id="3844c-103">Atualizar dispositivo</span><span class="sxs-lookup"><span data-stu-id="3844c-103">Update device</span></span>

<span data-ttu-id="3844c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3844c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3844c-105">Atualizar as propriedades de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3844c-105">Update the properties of a device.</span></span>

<span data-ttu-id="3844c-106">Somente algumas propriedades de um dispositivo podem ser atualizadas por meio de aplicativos de gerenciamento de dispositivo móvel aprovados(MDM).</span><span class="sxs-lookup"><span data-stu-id="3844c-106">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="3844c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3844c-107">Permissions</span></span>
<span data-ttu-id="3844c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3844c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3844c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3844c-110">Permission type</span></span>      | <span data-ttu-id="3844c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3844c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3844c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3844c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3844c-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3844c-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="3844c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3844c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3844c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3844c-115">Not supported.</span></span> |
|<span data-ttu-id="3844c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3844c-116">Application</span></span> | <span data-ttu-id="3844c-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3844c-117">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="3844c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3844c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```

> <span data-ttu-id="3844c-119">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="3844c-119">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3844c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3844c-120">Request headers</span></span>
| <span data-ttu-id="3844c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="3844c-121">Name</span></span>       | <span data-ttu-id="3844c-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="3844c-122">Type</span></span> | <span data-ttu-id="3844c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3844c-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3844c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3844c-124">Authorization</span></span>  | <span data-ttu-id="3844c-125">string</span><span class="sxs-lookup"><span data-stu-id="3844c-125">string</span></span>  | <span data-ttu-id="3844c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3844c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3844c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3844c-128">Request body</span></span>

<span data-ttu-id="3844c-129">No corpo da solicitação, forneça os valores para as propriedades [device](../resources/device.md) que devem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="3844c-129">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="3844c-130">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="3844c-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="3844c-131">Para obter um melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="3844c-131">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3844c-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3844c-132">Property</span></span>     | <span data-ttu-id="3844c-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="3844c-133">Type</span></span>   |<span data-ttu-id="3844c-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="3844c-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3844c-135">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="3844c-135">accountEnabled</span></span>|<span data-ttu-id="3844c-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="3844c-136">Boolean</span></span>| <span data-ttu-id="3844c-137">**true** se a conta estiver habilitada; caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="3844c-137">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="3844c-138">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="3844c-138">operatingSystem</span></span>|<span data-ttu-id="3844c-139">String</span><span class="sxs-lookup"><span data-stu-id="3844c-139">String</span></span>|<span data-ttu-id="3844c-140">O tipo de sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3844c-140">The type of operating system on the device.</span></span>|
|<span data-ttu-id="3844c-141">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="3844c-141">operatingSystemVersion</span></span>|<span data-ttu-id="3844c-142">String</span><span class="sxs-lookup"><span data-stu-id="3844c-142">String</span></span>|<span data-ttu-id="3844c-143">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3844c-143">The version of the operating system on the device</span></span>|
|<span data-ttu-id="3844c-144">displayName</span><span class="sxs-lookup"><span data-stu-id="3844c-144">displayName</span></span>|<span data-ttu-id="3844c-145">String</span><span class="sxs-lookup"><span data-stu-id="3844c-145">String</span></span>|<span data-ttu-id="3844c-146">O nome de exibição do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3844c-146">The display name for the device.</span></span>|
|<span data-ttu-id="3844c-147">isCompliant</span><span class="sxs-lookup"><span data-stu-id="3844c-147">isCompliant</span></span>|<span data-ttu-id="3844c-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="3844c-148">Boolean</span></span>|<span data-ttu-id="3844c-149">**True** se o dispositivo está em conformidade com políticas de MDM (Gerenciamento de Dispositivo Móvel); caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="3844c-149">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="3844c-150">Isso só pode ser atualizado pelo Intune para qualquer tipo de sistema operacional do dispositivo ou por um [aplicativo MDM aprovado](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) para dispositivos do sistema operacional Windows.</span><span class="sxs-lookup"><span data-stu-id="3844c-150">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="3844c-151">isManaged</span><span class="sxs-lookup"><span data-stu-id="3844c-151">isManaged</span></span>|<span data-ttu-id="3844c-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="3844c-152">Boolean</span></span>|<span data-ttu-id="3844c-153">**true** se o dispositivo for gerenciado por um aplicativo de gerenciamento de dispositivo móvel (MDM); caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="3844c-153">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="3844c-154">Isso só pode ser atualizado pelo Intune para qualquer tipo de sistema operacional do dispositivo ou por um [aplicativo MDM aprovado](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) para dispositivos do sistema operacional Windows.</span><span class="sxs-lookup"><span data-stu-id="3844c-154">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

<span data-ttu-id="3844c-155">Como o recurso de **dispositivo** suporta [extensões](/graph/extensibility-overview), você pode usar `PATCH` a operação para adicionar, atualizar ou excluir seus próprios dados específicos de aplicativo em Propriedades personalizadas de uma extensão em uma instância de **dispositivo** existente.</span><span class="sxs-lookup"><span data-stu-id="3844c-155">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **device** instance.</span></span>

## <a name="response"></a><span data-ttu-id="3844c-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="3844c-156">Response</span></span>

<span data-ttu-id="3844c-157">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3844c-157">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3844c-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3844c-158">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3844c-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3844c-159">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3844c-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="3844c-160">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3844c-161">C#</span><span class="sxs-lookup"><span data-stu-id="3844c-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3844c-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3844c-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3844c-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3844c-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3844c-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="3844c-164">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="3844c-165">Confira também</span><span class="sxs-lookup"><span data-stu-id="3844c-165">See also</span></span>

- [<span data-ttu-id="3844c-166">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="3844c-166">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="3844c-167">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="3844c-167">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="3844c-168">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="3844c-168">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
  ]
}
-->
