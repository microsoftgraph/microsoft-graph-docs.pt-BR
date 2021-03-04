---
title: Atualizar dispositivo
description: Atualize as propriedades de um dispositivo.
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 4c5eab86a49081f859f11de1f539bdb77dc9d42f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437062"
---
# <a name="update-device"></a><span data-ttu-id="eafdf-103">Atualizar dispositivo</span><span class="sxs-lookup"><span data-stu-id="eafdf-103">Update device</span></span>

<span data-ttu-id="eafdf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eafdf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eafdf-105">Atualize as propriedades de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="eafdf-105">Update the properties of a device.</span></span>

<span data-ttu-id="eafdf-106">Somente algumas propriedades de um dispositivo podem ser atualizadas por meio de aplicativos de gerenciamento de dispositivo móvel aprovados(MDM).</span><span class="sxs-lookup"><span data-stu-id="eafdf-106">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="eafdf-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="eafdf-107">Permissions</span></span>
<span data-ttu-id="eafdf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eafdf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eafdf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eafdf-110">Permission type</span></span>      | <span data-ttu-id="eafdf-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eafdf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eafdf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eafdf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="eafdf-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="eafdf-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="eafdf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eafdf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eafdf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eafdf-115">Not supported.</span></span> |
|<span data-ttu-id="eafdf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eafdf-116">Application</span></span> | <span data-ttu-id="eafdf-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="eafdf-117">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="eafdf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eafdf-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```

> <span data-ttu-id="eafdf-119">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="eafdf-119">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eafdf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eafdf-120">Request headers</span></span>
| <span data-ttu-id="eafdf-121">Nome</span><span class="sxs-lookup"><span data-stu-id="eafdf-121">Name</span></span>       | <span data-ttu-id="eafdf-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="eafdf-122">Type</span></span> | <span data-ttu-id="eafdf-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="eafdf-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="eafdf-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="eafdf-124">Authorization</span></span>  | <span data-ttu-id="eafdf-125">string</span><span class="sxs-lookup"><span data-stu-id="eafdf-125">string</span></span>  | <span data-ttu-id="eafdf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eafdf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eafdf-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eafdf-128">Request body</span></span>

<span data-ttu-id="eafdf-129">No corpo da solicitação, forneça os valores para as propriedades [device](../resources/device.md) que devem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="eafdf-129">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="eafdf-130">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="eafdf-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="eafdf-131">Para obter um melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="eafdf-131">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="eafdf-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eafdf-132">Property</span></span>     | <span data-ttu-id="eafdf-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="eafdf-133">Type</span></span>   |<span data-ttu-id="eafdf-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="eafdf-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eafdf-135">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="eafdf-135">accountEnabled</span></span>|<span data-ttu-id="eafdf-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="eafdf-136">Boolean</span></span>| <span data-ttu-id="eafdf-137">**true** se a conta estiver habilitada; caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="eafdf-137">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="eafdf-138">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="eafdf-138">operatingSystem</span></span>|<span data-ttu-id="eafdf-139">String</span><span class="sxs-lookup"><span data-stu-id="eafdf-139">String</span></span>|<span data-ttu-id="eafdf-140">O tipo de sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="eafdf-140">The type of operating system on the device.</span></span>|
|<span data-ttu-id="eafdf-141">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="eafdf-141">operatingSystemVersion</span></span>|<span data-ttu-id="eafdf-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eafdf-142">String</span></span>|<span data-ttu-id="eafdf-143">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="eafdf-143">The version of the operating system on the device</span></span>|
|<span data-ttu-id="eafdf-144">displayName</span><span class="sxs-lookup"><span data-stu-id="eafdf-144">displayName</span></span>|<span data-ttu-id="eafdf-145">String</span><span class="sxs-lookup"><span data-stu-id="eafdf-145">String</span></span>|<span data-ttu-id="eafdf-146">O nome de exibição do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="eafdf-146">The display name for the device.</span></span>|
|<span data-ttu-id="eafdf-147">isCompliant</span><span class="sxs-lookup"><span data-stu-id="eafdf-147">isCompliant</span></span>|<span data-ttu-id="eafdf-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="eafdf-148">Boolean</span></span>|<span data-ttu-id="eafdf-149">**True** se o dispositivo está em conformidade com políticas de MDM (Gerenciamento de Dispositivo Móvel); caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="eafdf-149">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="eafdf-150">Isso só pode ser atualizado pelo Intune para qualquer tipo de sistema operacional de dispositivo ou por um [aplicativo MDM](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) aprovado para dispositivos do sistema operacional Windows.</span><span class="sxs-lookup"><span data-stu-id="eafdf-150">This can only be updated by Intune for any device OS type or by an [approved MDM app](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="eafdf-151">isManaged</span><span class="sxs-lookup"><span data-stu-id="eafdf-151">isManaged</span></span>|<span data-ttu-id="eafdf-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="eafdf-152">Boolean</span></span>|<span data-ttu-id="eafdf-153">**true** se o dispositivo for gerenciado por um aplicativo de gerenciamento de dispositivo móvel (MDM); caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="eafdf-153">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="eafdf-154">Isso só pode ser atualizado pelo Intune para qualquer tipo de sistema operacional de dispositivo ou por um [aplicativo MDM](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) aprovado para dispositivos do sistema operacional Windows.</span><span class="sxs-lookup"><span data-stu-id="eafdf-154">This can only be updated by Intune for any device OS type or by an [approved MDM app](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

<span data-ttu-id="eafdf-155">Como o **recurso de** dispositivo dá suporte a extensões, você pode usar a operação para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo em propriedades [personalizadas](/graph/extensibility-overview)de uma extensão em uma instância de dispositivo `PATCH` existente. </span><span class="sxs-lookup"><span data-stu-id="eafdf-155">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **device** instance.</span></span>

## <a name="response"></a><span data-ttu-id="eafdf-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="eafdf-156">Response</span></span>

<span data-ttu-id="eafdf-157">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="eafdf-157">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="eafdf-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eafdf-158">Example</span></span>

##### <a name="request"></a><span data-ttu-id="eafdf-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eafdf-159">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="eafdf-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="eafdf-160">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="eafdf-161">C#</span><span class="sxs-lookup"><span data-stu-id="eafdf-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eafdf-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eafdf-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eafdf-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eafdf-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eafdf-164">Java</span><span class="sxs-lookup"><span data-stu-id="eafdf-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-device-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="eafdf-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="eafdf-165">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="eafdf-166">Confira também</span><span class="sxs-lookup"><span data-stu-id="eafdf-166">See also</span></span>

- [<span data-ttu-id="eafdf-167">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="eafdf-167">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="eafdf-168">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="eafdf-168">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="eafdf-169">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="eafdf-169">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
