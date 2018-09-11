# <a name="update-managedmobileapp"></a><span data-ttu-id="633ee-101">Atualizar managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="633ee-101">Update managedMobileApp</span></span>

> <span data-ttu-id="633ee-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="633ee-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="633ee-103">Atualizar as propriedades de um objeto [managedMobileApp](../resources/intune_mam_managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="633ee-103">Update the properties of a [managedMobileApp](../resources/intune_mam_managedmobileapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="633ee-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="633ee-104">Prerequisites</span></span>
<span data-ttu-id="633ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="633ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="633ee-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="633ee-107">Permission type</span></span>|<span data-ttu-id="633ee-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="633ee-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="633ee-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="633ee-109">Delegated (work or school account)</span></span>|<span data-ttu-id="633ee-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="633ee-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="633ee-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="633ee-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="633ee-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="633ee-112">Not supported.</span></span>|
|<span data-ttu-id="633ee-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="633ee-113">Application</span></span>|<span data-ttu-id="633ee-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="633ee-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="633ee-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="633ee-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps/{managedMobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="633ee-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="633ee-116">Request headers</span></span>
|<span data-ttu-id="633ee-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="633ee-117">Header</span></span>|<span data-ttu-id="633ee-118">Valor</span><span class="sxs-lookup"><span data-stu-id="633ee-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="633ee-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="633ee-119">Authorization</span></span>|<span data-ttu-id="633ee-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="633ee-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="633ee-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="633ee-121">Accept</span></span>|<span data-ttu-id="633ee-122">application/json</span><span class="sxs-lookup"><span data-stu-id="633ee-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="633ee-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="633ee-123">Request body</span></span>
<span data-ttu-id="633ee-124">No corpo da solicitação, forneça uma representação JSON do objeto [managedMobileApp](../resources/intune_mam_managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="633ee-124">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune_mam_managedmobileapp.md) object.</span></span>

<span data-ttu-id="633ee-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedMobileApp](../resources/intune_mam_managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="633ee-125">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune_mam_managedmobileapp.md).</span></span>

|<span data-ttu-id="633ee-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="633ee-126">Property</span></span>|<span data-ttu-id="633ee-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="633ee-127">Type</span></span>|<span data-ttu-id="633ee-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="633ee-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="633ee-129">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="633ee-129">mobileAppIdentifier</span></span>|[<span data-ttu-id="633ee-130">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="633ee-130">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="633ee-131">O identificador de um aplicativo com seu tipo de sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="633ee-131">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="633ee-132">id</span><span class="sxs-lookup"><span data-stu-id="633ee-132">id</span></span>|<span data-ttu-id="633ee-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="633ee-133">String</span></span>|<span data-ttu-id="633ee-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="633ee-134">Key of the entity.</span></span>|
|<span data-ttu-id="633ee-135">version</span><span class="sxs-lookup"><span data-stu-id="633ee-135">version</span></span>|<span data-ttu-id="633ee-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="633ee-136">String</span></span>|<span data-ttu-id="633ee-137">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="633ee-137">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="633ee-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="633ee-138">Response</span></span>
<span data-ttu-id="633ee-139">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedMobileApp](../resources/intune_mam_managedmobileapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="633ee-139">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune_mam_managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="633ee-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="633ee-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="633ee-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="633ee-141">Request</span></span>
<span data-ttu-id="633ee-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="633ee-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
Content-type: application/json
Content-length: 126

{
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="633ee-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="633ee-143">Response</span></span>
<span data-ttu-id="633ee-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="633ee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 230

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "0a129715-9715-0a12-1597-120a1597120a",
  "version": "Version value"
}
```








