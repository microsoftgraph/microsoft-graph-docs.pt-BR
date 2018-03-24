# <a name="update-androidforworkenrollmentprofile"></a><span data-ttu-id="101ed-101">Atualizar androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="101ed-101">Update androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="101ed-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="101ed-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="101ed-103">Atualizar as propriedades de um objeto [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="101ed-103">Update the properties of a [calendar](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="101ed-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="101ed-104">Prerequisites</span></span>
<span data-ttu-id="101ed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="101ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="101ed-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="101ed-107">Permission type</span></span>|<span data-ttu-id="101ed-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="101ed-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="101ed-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="101ed-109">Delegated (work or school account)</span></span>|<span data-ttu-id="101ed-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="101ed-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="101ed-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="101ed-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="101ed-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="101ed-112">Not supported.</span></span>|
|<span data-ttu-id="101ed-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="101ed-113">Application</span></span>|<span data-ttu-id="101ed-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="101ed-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="101ed-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="101ed-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="101ed-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="101ed-116">Request headers</span></span>
|<span data-ttu-id="101ed-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="101ed-117">Header</span></span>|<span data-ttu-id="101ed-118">Valor</span><span class="sxs-lookup"><span data-stu-id="101ed-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="101ed-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="101ed-119">Authorization</span></span>|<span data-ttu-id="101ed-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="101ed-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="101ed-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="101ed-121">Accept</span></span>|<span data-ttu-id="101ed-122">application/json</span><span class="sxs-lookup"><span data-stu-id="101ed-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="101ed-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="101ed-123">Request body</span></span>
<span data-ttu-id="101ed-124">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="101ed-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) object.</span></span>

<span data-ttu-id="101ed-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="101ed-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="101ed-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="101ed-126">Property</span></span>|<span data-ttu-id="101ed-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="101ed-127">Type</span></span>|<span data-ttu-id="101ed-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="101ed-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="101ed-129">accountId</span><span class="sxs-lookup"><span data-stu-id="101ed-129">accountId</span></span>|<span data-ttu-id="101ed-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="101ed-130">String</span></span>|<span data-ttu-id="101ed-131">GUID de locatário ao qual o perfil de registro pertence.</span><span class="sxs-lookup"><span data-stu-id="101ed-131">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="101ed-132">id</span><span class="sxs-lookup"><span data-stu-id="101ed-132">id</span></span>|<span data-ttu-id="101ed-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="101ed-133">String</span></span>|<span data-ttu-id="101ed-134">GUID exclusivo do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="101ed-134">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="101ed-135">nome</span><span class="sxs-lookup"><span data-stu-id="101ed-135">name</span></span>|<span data-ttu-id="101ed-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="101ed-136">String</span></span>|<span data-ttu-id="101ed-137">(Preterido) Nome de exibição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="101ed-137">(Deprecated) Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="101ed-138">displayName</span><span class="sxs-lookup"><span data-stu-id="101ed-138">displayName</span></span>|<span data-ttu-id="101ed-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="101ed-139">String</span></span>|<span data-ttu-id="101ed-140">Nome de exibição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="101ed-140">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="101ed-141">descrição</span><span class="sxs-lookup"><span data-stu-id="101ed-141">description</span></span>|<span data-ttu-id="101ed-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="101ed-142">String</span></span>|<span data-ttu-id="101ed-143">Descrição do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="101ed-143">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="101ed-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="101ed-144">createdDateTime</span></span>|<span data-ttu-id="101ed-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="101ed-145">DateTimeOffset</span></span>|<span data-ttu-id="101ed-146">Data e hora de criação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="101ed-146">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="101ed-147">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="101ed-147">modifiedDateTime</span></span>|<span data-ttu-id="101ed-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="101ed-148">DateTimeOffset</span></span>|<span data-ttu-id="101ed-149">(Preterido) Data e hora da última modificação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="101ed-149">(Deprecated) Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="101ed-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="101ed-150">lastModifiedDateTime</span></span>|<span data-ttu-id="101ed-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="101ed-151">DateTimeOffset</span></span>|<span data-ttu-id="101ed-152">Data e hora da última modificação do perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="101ed-152">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="101ed-153">tokenValue</span><span class="sxs-lookup"><span data-stu-id="101ed-153">tokenValue</span></span>|<span data-ttu-id="101ed-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="101ed-154">String</span></span>|<span data-ttu-id="101ed-155">Valor do token mais recentemente criado para este perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="101ed-155">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="101ed-156">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="101ed-156">tokenExpirationDateTime</span></span>|<span data-ttu-id="101ed-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="101ed-157">DateTimeOffset</span></span>|<span data-ttu-id="101ed-158">Data e hora em que o token mais recentemente criado expirará.</span><span class="sxs-lookup"><span data-stu-id="101ed-158">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="101ed-159">totalEnrollmentCount</span><span class="sxs-lookup"><span data-stu-id="101ed-159">totalEnrollmentCount</span></span>|<span data-ttu-id="101ed-160">Int32</span><span class="sxs-lookup"><span data-stu-id="101ed-160">Int32</span></span>|<span data-ttu-id="101ed-161">(Preterido) Número total de dispositivos Android que foram registrados usando esse perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="101ed-161">(Deprecated) Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="101ed-162">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="101ed-162">enrolledDeviceCount</span></span>|<span data-ttu-id="101ed-163">Int32</span><span class="sxs-lookup"><span data-stu-id="101ed-163">Int32</span></span>|<span data-ttu-id="101ed-164">Número total de dispositivos Android que foram registrados usando esse perfil de registro.</span><span class="sxs-lookup"><span data-stu-id="101ed-164">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="101ed-165">qrCode</span><span class="sxs-lookup"><span data-stu-id="101ed-165">qrCode</span></span>|<span data-ttu-id="101ed-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="101ed-166">String</span></span>|<span data-ttu-id="101ed-167">(Preterido) Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="101ed-167">(Deprecated) String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="101ed-168">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="101ed-168">qrCodeContent</span></span>|<span data-ttu-id="101ed-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="101ed-169">String</span></span>|<span data-ttu-id="101ed-170">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="101ed-170">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="101ed-171">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="101ed-171">qrCodeImage</span></span>|[<span data-ttu-id="101ed-172">mimeContent</span><span class="sxs-lookup"><span data-stu-id="101ed-172">mimeContent</span></span>](../resources/intune_androidforwork_mimecontent.md)|<span data-ttu-id="101ed-173">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="101ed-173">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="101ed-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="101ed-174">Response</span></span>
<span data-ttu-id="101ed-175">Se tiver êxito, este método retornará um código de resposta `200 OK` e o objeto [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="101ed-175">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="101ed-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="101ed-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="101ed-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="101ed-177">Request</span></span>
<span data-ttu-id="101ed-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="101ed-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
Content-type: application/json
Content-length: 575

{
  "accountId": "Account Id value",
  "name": "Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "tokenValue": "Token Value value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "totalEnrollmentCount": 4,
  "enrolledDeviceCount": 3,
  "qrCode": "Qr Code value",
  "qrCodeContent": "Qr Code Content value",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```

### <a name="response"></a><span data-ttu-id="101ed-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="101ed-179">Response</span></span>
<span data-ttu-id="101ed-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="101ed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 813

{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "accountId": "Account Id value",
  "id": "e6742553-2553-e674-5325-74e6532574e6",
  "name": "Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "tokenValue": "Token Value value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "totalEnrollmentCount": 4,
  "enrolledDeviceCount": 3,
  "qrCode": "Qr Code value",
  "qrCodeContent": "Qr Code Content value",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```



