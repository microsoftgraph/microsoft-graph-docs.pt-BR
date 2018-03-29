# <a name="update-deviceappmanagement"></a><span data-ttu-id="d995d-101">Atualizar deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="d995d-101">Update deviceAppManagement</span></span>

> <span data-ttu-id="d995d-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d995d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d995d-103">Atualizar as propriedades de um objeto de [deviceAppManagement](../resources/intune_onboarding_deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="d995d-103">Update the properties of a [calendar](../resources/intune_onboarding_deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d995d-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d995d-104">Prerequisites</span></span>
<span data-ttu-id="d995d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d995d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d995d-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d995d-107">Permission type</span></span>|<span data-ttu-id="d995d-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d995d-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d995d-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d995d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d995d-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d995d-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d995d-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d995d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d995d-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d995d-112">Not supported.</span></span>|
|<span data-ttu-id="d995d-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d995d-113">Application</span></span>|<span data-ttu-id="d995d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d995d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d995d-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d995d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="d995d-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d995d-116">Request headers</span></span>
|<span data-ttu-id="d995d-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d995d-117">Header</span></span>|<span data-ttu-id="d995d-118">Valor</span><span class="sxs-lookup"><span data-stu-id="d995d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d995d-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="d995d-119">Authorization</span></span>|<span data-ttu-id="d995d-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d995d-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d995d-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d995d-121">Accept</span></span>|<span data-ttu-id="d995d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d995d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d995d-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d995d-123">Request body</span></span>
<span data-ttu-id="d995d-124">No corpo da solicitação, forneça uma representação JSON do objeto [deviceAppManagement](../resources/intune_onboarding_deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="d995d-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_onboarding_deviceappmanagement.md) object.</span></span>

<span data-ttu-id="d995d-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceAppManagement](../resources/intune_onboarding_deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="d995d-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="d995d-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d995d-126">Property</span></span>|<span data-ttu-id="d995d-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="d995d-127">Type</span></span>|<span data-ttu-id="d995d-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="d995d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d995d-129">id</span><span class="sxs-lookup"><span data-stu-id="d995d-129">id</span></span>|<span data-ttu-id="d995d-130">String</span><span class="sxs-lookup"><span data-stu-id="d995d-130">String</span></span>|<span data-ttu-id="d995d-131">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d995d-131">Not yet documented</span></span>|
|<span data-ttu-id="d995d-132">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d995d-132">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="d995d-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d995d-133">DateTimeOffset</span></span>|<span data-ttu-id="d995d-134">A última vez que os aplicativos da Microsoft Store para Empresas foram sincronizados com êxito para essa conta.</span><span class="sxs-lookup"><span data-stu-id="d995d-134">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|
|<span data-ttu-id="d995d-135">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="d995d-135">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="d995d-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="d995d-136">Boolean</span></span>|<span data-ttu-id="d995d-137">Se a conta está ativada para sincronizar aplicativos do Microsoft Store para Empresa.</span><span class="sxs-lookup"><span data-stu-id="d995d-137">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="d995d-138">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="d995d-138">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="d995d-139">String</span><span class="sxs-lookup"><span data-stu-id="d995d-139">String</span></span>|<span data-ttu-id="d995d-140">As informações sobre a localidade usada para sincronizar aplicativos do Microsoft Store para Empresas.</span><span class="sxs-lookup"><span data-stu-id="d995d-140">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="d995d-141">Culturas específicas de um país/região.</span><span class="sxs-lookup"><span data-stu-id="d995d-141">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="d995d-142">Os nomes dessas culturas seguem a RFC 4646 (Windows Vista e mais recentes).</span><span class="sxs-lookup"><span data-stu-id="d995d-142">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="d995d-143">O formato é <languagecode2>-<country/regioncode2>, onde <languagecode2> é um código em duas letras minúsculas derivado da ISO 639-1 e <country/regioncode2> é um código em duas letras maiúsculas derivado da ISO 3166.</span><span class="sxs-lookup"><span data-stu-id="d995d-143">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="d995d-144">Por exemplo, en-US para inglês (Estados Unidos) é uma cultura específica.</span><span class="sxs-lookup"><span data-stu-id="d995d-144">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="d995d-145">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="d995d-145">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="d995d-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d995d-146">DateTimeOffset</span></span>|<span data-ttu-id="d995d-147">A última vez em uma sincronização de aplicativo na Microsoft Store para Empresas foi concluída.</span><span class="sxs-lookup"><span data-stu-id="d995d-147">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|



## <a name="response"></a><span data-ttu-id="d995d-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="d995d-148">Response</span></span>
<span data-ttu-id="d995d-149">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [deviceAppManagement](../resources/intune_onboarding_deviceappmanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d995d-149">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_onboarding_deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d995d-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d995d-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="d995d-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d995d-151">Request</span></span>
<span data-ttu-id="d995d-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d995d-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 336

{
  "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "2016-12-31T23:57:45.2453148-08:00",
  "isEnabledForMicrosoftStoreForBusiness": true,
  "microsoftStoreForBusinessLanguage": "Microsoft Store For Business Language value",
  "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "2017-01-01T00:02:00.0421137-08:00"
}
```

### <a name="response"></a><span data-ttu-id="d995d-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="d995d-153">Response</span></span>
<span data-ttu-id="d995d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d995d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 443

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb",
  "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "2016-12-31T23:57:45.2453148-08:00",
  "isEnabledForMicrosoftStoreForBusiness": true,
  "microsoftStoreForBusinessLanguage": "Microsoft Store For Business Language value",
  "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "2017-01-01T00:02:00.0421137-08:00"
}
```



