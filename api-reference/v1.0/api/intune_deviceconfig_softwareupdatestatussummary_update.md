# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="636ae-101">Atualizar softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="636ae-101">Update softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="636ae-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="636ae-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="636ae-103">Atualizar as propriedades de um objeto [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="636ae-103">Update the properties of a [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="636ae-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="636ae-104">Prerequisites</span></span>
<span data-ttu-id="636ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="636ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="636ae-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="636ae-107">Permission type</span></span>|<span data-ttu-id="636ae-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="636ae-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="636ae-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="636ae-109">Delegated (work or school account)</span></span>|<span data-ttu-id="636ae-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="636ae-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="636ae-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="636ae-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="636ae-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="636ae-112">Not supported.</span></span>|
|<span data-ttu-id="636ae-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="636ae-113">Application</span></span>|<span data-ttu-id="636ae-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="636ae-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="636ae-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="636ae-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="636ae-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="636ae-116">Request headers</span></span>
|<span data-ttu-id="636ae-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="636ae-117">Header</span></span>|<span data-ttu-id="636ae-118">Valor</span><span class="sxs-lookup"><span data-stu-id="636ae-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="636ae-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="636ae-119">Authorization</span></span>|<span data-ttu-id="636ae-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="636ae-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="636ae-121">Accept</span><span class="sxs-lookup"><span data-stu-id="636ae-121">Accept</span></span>|<span data-ttu-id="636ae-122">application/json</span><span class="sxs-lookup"><span data-stu-id="636ae-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="636ae-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="636ae-123">Request body</span></span>
<span data-ttu-id="636ae-124">No corpo da solicitação, forneça uma representação JSON do objeto [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="636ae-124">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="636ae-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="636ae-125">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="636ae-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="636ae-126">Property</span></span>|<span data-ttu-id="636ae-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="636ae-127">Type</span></span>|<span data-ttu-id="636ae-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="636ae-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="636ae-129">id</span><span class="sxs-lookup"><span data-stu-id="636ae-129">id</span></span>|<span data-ttu-id="636ae-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="636ae-130">String</span></span>|<span data-ttu-id="636ae-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="636ae-131">Key of the entity.</span></span>|
|<span data-ttu-id="636ae-132">displayName</span><span class="sxs-lookup"><span data-stu-id="636ae-132">displayName</span></span>|<span data-ttu-id="636ae-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="636ae-133">String</span></span>|<span data-ttu-id="636ae-134">O nome da política.</span><span class="sxs-lookup"><span data-stu-id="636ae-134">The name of the policy.</span></span>|
|<span data-ttu-id="636ae-135">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="636ae-135">compliantDeviceCount</span></span>|<span data-ttu-id="636ae-136">Int32</span><span class="sxs-lookup"><span data-stu-id="636ae-136">Int32</span></span>|<span data-ttu-id="636ae-137">Número de dispositivos em conformidade.</span><span class="sxs-lookup"><span data-stu-id="636ae-137">Number of compliant devices.</span></span>|
|<span data-ttu-id="636ae-138">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="636ae-138">nonCompliantDeviceCount</span></span>|<span data-ttu-id="636ae-139">Int32</span><span class="sxs-lookup"><span data-stu-id="636ae-139">Int32</span></span>|<span data-ttu-id="636ae-140">Número de dispositivos sem conformidade.</span><span class="sxs-lookup"><span data-stu-id="636ae-140">Number of non compliant devices.</span></span>|
|<span data-ttu-id="636ae-141">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="636ae-141">remediatedDeviceCount</span></span>|<span data-ttu-id="636ae-142">Int32</span><span class="sxs-lookup"><span data-stu-id="636ae-142">Int32</span></span>|<span data-ttu-id="636ae-143">Número de dispositivos corrigidos.</span><span class="sxs-lookup"><span data-stu-id="636ae-143">Number of remediated devices.</span></span>|
|<span data-ttu-id="636ae-144">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="636ae-144">errorDeviceCount</span></span>|<span data-ttu-id="636ae-145">Int32</span><span class="sxs-lookup"><span data-stu-id="636ae-145">Int32</span></span>|<span data-ttu-id="636ae-146">Número de dispositivos com erro.</span><span class="sxs-lookup"><span data-stu-id="636ae-146">Number of devices had error.</span></span>|
|<span data-ttu-id="636ae-147">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="636ae-147">unknownDeviceCount</span></span>|<span data-ttu-id="636ae-148">Int32</span><span class="sxs-lookup"><span data-stu-id="636ae-148">Int32</span></span>|<span data-ttu-id="636ae-149">Número de dispositivos desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="636ae-149">Number of unknown devices.</span></span>|
|<span data-ttu-id="636ae-150">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="636ae-150">conflictDeviceCount</span></span>|<span data-ttu-id="636ae-151">Int32</span><span class="sxs-lookup"><span data-stu-id="636ae-151">Int32</span></span>|<span data-ttu-id="636ae-152">Número de dispositivos em conflito.</span><span class="sxs-lookup"><span data-stu-id="636ae-152">Number of conflict devices.</span></span>|
|<span data-ttu-id="636ae-153">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="636ae-153">notApplicableDeviceCount</span></span>|<span data-ttu-id="636ae-154">Int32</span><span class="sxs-lookup"><span data-stu-id="636ae-154">Int32</span></span>|<span data-ttu-id="636ae-155">Número de dispositivos não aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="636ae-155">Number of not applicable devices.</span></span>|
|<span data-ttu-id="636ae-156">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="636ae-156">compliantUserCount</span></span>|<span data-ttu-id="636ae-157">Int32</span><span class="sxs-lookup"><span data-stu-id="636ae-157">Int32</span></span>|<span data-ttu-id="636ae-158">Número de usuários em conformidade.</span><span class="sxs-lookup"><span data-stu-id="636ae-158">Number of compliant users.</span></span>|
|<span data-ttu-id="636ae-159">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="636ae-159">nonCompliantUserCount</span></span>|<span data-ttu-id="636ae-160">Int32</span><span class="sxs-lookup"><span data-stu-id="636ae-160">Int32</span></span>|<span data-ttu-id="636ae-161">Número de usuários em não conformidade.</span><span class="sxs-lookup"><span data-stu-id="636ae-161">Number of non compliant users.</span></span>|
|<span data-ttu-id="636ae-162">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="636ae-162">remediatedUserCount</span></span>|<span data-ttu-id="636ae-163">Int32</span><span class="sxs-lookup"><span data-stu-id="636ae-163">Int32</span></span>|<span data-ttu-id="636ae-164">Número de usuários corrigidos.</span><span class="sxs-lookup"><span data-stu-id="636ae-164">Number of remediated users.</span></span>|
|<span data-ttu-id="636ae-165">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="636ae-165">errorUserCount</span></span>|<span data-ttu-id="636ae-166">Int32</span><span class="sxs-lookup"><span data-stu-id="636ae-166">Int32</span></span>|<span data-ttu-id="636ae-167">Número de usuários com erro.</span><span class="sxs-lookup"><span data-stu-id="636ae-167">Number of users had error.</span></span>|
|<span data-ttu-id="636ae-168">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="636ae-168">unknownUserCount</span></span>|<span data-ttu-id="636ae-169">Int32</span><span class="sxs-lookup"><span data-stu-id="636ae-169">Int32</span></span>|<span data-ttu-id="636ae-170">Número de usuários desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="636ae-170">Number of unknown users.</span></span>|
|<span data-ttu-id="636ae-171">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="636ae-171">conflictUserCount</span></span>|<span data-ttu-id="636ae-172">Int32</span><span class="sxs-lookup"><span data-stu-id="636ae-172">Int32</span></span>|<span data-ttu-id="636ae-173">Número de usuários com conflitos.</span><span class="sxs-lookup"><span data-stu-id="636ae-173">Number of conflict users.</span></span>|
|<span data-ttu-id="636ae-174">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="636ae-174">notApplicableUserCount</span></span>|<span data-ttu-id="636ae-175">Int32</span><span class="sxs-lookup"><span data-stu-id="636ae-175">Int32</span></span>|<span data-ttu-id="636ae-176">Número de usuários não aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="636ae-176">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="636ae-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="636ae-177">Response</span></span>
<span data-ttu-id="636ae-178">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="636ae-178">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="636ae-179">Exemplo</span><span class="sxs-lookup"><span data-stu-id="636ae-179">Example</span></span>
### <a name="request"></a><span data-ttu-id="636ae-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="636ae-180">Request</span></span>
<span data-ttu-id="636ae-181">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="636ae-181">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/softwareUpdateStatusSummary
Content-type: application/json
Content-length: 518

{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "displayName": "Display Name value",
  "compliantDeviceCount": 4,
  "nonCompliantDeviceCount": 7,
  "remediatedDeviceCount": 5,
  "errorDeviceCount": 0,
  "unknownDeviceCount": 2,
  "conflictDeviceCount": 3,
  "notApplicableDeviceCount": 8,
  "compliantUserCount": 2,
  "nonCompliantUserCount": 5,
  "remediatedUserCount": 3,
  "errorUserCount": 14,
  "unknownUserCount": 0,
  "conflictUserCount": 1,
  "notApplicableUserCount": 6
}
```

### <a name="response"></a><span data-ttu-id="636ae-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="636ae-182">Response</span></span>
<span data-ttu-id="636ae-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="636ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 567

{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "id": "4f71421f-421f-4f71-1f42-714f1f42714f",
  "displayName": "Display Name value",
  "compliantDeviceCount": 4,
  "nonCompliantDeviceCount": 7,
  "remediatedDeviceCount": 5,
  "errorDeviceCount": 0,
  "unknownDeviceCount": 2,
  "conflictDeviceCount": 3,
  "notApplicableDeviceCount": 8,
  "compliantUserCount": 2,
  "nonCompliantUserCount": 5,
  "remediatedUserCount": 3,
  "errorUserCount": 14,
  "unknownUserCount": 0,
  "conflictUserCount": 1,
  "notApplicableUserCount": 6
}
```



