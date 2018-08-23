# <a name="update-deviceappmanagement"></a><span data-ttu-id="2d10b-101">Atualizar deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="2d10b-101">Update deviceAppManagement</span></span>

> <span data-ttu-id="2d10b-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2d10b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2d10b-103">Atualizar as propriedades de um objeto de [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="2d10b-103">Update the properties of a [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2d10b-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2d10b-104">Prerequisites</span></span>
<span data-ttu-id="2d10b-105">Uma das seguintes permissões é necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="2d10b-105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see Permissions.</span></span> <span data-ttu-id="2d10b-106">Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2d10b-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="2d10b-107">Observe que a permissão apropriada varia de acordo com o fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="2d10b-107">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="2d10b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2d10b-108">Permission type</span></span>|<span data-ttu-id="2d10b-109">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2d10b-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d10b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2d10b-110">Delegated (work or school account)</span></span>|<span data-ttu-id="2d10b-111">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d10b-111">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2d10b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2d10b-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d10b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d10b-113">Not supported.</span></span>|
|<span data-ttu-id="2d10b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2d10b-114">Application</span></span>|<span data-ttu-id="2d10b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d10b-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d10b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2d10b-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="2d10b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2d10b-117">Request headers</span></span>
|<span data-ttu-id="2d10b-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2d10b-118">Header</span></span>|<span data-ttu-id="2d10b-119">Valor</span><span class="sxs-lookup"><span data-stu-id="2d10b-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d10b-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="2d10b-120">Authorization</span></span>|<span data-ttu-id="2d10b-121">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="2d10b-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d10b-122">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2d10b-122">Accept</span></span>|<span data-ttu-id="2d10b-123">application/json</span><span class="sxs-lookup"><span data-stu-id="2d10b-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d10b-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2d10b-124">Request body</span></span>
<span data-ttu-id="2d10b-125">No corpo da solicitação, forneça uma representação JSON do objeto [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="2d10b-125">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object.</span></span>

<span data-ttu-id="2d10b-126">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="2d10b-126">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md).</span></span>

|<span data-ttu-id="2d10b-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d10b-127">Property</span></span>|<span data-ttu-id="2d10b-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d10b-128">Type</span></span>|<span data-ttu-id="2d10b-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d10b-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d10b-130">id</span><span class="sxs-lookup"><span data-stu-id="2d10b-130">id</span></span>|<span data-ttu-id="2d10b-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d10b-131">String</span></span>|<span data-ttu-id="2d10b-132">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2d10b-132">Key of the entity.</span></span>|
|<span data-ttu-id="2d10b-133">**Nível de contratação**</span><span class="sxs-lookup"><span data-stu-id="2d10b-133">**On-boarding**</span></span>|
|<span data-ttu-id="2d10b-134">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="2d10b-134">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="2d10b-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d10b-135">Boolean</span></span>|<span data-ttu-id="2d10b-136">Se a conta está ativada para sincronizar aplicativos do Microsoft Store para Empresa.</span><span class="sxs-lookup"><span data-stu-id="2d10b-136">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="2d10b-137">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="2d10b-137">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="2d10b-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d10b-138">String</span></span>|<span data-ttu-id="2d10b-139">As informações sobre a localidade usada para sincronizar aplicativos do Microsoft Store para Empresas.</span><span class="sxs-lookup"><span data-stu-id="2d10b-139">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="2d10b-140">Culturas específicas de um país/região.</span><span class="sxs-lookup"><span data-stu-id="2d10b-140">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="2d10b-141">Os nomes dessas culturas seguem a RFC 4646 (Windows Vista e mais recentes).</span><span class="sxs-lookup"><span data-stu-id="2d10b-141">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="2d10b-142">O formato é <languagecode2>-<country/regioncode2>, onde <languagecode2> é um código em duas letras minúsculas derivado da ISO 639-1 e <country/regioncode2> é um código em duas letras maiúsculas derivado da ISO 3166.</span><span class="sxs-lookup"><span data-stu-id="2d10b-142">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="2d10b-143">Por exemplo, en-US para inglês (Estados Unidos) é uma cultura específica.</span><span class="sxs-lookup"><span data-stu-id="2d10b-143">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="2d10b-144">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="2d10b-144">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="2d10b-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d10b-145">DateTimeOffset</span></span>|<span data-ttu-id="2d10b-146">A última vez em que uma sincronização de aplicativo na Microsoft Store para Empresas foi concluída.</span><span class="sxs-lookup"><span data-stu-id="2d10b-146">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="2d10b-147">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="2d10b-147">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="2d10b-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d10b-148">DateTimeOffset</span></span>|<span data-ttu-id="2d10b-149">A última vez que os aplicativos da Microsoft Store para Empresas foram sincronizados com êxito para essa conta.</span><span class="sxs-lookup"><span data-stu-id="2d10b-149">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|

## <a name="response"></a><span data-ttu-id="2d10b-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d10b-150">Response</span></span>
<span data-ttu-id="2d10b-151">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2d10b-151">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d10b-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2d10b-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="2d10b-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d10b-153">Request</span></span>
<span data-ttu-id="2d10b-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d10b-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="2d10b-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d10b-155">Response</span></span>
<span data-ttu-id="2d10b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2d10b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```



