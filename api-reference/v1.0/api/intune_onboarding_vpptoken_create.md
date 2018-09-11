# <a name="create-vpptoken"></a><span data-ttu-id="264f8-101">Criar vppToken</span><span class="sxs-lookup"><span data-stu-id="264f8-101">Create vppToken</span></span>

> <span data-ttu-id="264f8-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="264f8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="264f8-103">Criar um novo objeto [vppToken](../resources/intune_onboarding_vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="264f8-103">Create a new [vppToken](../resources/intune_onboarding_vpptoken.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="264f8-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="264f8-104">Prerequisites</span></span>
<span data-ttu-id="264f8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="264f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="264f8-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="264f8-107">Permission type</span></span>|<span data-ttu-id="264f8-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="264f8-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="264f8-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="264f8-109">Delegated (work or school account)</span></span>|<span data-ttu-id="264f8-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="264f8-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="264f8-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="264f8-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="264f8-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="264f8-112">Not supported.</span></span>|
|<span data-ttu-id="264f8-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="264f8-113">Application</span></span>|<span data-ttu-id="264f8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="264f8-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="264f8-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="264f8-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a><span data-ttu-id="264f8-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="264f8-116">Request headers</span></span>
|<span data-ttu-id="264f8-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="264f8-117">Header</span></span>|<span data-ttu-id="264f8-118">Valor</span><span class="sxs-lookup"><span data-stu-id="264f8-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="264f8-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="264f8-119">Authorization</span></span>|<span data-ttu-id="264f8-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="264f8-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="264f8-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="264f8-121">Accept</span></span>|<span data-ttu-id="264f8-122">application/json</span><span class="sxs-lookup"><span data-stu-id="264f8-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="264f8-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="264f8-123">Request body</span></span>
<span data-ttu-id="264f8-124">No corpo da solicitação, forneça uma representação JSON do objeto vppToken.</span><span class="sxs-lookup"><span data-stu-id="264f8-124">In the request body, supply a JSON representation for the vppToken object.</span></span>

<span data-ttu-id="264f8-125">A tabela a seguir mostra as propriedades que são necessárias ao criar o vppToken.</span><span class="sxs-lookup"><span data-stu-id="264f8-125">The following table shows the properties that are required when you create the vppToken.</span></span>

|<span data-ttu-id="264f8-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="264f8-126">Property</span></span>|<span data-ttu-id="264f8-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="264f8-127">Type</span></span>|<span data-ttu-id="264f8-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="264f8-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="264f8-129">id</span><span class="sxs-lookup"><span data-stu-id="264f8-129">id</span></span>|<span data-ttu-id="264f8-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="264f8-130">String</span></span>|<span data-ttu-id="264f8-131">Isso é gerado automaticamente quando o appleVolumePurchaseProgramToken é criado.</span><span class="sxs-lookup"><span data-stu-id="264f8-131">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="264f8-132">É a Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="264f8-132">It is the Key of the entity.</span></span>|
|<span data-ttu-id="264f8-133">organizationName</span><span class="sxs-lookup"><span data-stu-id="264f8-133">organizationName</span></span>|<span data-ttu-id="264f8-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="264f8-134">String</span></span>|<span data-ttu-id="264f8-135">A organização associada ao Token do Programa de Compra por Volume da Apple</span><span class="sxs-lookup"><span data-stu-id="264f8-135">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="264f8-136">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="264f8-136">vppTokenAccountType</span></span>|[<span data-ttu-id="264f8-137">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="264f8-137">vppTokenAccountType</span></span>](../resources/intune_shared_vpptokenaccounttype.md)|<span data-ttu-id="264f8-p103">|||UNTRANSLATED_CONTENT_START|||The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with. Possible values are: `business`, `education`. Possible values are: `business`, `education`.|||UNTRANSLATED_CONTENT_END|||</span><span class="sxs-lookup"><span data-stu-id="264f8-p103">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with. The possible values are: `business`, `education`. The possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="264f8-141">appleId</span><span class="sxs-lookup"><span data-stu-id="264f8-141">appleId</span></span>|<span data-ttu-id="264f8-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="264f8-142">String</span></span>|<span data-ttu-id="264f8-143">O Apple ID associado ao Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="264f8-143">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="264f8-144">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="264f8-144">expirationDateTime</span></span>|<span data-ttu-id="264f8-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="264f8-145">DateTimeOffset</span></span>|<span data-ttu-id="264f8-146">A data e hora de expiração do Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="264f8-146">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="264f8-147">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="264f8-147">lastSyncDateTime</span></span>|<span data-ttu-id="264f8-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="264f8-148">DateTimeOffset</span></span>|<span data-ttu-id="264f8-149">A última vez que uma sincronização de aplicativo foi realizada com o serviço do Apple Volume Purchase Program usando Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="264f8-149">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="264f8-150">token</span><span class="sxs-lookup"><span data-stu-id="264f8-150">token</span></span>|<span data-ttu-id="264f8-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="264f8-151">String</span></span>|<span data-ttu-id="264f8-152">A cadeia de caracteres do Token do Apple Volume Purchase Program baixada do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="264f8-152">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="264f8-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="264f8-153">lastModifiedDateTime</span></span>|<span data-ttu-id="264f8-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="264f8-154">DateTimeOffset</span></span>|<span data-ttu-id="264f8-155">Data e hora da última modificação associada com o Token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="264f8-155">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="264f8-156">state</span><span class="sxs-lookup"><span data-stu-id="264f8-156">state</span></span>|[<span data-ttu-id="264f8-157">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="264f8-157">vppTokenState</span></span>](../resources/intune_onboarding_vpptokenstate.md)|<span data-ttu-id="264f8-p104">Estado atual do token do Programa de Compra de Volume da Apple. Os valores possíveis são: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`. Os valores possíveis são: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="264f8-p104">Current state of the Apple Volume Purchase Program Token. The possible values are: `unknown`, `valid`, `expired`, `invalid`. The possible values are: `assignedToExternalMDM`, `unknown`, `valid`, `expired`.</span></span>|
|<span data-ttu-id="264f8-161">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="264f8-161">lastSyncStatus</span></span>|[<span data-ttu-id="264f8-162">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="264f8-162">vppTokenSyncStatus</span></span>](../resources/intune_onboarding_vpptokensyncstatus.md)|<span data-ttu-id="264f8-p105">Status de sincronização atual da última sincronização de aplicativo que foi disparada usando o token do Programa de Compra de Volume da Apple. Os valores possíveis são: `none`, `inProgress`, `completed`, `failed`. Os valores possíveis são: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="264f8-p105">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token. The possible values are: `none`, `inProgress`, `completed`, `failed`. The possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="264f8-166">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="264f8-166">automaticallyUpdateApps</span></span>|<span data-ttu-id="264f8-167">Booleano</span><span class="sxs-lookup"><span data-stu-id="264f8-167">Boolean</span></span>|<span data-ttu-id="264f8-168">Se os aplicativos para o token VPP serão automaticamente atualizados ou não.</span><span class="sxs-lookup"><span data-stu-id="264f8-168">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="264f8-169">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="264f8-169">countryOrRegion</span></span>|<span data-ttu-id="264f8-170">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="264f8-170">String</span></span>|<span data-ttu-id="264f8-171">Se os aplicativos para o token VPP serão automaticamente atualizados ou não.</span><span class="sxs-lookup"><span data-stu-id="264f8-171">Whether or not apps for the VPP token will be automatically updated.</span></span>|



## <a name="response"></a><span data-ttu-id="264f8-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="264f8-172">Response</span></span>
<span data-ttu-id="264f8-173">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [vppToken](../resources/intune_onboarding_vpptoken.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="264f8-173">If successful, this method returns a `201 Created` response code and a [vppToken](../resources/intune_onboarding_vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="264f8-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="264f8-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="264f8-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="264f8-175">Request</span></span>
<span data-ttu-id="264f8-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="264f8-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens
Content-type: application/json
Content-length: 525

{
  "@odata.type": "#microsoft.graph.vppToken",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "valid",
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value"
}
```

### <a name="response"></a><span data-ttu-id="264f8-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="264f8-177">Response</span></span>
<span data-ttu-id="264f8-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="264f8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 574

{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "9ceb2f92-2f92-9ceb-922f-eb9c922feb9c",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "valid",
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value"
}
```








