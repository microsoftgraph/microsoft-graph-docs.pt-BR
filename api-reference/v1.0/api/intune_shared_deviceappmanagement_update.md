# <a name="update-deviceappmanagement"></a><span data-ttu-id="c02ac-101">Atualizar deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="c02ac-101">Update deviceAppManagement</span></span>

> <span data-ttu-id="c02ac-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c02ac-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c02ac-103">Atualizar as propriedades de um objeto de [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="c02ac-103">Update the properties of a [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c02ac-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c02ac-104">Prerequisites</span></span>
<span data-ttu-id="c02ac-105">Uma das seguintes permissões é necessário chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="c02ac-105">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c02ac-106">Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c02ac-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="c02ac-107">Observe que a permissão apropriada varia de acordo com o fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="c02ac-107">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="c02ac-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c02ac-108">Permission type</span></span>|<span data-ttu-id="c02ac-109">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c02ac-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c02ac-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c02ac-110">Delegated (work or school account)</span></span>|<span data-ttu-id="c02ac-111">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c02ac-111">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c02ac-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c02ac-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c02ac-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c02ac-113">Not supported.</span></span>|
|<span data-ttu-id="c02ac-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c02ac-114">Application</span></span>|<span data-ttu-id="c02ac-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c02ac-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c02ac-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c02ac-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="c02ac-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c02ac-117">Request headers</span></span>
|<span data-ttu-id="c02ac-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c02ac-118">Header</span></span>|<span data-ttu-id="c02ac-119">Valor</span><span class="sxs-lookup"><span data-stu-id="c02ac-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c02ac-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c02ac-120">Authorization</span></span>|<span data-ttu-id="c02ac-121">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c02ac-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c02ac-122">Accept</span><span class="sxs-lookup"><span data-stu-id="c02ac-122">Accept</span></span>|<span data-ttu-id="c02ac-123">application/json</span><span class="sxs-lookup"><span data-stu-id="c02ac-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c02ac-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c02ac-124">Request body</span></span>
<span data-ttu-id="c02ac-125">No corpo da solicitação, forneça uma representação JSON do objeto [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="c02ac-125">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object.</span></span>

<span data-ttu-id="c02ac-126">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="c02ac-126">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md).</span></span>

|<span data-ttu-id="c02ac-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c02ac-127">Property</span></span>|<span data-ttu-id="c02ac-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="c02ac-128">Type</span></span>|<span data-ttu-id="c02ac-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="c02ac-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c02ac-130">id</span><span class="sxs-lookup"><span data-stu-id="c02ac-130">id</span></span>|<span data-ttu-id="c02ac-131">String</span><span class="sxs-lookup"><span data-stu-id="c02ac-131">String</span></span>|<span data-ttu-id="c02ac-132">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c02ac-132">Key of the entity.</span></span>|
|<span data-ttu-id="c02ac-133">**Inclusão**</span><span class="sxs-lookup"><span data-stu-id="c02ac-133">**Onboarding**</span></span>|
|<span data-ttu-id="c02ac-134">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="c02ac-134">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="c02ac-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="c02ac-135">Boolean</span></span>|<span data-ttu-id="c02ac-136">Se a conta está ativada para sincronizar aplicativos do Microsoft Store para Empresa.</span><span class="sxs-lookup"><span data-stu-id="c02ac-136">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="c02ac-137">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="c02ac-137">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="c02ac-138">String</span><span class="sxs-lookup"><span data-stu-id="c02ac-138">String</span></span>|<span data-ttu-id="c02ac-139">As informações sobre a localidade usada para sincronizar aplicativos do Microsoft Store para Empresas.</span><span class="sxs-lookup"><span data-stu-id="c02ac-139">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="c02ac-140">Culturas específicas de um país/região.</span><span class="sxs-lookup"><span data-stu-id="c02ac-140">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="c02ac-141">Os nomes dessas culturas seguem a RFC 4646 (Windows Vista e mais recentes).</span><span class="sxs-lookup"><span data-stu-id="c02ac-141">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="c02ac-142">O formato é <languagecode2>-<country/regioncode2>, onde <languagecode2> é um código em duas letras minúsculas derivado da ISO 639-1 e <country/regioncode2> é um código em duas letras maiúsculas derivado da ISO 3166.</span><span class="sxs-lookup"><span data-stu-id="c02ac-142">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="c02ac-143">Por exemplo, en-US para inglês (Estados Unidos) é uma cultura específica.</span><span class="sxs-lookup"><span data-stu-id="c02ac-143">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="c02ac-144">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="c02ac-144">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="c02ac-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c02ac-145">DateTimeOffset</span></span>|<span data-ttu-id="c02ac-146">A última vez em uma sincronização de aplicativo na Microsoft Store para Empresas foi concluída.</span><span class="sxs-lookup"><span data-stu-id="c02ac-146">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="c02ac-147">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="c02ac-147">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="c02ac-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c02ac-148">DateTimeOffset</span></span>|<span data-ttu-id="c02ac-149">A última vez que os aplicativos da Microsoft Store para Empresas foram sincronizados com êxito para essa conta.</span><span class="sxs-lookup"><span data-stu-id="c02ac-149">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|

## <a name="response"></a><span data-ttu-id="c02ac-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="c02ac-150">Response</span></span>
<span data-ttu-id="c02ac-151">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c02ac-151">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="c02ac-152">Exemplo de solicitação</span><span class="sxs-lookup"><span data-stu-id="c02ac-152">Example request</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

## <a name="example-response"></a><span data-ttu-id="c02ac-153">Resposta de exemplo</span><span class="sxs-lookup"><span data-stu-id="c02ac-153">Example response</span></span>

<span data-ttu-id="c02ac-154">No objeto response mostrado aqui pode estar truncado para fins de concisão.</span><span class="sxs-lookup"><span data-stu-id="c02ac-154">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c02ac-155">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c02ac-155">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```



