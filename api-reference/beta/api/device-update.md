---
title: Atualizar dispositivo
description: Atualize as propriedades de um dispositivo.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 42471e32eac050b84e36477c1cd48fd06feb4244
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916373"
---
# <a name="update-device"></a><span data-ttu-id="be2f8-103">Atualizar dispositivo</span><span class="sxs-lookup"><span data-stu-id="be2f8-103">Update device</span></span>

> <span data-ttu-id="be2f8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="be2f8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be2f8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="be2f8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="be2f8-106">Atualize as propriedades de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="be2f8-106">Update the properties of a device.</span></span>

<span data-ttu-id="be2f8-107">Somente algumas propriedades de um dispositivo podem ser atualizadas por meio de aplicativos de gerenciamento de dispositivo móvel aprovados(MDM).</span><span class="sxs-lookup"><span data-stu-id="be2f8-107">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="be2f8-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="be2f8-108">Permissions</span></span>
<span data-ttu-id="be2f8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be2f8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be2f8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be2f8-111">Permission type</span></span>      | <span data-ttu-id="be2f8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="be2f8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be2f8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be2f8-113">Delegated (work or school account)</span></span> | <span data-ttu-id="be2f8-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="be2f8-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="be2f8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="be2f8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be2f8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be2f8-116">Not supported.</span></span> |
|<span data-ttu-id="be2f8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="be2f8-117">Application</span></span> | <span data-ttu-id="be2f8-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="be2f8-118">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="be2f8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be2f8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```

> <span data-ttu-id="be2f8-120">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="be2f8-120">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="be2f8-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be2f8-121">Request headers</span></span>
| <span data-ttu-id="be2f8-122">Nome</span><span class="sxs-lookup"><span data-stu-id="be2f8-122">Name</span></span>       | <span data-ttu-id="be2f8-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="be2f8-123">Type</span></span> | <span data-ttu-id="be2f8-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="be2f8-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="be2f8-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="be2f8-125">Authorization</span></span>  | <span data-ttu-id="be2f8-126">string</span><span class="sxs-lookup"><span data-stu-id="be2f8-126">string</span></span>  | <span data-ttu-id="be2f8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be2f8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be2f8-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be2f8-129">Request body</span></span>

<span data-ttu-id="be2f8-130">No corpo da solicitação, forneça os valores para as propriedades [device](../resources/device.md) que devem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="be2f8-130">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="be2f8-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="be2f8-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="be2f8-132">Para obter o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="be2f8-132">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="be2f8-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="be2f8-133">Property</span></span>     | <span data-ttu-id="be2f8-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="be2f8-134">Type</span></span>   |<span data-ttu-id="be2f8-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="be2f8-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be2f8-136">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="be2f8-136">accountEnabled</span></span>|<span data-ttu-id="be2f8-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="be2f8-137">Boolean</span></span>| <span data-ttu-id="be2f8-138">**true** se a conta estiver habilitada; caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="be2f8-138">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="be2f8-139">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="be2f8-139">operatingSystem</span></span>|<span data-ttu-id="be2f8-140">String</span><span class="sxs-lookup"><span data-stu-id="be2f8-140">String</span></span>|<span data-ttu-id="be2f8-141">O tipo de sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="be2f8-141">The type of operating system on the device.</span></span>|
|<span data-ttu-id="be2f8-142">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="be2f8-142">operatingSystemVersion</span></span>|<span data-ttu-id="be2f8-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="be2f8-143">String</span></span>|<span data-ttu-id="be2f8-144">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="be2f8-144">The version of the operating system on the device</span></span>|
|<span data-ttu-id="be2f8-145">displayName</span><span class="sxs-lookup"><span data-stu-id="be2f8-145">displayName</span></span>|<span data-ttu-id="be2f8-146">String</span><span class="sxs-lookup"><span data-stu-id="be2f8-146">String</span></span>|<span data-ttu-id="be2f8-147">O nome de exibição do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="be2f8-147">The display name for the device.</span></span>|
|<span data-ttu-id="be2f8-148">isCompliant</span><span class="sxs-lookup"><span data-stu-id="be2f8-148">isCompliant</span></span>|<span data-ttu-id="be2f8-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="be2f8-149">Boolean</span></span>|<span data-ttu-id="be2f8-150">**True** se o dispositivo está em conformidade com políticas de MDM (Gerenciamento de Dispositivo Móvel); caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="be2f8-150">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="be2f8-151">Isso só pode ser atualizado por Intune para qualquer tipo de sistema operacional do dispositivo ou por um [aprovada MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) para dispositivos do sistema operacional Windows.</span><span class="sxs-lookup"><span data-stu-id="be2f8-151">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="be2f8-152">isManaged</span><span class="sxs-lookup"><span data-stu-id="be2f8-152">isManaged</span></span>|<span data-ttu-id="be2f8-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="be2f8-153">Boolean</span></span>|<span data-ttu-id="be2f8-154">**true** se o dispositivo for gerenciado por um aplicativo de gerenciamento de dispositivo móvel (MDM); caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="be2f8-154">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="be2f8-155">Isso só pode ser atualizado por Intune para qualquer tipo de sistema operacional do dispositivo ou por um [aprovada MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) para dispositivos do sistema operacional Windows.</span><span class="sxs-lookup"><span data-stu-id="be2f8-155">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

<span data-ttu-id="be2f8-156">Desde que o recurso de **dispositivo** oferece suporte às [extensões](/graph/extensibility-overview), você pode usar o `PATCH` operação para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo nas propriedades personalizadas de uma extensão em uma instância existente do **dispositivo** .</span><span class="sxs-lookup"><span data-stu-id="be2f8-156">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **device** instance.</span></span>

## <a name="response"></a><span data-ttu-id="be2f8-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="be2f8-157">Response</span></span>

<span data-ttu-id="be2f8-158">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="be2f8-158">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="be2f8-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="be2f8-159">Example</span></span>

##### <a name="request"></a><span data-ttu-id="be2f8-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be2f8-160">Request</span></span>

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
##### <a name="response"></a><span data-ttu-id="be2f8-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="be2f8-161">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="be2f8-162">Confira também</span><span class="sxs-lookup"><span data-stu-id="be2f8-162">See also</span></span>

- [<span data-ttu-id="be2f8-163">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="be2f8-163">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="be2f8-164">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="be2f8-164">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="be2f8-165">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="be2f8-165">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
