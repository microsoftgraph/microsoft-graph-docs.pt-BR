---
title: Atualizar dispositivo
description: Atualizar as propriedades de um dispositivo.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fee5f5a33a881801fa50ee5fae7a01ebbdf197cc
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33326031"
---
# <a name="update-device"></a><span data-ttu-id="2ce51-103">Atualizar dispositivo</span><span class="sxs-lookup"><span data-stu-id="2ce51-103">Update device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ce51-104">Atualizar as propriedades de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ce51-104">Update the properties of a device.</span></span>

<span data-ttu-id="2ce51-105">Somente algumas propriedades de um dispositivo podem ser atualizadas por meio de aplicativos de gerenciamento de dispositivo móvel aprovados(MDM).</span><span class="sxs-lookup"><span data-stu-id="2ce51-105">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ce51-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2ce51-106">Permissions</span></span>
<span data-ttu-id="2ce51-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ce51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ce51-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ce51-109">Permission type</span></span>      | <span data-ttu-id="2ce51-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2ce51-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ce51-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ce51-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2ce51-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2ce51-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="2ce51-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ce51-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ce51-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ce51-114">Not supported.</span></span> |
|<span data-ttu-id="2ce51-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ce51-115">Application</span></span> | <span data-ttu-id="2ce51-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2ce51-116">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ce51-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ce51-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```

> <span data-ttu-id="2ce51-118">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="2ce51-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ce51-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ce51-119">Request headers</span></span>
| <span data-ttu-id="2ce51-120">Nome</span><span class="sxs-lookup"><span data-stu-id="2ce51-120">Name</span></span>       | <span data-ttu-id="2ce51-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ce51-121">Type</span></span> | <span data-ttu-id="2ce51-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ce51-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2ce51-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ce51-123">Authorization</span></span>  | <span data-ttu-id="2ce51-124">string</span><span class="sxs-lookup"><span data-stu-id="2ce51-124">string</span></span>  | <span data-ttu-id="2ce51-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ce51-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ce51-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ce51-127">Request body</span></span>

<span data-ttu-id="2ce51-128">No corpo da solicitação, forneça os valores para as propriedades [device](../resources/device.md) que devem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="2ce51-128">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="2ce51-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="2ce51-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="2ce51-130">Para obter um melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="2ce51-130">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2ce51-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ce51-131">Property</span></span>     | <span data-ttu-id="2ce51-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ce51-132">Type</span></span>   |<span data-ttu-id="2ce51-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ce51-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ce51-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="2ce51-134">accountEnabled</span></span>|<span data-ttu-id="2ce51-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="2ce51-135">Boolean</span></span>| <span data-ttu-id="2ce51-136">**true** se a conta estiver habilitada; caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="2ce51-136">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="2ce51-137">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="2ce51-137">operatingSystem</span></span>|<span data-ttu-id="2ce51-138">String</span><span class="sxs-lookup"><span data-stu-id="2ce51-138">String</span></span>|<span data-ttu-id="2ce51-139">O tipo de sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ce51-139">The type of operating system on the device.</span></span>|
|<span data-ttu-id="2ce51-140">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="2ce51-140">operatingSystemVersion</span></span>|<span data-ttu-id="2ce51-141">String</span><span class="sxs-lookup"><span data-stu-id="2ce51-141">String</span></span>|<span data-ttu-id="2ce51-142">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ce51-142">The version of the operating system on the device</span></span>|
|<span data-ttu-id="2ce51-143">displayName</span><span class="sxs-lookup"><span data-stu-id="2ce51-143">displayName</span></span>|<span data-ttu-id="2ce51-144">String</span><span class="sxs-lookup"><span data-stu-id="2ce51-144">String</span></span>|<span data-ttu-id="2ce51-145">O nome de exibição do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ce51-145">The display name for the device.</span></span>|
|<span data-ttu-id="2ce51-146">isCompliant</span><span class="sxs-lookup"><span data-stu-id="2ce51-146">isCompliant</span></span>|<span data-ttu-id="2ce51-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ce51-147">Boolean</span></span>|<span data-ttu-id="2ce51-148">**True** se o dispositivo está em conformidade com políticas de MDM (Gerenciamento de Dispositivo Móvel); caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="2ce51-148">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="2ce51-149">Isso só pode ser atualizado pelo Intune para qualquer tipo de sistema operacional do dispositivo ou por um [aplicativo MDM aprovado](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) para dispositivos do sistema operacional Windows.</span><span class="sxs-lookup"><span data-stu-id="2ce51-149">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="2ce51-150">isManaged</span><span class="sxs-lookup"><span data-stu-id="2ce51-150">isManaged</span></span>|<span data-ttu-id="2ce51-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="2ce51-151">Boolean</span></span>|<span data-ttu-id="2ce51-152">**true** se o dispositivo for gerenciado por um aplicativo de gerenciamento de dispositivo móvel (MDM); caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="2ce51-152">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="2ce51-153">Isso só pode ser atualizado pelo Intune para qualquer tipo de sistema operacional do dispositivo ou por um [aplicativo MDM aprovado](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) para dispositivos do sistema operacional Windows.</span><span class="sxs-lookup"><span data-stu-id="2ce51-153">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

<span data-ttu-id="2ce51-154">Como o recurso de **dispositivo** suporta [extensões](/graph/extensibility-overview), você pode usar `PATCH` a operação para adicionar, atualizar ou excluir seus próprios dados específicos de aplicativo em Propriedades personalizadas de uma extensão em uma instância de **dispositivo** existente.</span><span class="sxs-lookup"><span data-stu-id="2ce51-154">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **device** instance.</span></span>

## <a name="response"></a><span data-ttu-id="2ce51-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ce51-155">Response</span></span>

<span data-ttu-id="2ce51-156">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2ce51-156">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2ce51-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ce51-157">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2ce51-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ce51-158">Request</span></span>

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
##### <a name="response"></a><span data-ttu-id="2ce51-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ce51-159">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="2ce51-160">Confira também</span><span class="sxs-lookup"><span data-stu-id="2ce51-160">See also</span></span>

- [<span data-ttu-id="2ce51-161">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="2ce51-161">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="2ce51-162">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="2ce51-162">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="2ce51-163">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="2ce51-163">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
