# <a name="update-device"></a><span data-ttu-id="7b8a1-101">Atualizar dispositivo</span><span class="sxs-lookup"><span data-stu-id="7b8a1-101">Update device</span></span>

<span data-ttu-id="7b8a1-102">Atualiza as propriedades de um dispositivo registrado.</span><span class="sxs-lookup"><span data-stu-id="7b8a1-102">Update the properties of a registered device.</span></span>

<span data-ttu-id="7b8a1-103">Somente algumas propriedades de um dispositivo podem ser atualizadas por meio de aplicativos de gerenciamento de dispositivo móvel aprovados(MDM).</span><span class="sxs-lookup"><span data-stu-id="7b8a1-103">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b8a1-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="7b8a1-104">Permissions</span></span>
<span data-ttu-id="7b8a1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7b8a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7b8a1-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7b8a1-107">Permission type</span></span>      | <span data-ttu-id="7b8a1-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7b8a1-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b8a1-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7b8a1-109">Delegated (work or school account)</span></span> | <span data-ttu-id="7b8a1-110">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7b8a1-110">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="7b8a1-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7b8a1-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b8a1-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b8a1-112">Not supported.</span></span> |
|<span data-ttu-id="7b8a1-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7b8a1-113">Application</span></span> | <span data-ttu-id="7b8a1-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7b8a1-114">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b8a1-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7b8a1-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```
> <span data-ttu-id="7b8a1-116">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="7b8a1-116">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b8a1-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7b8a1-117">Request headers</span></span>
| <span data-ttu-id="7b8a1-118">Nome</span><span class="sxs-lookup"><span data-stu-id="7b8a1-118">Name</span></span>       | <span data-ttu-id="7b8a1-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b8a1-119">Type</span></span> | <span data-ttu-id="7b8a1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b8a1-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7b8a1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7b8a1-121">Authorization</span></span>  | <span data-ttu-id="7b8a1-122">string</span><span class="sxs-lookup"><span data-stu-id="7b8a1-122">string</span></span>  | <span data-ttu-id="7b8a1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b8a1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b8a1-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7b8a1-125">Request body</span></span>

<span data-ttu-id="7b8a1-126">No corpo da solicitação, forneça os valores para as propriedades [device](../resources/device.md) que devem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="7b8a1-126">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="7b8a1-127">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="7b8a1-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="7b8a1-128">Para obter o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="7b8a1-128">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7b8a1-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b8a1-129">Property</span></span>     | <span data-ttu-id="7b8a1-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b8a1-130">Type</span></span>   |<span data-ttu-id="7b8a1-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b8a1-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b8a1-132">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="7b8a1-132">accountEnabled</span></span>|<span data-ttu-id="7b8a1-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b8a1-133">Boolean</span></span>| <span data-ttu-id="7b8a1-134">**true** se a conta estiver habilitada; caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="7b8a1-134">true if the account is enabled; otherwise, false.</span></span> |
|<span data-ttu-id="7b8a1-135">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="7b8a1-135">operatingSystem</span></span>|<span data-ttu-id="7b8a1-136">String</span><span class="sxs-lookup"><span data-stu-id="7b8a1-136">String</span></span>|<span data-ttu-id="7b8a1-137">O tipo de sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7b8a1-137">The type of operating system on the device. Required.</span></span>|
|<span data-ttu-id="7b8a1-138">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="7b8a1-138">operatingSystemVersion</span></span>|<span data-ttu-id="7b8a1-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7b8a1-139">String</span></span>|<span data-ttu-id="7b8a1-140">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7b8a1-140">The version of the operating system on the device. Required.</span></span>|
|<span data-ttu-id="7b8a1-141">displayName</span><span class="sxs-lookup"><span data-stu-id="7b8a1-141">displayName</span></span>|<span data-ttu-id="7b8a1-142">String</span><span class="sxs-lookup"><span data-stu-id="7b8a1-142">String</span></span>|<span data-ttu-id="7b8a1-143">O nome de exibição do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7b8a1-143">The display name for the device. Required.</span></span>|
|<span data-ttu-id="7b8a1-144">isCompliant</span><span class="sxs-lookup"><span data-stu-id="7b8a1-144">isCompliant</span></span>|<span data-ttu-id="7b8a1-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="7b8a1-145">Boolean</span></span>|<span data-ttu-id="7b8a1-146">**True** se o dispositivo está em conformidade com políticas de MDM (Gerenciamento de Dispositivo Móvel); caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="7b8a1-146">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="7b8a1-147">A atualização só pode ser feita por um aplicativo MDM aprovado.</span><span class="sxs-lookup"><span data-stu-id="7b8a1-147">This can only be updated by an approved MDM app.</span></span> |
|<span data-ttu-id="7b8a1-148">isManaged</span><span class="sxs-lookup"><span data-stu-id="7b8a1-148">isManaged</span></span>|<span data-ttu-id="7b8a1-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="7b8a1-149">Boolean</span></span>|<span data-ttu-id="7b8a1-150">**true** se o dispositivo for gerenciado por um aplicativo de gerenciamento de dispositivo móvel (MDM); caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="7b8a1-150">**true** if the device is managed by a Mobile Device Management (MDM) app such as Intune; otherwise, **false**.</span></span> <span data-ttu-id="7b8a1-151">A atualização só pode ser feita por um aplicativo MDM aprovado.</span><span class="sxs-lookup"><span data-stu-id="7b8a1-151">This can only be updated by an approved MDM app.</span></span> |

## <a name="response"></a><span data-ttu-id="7b8a1-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b8a1-152">Response</span></span>

<span data-ttu-id="7b8a1-153">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7b8a1-153">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7b8a1-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7b8a1-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7b8a1-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b8a1-155">Request</span></span>

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
##### <a name="response"></a><span data-ttu-id="7b8a1-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b8a1-156">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```
