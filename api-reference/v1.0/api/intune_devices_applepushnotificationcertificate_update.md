# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="9a8c5-101">Atualizar applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="9a8c5-101">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="9a8c5-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9a8c5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9a8c5-103">Atualizar as propriedades de um objeto [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="9a8c5-103">Update the properties of a [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9a8c5-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9a8c5-104">Prerequisites</span></span>
<span data-ttu-id="9a8c5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9a8c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9a8c5-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a8c5-107">Permission type</span></span>|<span data-ttu-id="9a8c5-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9a8c5-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a8c5-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a8c5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9a8c5-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a8c5-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9a8c5-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a8c5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a8c5-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a8c5-112">Not supported.</span></span>|
|<span data-ttu-id="9a8c5-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a8c5-113">Application</span></span>|<span data-ttu-id="9a8c5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a8c5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a8c5-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a8c5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="9a8c5-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a8c5-116">Request headers</span></span>
|<span data-ttu-id="9a8c5-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9a8c5-117">Header</span></span>|<span data-ttu-id="9a8c5-118">Valor</span><span class="sxs-lookup"><span data-stu-id="9a8c5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a8c5-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a8c5-119">Authorization</span></span>|<span data-ttu-id="9a8c5-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="9a8c5-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a8c5-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9a8c5-121">Accept</span></span>|<span data-ttu-id="9a8c5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="9a8c5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a8c5-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a8c5-123">Request body</span></span>
<span data-ttu-id="9a8c5-124">No corpo da solicitação, forneça uma representação JSON do objeto [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="9a8c5-124">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="9a8c5-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="9a8c5-125">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="9a8c5-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a8c5-126">Property</span></span>|<span data-ttu-id="9a8c5-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a8c5-127">Type</span></span>|<span data-ttu-id="9a8c5-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a8c5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a8c5-129">id</span><span class="sxs-lookup"><span data-stu-id="9a8c5-129">id</span></span>|<span data-ttu-id="9a8c5-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a8c5-130">String</span></span>|<span data-ttu-id="9a8c5-131">O identificador exclusivo do certificado.</span><span class="sxs-lookup"><span data-stu-id="9a8c5-131">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="9a8c5-132">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="9a8c5-132">appleIdentifier</span></span>|<span data-ttu-id="9a8c5-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a8c5-133">String</span></span>|<span data-ttu-id="9a8c5-134">Id da Apple da conta usada para criar o certificado de push do MDM.</span><span class="sxs-lookup"><span data-stu-id="9a8c5-134">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="9a8c5-135">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="9a8c5-135">topicIdentifier</span></span>|<span data-ttu-id="9a8c5-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a8c5-136">String</span></span>|<span data-ttu-id="9a8c5-137">ID do tópico.</span><span class="sxs-lookup"><span data-stu-id="9a8c5-137">Topic Id.</span></span>|
|<span data-ttu-id="9a8c5-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a8c5-138">lastModifiedDateTime</span></span>|<span data-ttu-id="9a8c5-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a8c5-139">DateTimeOffset</span></span>|<span data-ttu-id="9a8c5-140">Data e hora da última modificação de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="9a8c5-140">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="9a8c5-141">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9a8c5-141">expirationDateTime</span></span>|<span data-ttu-id="9a8c5-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a8c5-142">DateTimeOffset</span></span>|<span data-ttu-id="9a8c5-143">Data e hora do vencimento de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="9a8c5-143">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="9a8c5-144">certificado</span><span class="sxs-lookup"><span data-stu-id="9a8c5-144">certificate</span></span>|<span data-ttu-id="9a8c5-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a8c5-145">String</span></span>|<span data-ttu-id="9a8c5-146">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9a8c5-146">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9a8c5-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a8c5-147">Response</span></span>
<span data-ttu-id="9a8c5-148">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a8c5-148">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a8c5-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a8c5-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="9a8c5-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a8c5-150">Request</span></span>
<span data-ttu-id="9a8c5-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a8c5-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/applePushNotificationCertificate
Content-type: application/json
Content-length: 264

{
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificate": "Certificate value"
}
```

### <a name="response"></a><span data-ttu-id="9a8c5-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a8c5-152">Response</span></span>
<span data-ttu-id="9a8c5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9a8c5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 384

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "c4c8f047-f047-c4c8-47f0-c8c447f0c8c4",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificate": "Certificate value"
}
```








