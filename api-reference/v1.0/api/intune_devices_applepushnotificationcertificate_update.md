# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="5e24a-101">Atualizar applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="5e24a-101">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="5e24a-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5e24a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5e24a-103">Atualizar as propriedades de um objeto [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="5e24a-103">Update the properties of a [calendar](../resources/intune_devices_applepushnotificationcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5e24a-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5e24a-104">Prerequisites</span></span>
<span data-ttu-id="5e24a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5e24a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5e24a-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e24a-107">Permission type</span></span>|<span data-ttu-id="5e24a-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5e24a-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e24a-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e24a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5e24a-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e24a-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5e24a-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e24a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e24a-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e24a-112">Not supported.</span></span>|
|<span data-ttu-id="5e24a-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5e24a-113">Application</span></span>|<span data-ttu-id="5e24a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e24a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e24a-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e24a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="5e24a-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e24a-116">Request headers</span></span>
|<span data-ttu-id="5e24a-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5e24a-117">Header</span></span>|<span data-ttu-id="5e24a-118">Valor</span><span class="sxs-lookup"><span data-stu-id="5e24a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e24a-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e24a-119">Authorization</span></span>|<span data-ttu-id="5e24a-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e24a-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5e24a-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5e24a-121">Accept</span></span>|<span data-ttu-id="5e24a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5e24a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e24a-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e24a-123">Request body</span></span>
<span data-ttu-id="5e24a-124">No corpo da solicitação, forneça uma representação JSON do objeto [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="5e24a-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_devices_applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="5e24a-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="5e24a-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="5e24a-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e24a-126">Property</span></span>|<span data-ttu-id="5e24a-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e24a-127">Type</span></span>|<span data-ttu-id="5e24a-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e24a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e24a-129">id</span><span class="sxs-lookup"><span data-stu-id="5e24a-129">id</span></span>|<span data-ttu-id="5e24a-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e24a-130">String</span></span>|<span data-ttu-id="5e24a-131">O identificador exclusivo do certificado.</span><span class="sxs-lookup"><span data-stu-id="5e24a-131">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="5e24a-132">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="5e24a-132">appleIdentifier</span></span>|<span data-ttu-id="5e24a-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e24a-133">String</span></span>|<span data-ttu-id="5e24a-134">Id da Apple da conta usada para criar o certificado de push do MDM.</span><span class="sxs-lookup"><span data-stu-id="5e24a-134">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="5e24a-135">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="5e24a-135">topicIdentifier</span></span>|<span data-ttu-id="5e24a-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e24a-136">String</span></span>|<span data-ttu-id="5e24a-137">ID do tópico.</span><span class="sxs-lookup"><span data-stu-id="5e24a-137">Topic Id.</span></span>|
|<span data-ttu-id="5e24a-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5e24a-138">lastModifiedDateTime</span></span>|<span data-ttu-id="5e24a-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e24a-139">DateTimeOffset</span></span>|<span data-ttu-id="5e24a-140">Data e hora da última modificação de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="5e24a-140">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="5e24a-141">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5e24a-141">expirationDateTime</span></span>|<span data-ttu-id="5e24a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e24a-142">DateTimeOffset</span></span>|<span data-ttu-id="5e24a-143">Data e hora do vencimento de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="5e24a-143">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="5e24a-144">certificado</span><span class="sxs-lookup"><span data-stu-id="5e24a-144">ACS, certificate</span></span>|<span data-ttu-id="5e24a-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e24a-145">String</span></span>|<span data-ttu-id="5e24a-146">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5e24a-146">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5e24a-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e24a-147">Response</span></span>
<span data-ttu-id="5e24a-148">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5e24a-148">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_devices_applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e24a-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5e24a-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="5e24a-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e24a-150">Request</span></span>
<span data-ttu-id="5e24a-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e24a-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5e24a-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e24a-152">Response</span></span>
<span data-ttu-id="5e24a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5e24a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



