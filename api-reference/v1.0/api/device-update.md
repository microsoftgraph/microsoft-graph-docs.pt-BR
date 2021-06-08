---
title: Atualizar dispositivo
description: Atualiza as propriedades de um dispositivo registrado.
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: ef160a0e31ee5753258e8da4403158c693a13e5e
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787818"
---
# <a name="update-device"></a><span data-ttu-id="ece56-103">Atualizar dispositivo</span><span class="sxs-lookup"><span data-stu-id="ece56-103">Update device</span></span>

<span data-ttu-id="ece56-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ece56-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ece56-105">Atualiza as propriedades de um dispositivo registrado.</span><span class="sxs-lookup"><span data-stu-id="ece56-105">Update the properties of a registered device.</span></span>

<span data-ttu-id="ece56-106">Somente algumas propriedades de um dispositivo podem ser atualizadas por meio de aplicativos de gerenciamento de dispositivo móvel aprovados(MDM).</span><span class="sxs-lookup"><span data-stu-id="ece56-106">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="ece56-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ece56-107">Permissions</span></span>
<span data-ttu-id="ece56-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ece56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ece56-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ece56-110">Permission type</span></span>      | <span data-ttu-id="ece56-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ece56-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ece56-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ece56-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ece56-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ece56-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="ece56-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ece56-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ece56-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ece56-115">Not supported.</span></span> |
|<span data-ttu-id="ece56-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ece56-116">Application</span></span> | <span data-ttu-id="ece56-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ece56-117">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="ece56-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ece56-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```
> <span data-ttu-id="ece56-119">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="ece56-119">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ece56-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ece56-120">Request headers</span></span>
| <span data-ttu-id="ece56-121">Nome</span><span class="sxs-lookup"><span data-stu-id="ece56-121">Name</span></span>       | <span data-ttu-id="ece56-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="ece56-122">Type</span></span> | <span data-ttu-id="ece56-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ece56-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ece56-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ece56-124">Authorization</span></span>  | <span data-ttu-id="ece56-125">string</span><span class="sxs-lookup"><span data-stu-id="ece56-125">string</span></span>  | <span data-ttu-id="ece56-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ece56-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ece56-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ece56-128">Request body</span></span>

<span data-ttu-id="ece56-129">No corpo da solicitação, forneça os valores para as propriedades [device](../resources/device.md) que devem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="ece56-129">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="ece56-130">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="ece56-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ece56-131">Para obter um melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="ece56-131">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ece56-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ece56-132">Property</span></span>     | <span data-ttu-id="ece56-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="ece56-133">Type</span></span>   |<span data-ttu-id="ece56-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="ece56-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ece56-135">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="ece56-135">accountEnabled</span></span>|<span data-ttu-id="ece56-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="ece56-136">Boolean</span></span>| <span data-ttu-id="ece56-137">**true** se a conta estiver habilitada; caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="ece56-137">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="ece56-138">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="ece56-138">operatingSystem</span></span>|<span data-ttu-id="ece56-139">String</span><span class="sxs-lookup"><span data-stu-id="ece56-139">String</span></span>|<span data-ttu-id="ece56-140">O tipo de sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ece56-140">The type of operating system on the device.</span></span>|
|<span data-ttu-id="ece56-141">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="ece56-141">operatingSystemVersion</span></span>|<span data-ttu-id="ece56-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ece56-142">String</span></span>|<span data-ttu-id="ece56-143">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ece56-143">The version of the operating system on the device</span></span>|
|<span data-ttu-id="ece56-144">displayName</span><span class="sxs-lookup"><span data-stu-id="ece56-144">displayName</span></span>|<span data-ttu-id="ece56-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ece56-145">String</span></span>|<span data-ttu-id="ece56-146">O nome de exibição do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ece56-146">The display name for the device.</span></span>|
|<span data-ttu-id="ece56-147">isCompliant</span><span class="sxs-lookup"><span data-stu-id="ece56-147">isCompliant</span></span>|<span data-ttu-id="ece56-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="ece56-148">Boolean</span></span>|<span data-ttu-id="ece56-149">**True** se o dispositivo está em conformidade com políticas de MDM (Gerenciamento de Dispositivo Móvel); caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="ece56-149">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="ece56-150">Isso só pode ser atualizado pelo Intune para qualquer tipo de sistema operacional de dispositivo ou por um [aplicativo MDM](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) aprovado para Windows do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="ece56-150">This can only be updated by Intune for any device OS type or by an [approved MDM app](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="ece56-151">isManaged</span><span class="sxs-lookup"><span data-stu-id="ece56-151">isManaged</span></span>|<span data-ttu-id="ece56-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="ece56-152">Boolean</span></span>|<span data-ttu-id="ece56-153">**true** se o dispositivo for gerenciado por um aplicativo de gerenciamento de dispositivo móvel (MDM); caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="ece56-153">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="ece56-154">Isso só pode ser atualizado pelo Intune para qualquer tipo de sistema operacional de dispositivo ou por um [aplicativo MDM](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) aprovado para Windows do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="ece56-154">This can only be updated by Intune for any device OS type or by an [approved MDM app](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

## <a name="response"></a><span data-ttu-id="ece56-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="ece56-155">Response</span></span>

<span data-ttu-id="ece56-156">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ece56-156">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ece56-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ece56-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ece56-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ece56-158">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ece56-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="ece56-159">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ece56-160">C#</span><span class="sxs-lookup"><span data-stu-id="ece56-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ece56-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ece56-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ece56-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ece56-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ece56-163">Java</span><span class="sxs-lookup"><span data-stu-id="ece56-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-device-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ece56-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="ece56-164">Response</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
