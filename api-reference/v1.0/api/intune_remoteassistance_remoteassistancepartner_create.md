# <a name="create-remoteassistancepartner"></a><span data-ttu-id="6ce7d-101">Criar remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="6ce7d-101">Create remoteAssistancePartner</span></span>

> <span data-ttu-id="6ce7d-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6ce7d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6ce7d-103">Criar um novo objeto [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="6ce7d-103">Create a new [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6ce7d-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6ce7d-104">Prerequisites</span></span>
<span data-ttu-id="6ce7d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6ce7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6ce7d-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ce7d-107">Permission type</span></span>|<span data-ttu-id="6ce7d-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6ce7d-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ce7d-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ce7d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6ce7d-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ce7d-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6ce7d-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ce7d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ce7d-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ce7d-112">Not supported.</span></span>|
|<span data-ttu-id="6ce7d-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ce7d-113">Application</span></span>|<span data-ttu-id="6ce7d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ce7d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ce7d-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ce7d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="6ce7d-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6ce7d-116">Request headers</span></span>
|<span data-ttu-id="6ce7d-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6ce7d-117">Header</span></span>|<span data-ttu-id="6ce7d-118">Valor</span><span class="sxs-lookup"><span data-stu-id="6ce7d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ce7d-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="6ce7d-119">Authorization</span></span>|<span data-ttu-id="6ce7d-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ce7d-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ce7d-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6ce7d-121">Accept</span></span>|<span data-ttu-id="6ce7d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6ce7d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ce7d-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6ce7d-123">Request body</span></span>
<span data-ttu-id="6ce7d-124">No corpo da solicitação, forneça uma representação JSON do objeto remoteAssistancePartner.</span><span class="sxs-lookup"><span data-stu-id="6ce7d-124">In the request body, supply a JSON representation for the remoteAssistancePartner object.</span></span>

<span data-ttu-id="6ce7d-125">A tabela a seguir mostra as propriedades que são necessárias ao criar remoteAssistancePartner.</span><span class="sxs-lookup"><span data-stu-id="6ce7d-125">The following table shows the properties that are required when you create the remoteAssistancePartner.</span></span>

|<span data-ttu-id="6ce7d-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6ce7d-126">Property</span></span>|<span data-ttu-id="6ce7d-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ce7d-127">Type</span></span>|<span data-ttu-id="6ce7d-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ce7d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ce7d-129">id</span><span class="sxs-lookup"><span data-stu-id="6ce7d-129">id</span></span>|<span data-ttu-id="6ce7d-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6ce7d-130">String</span></span>|<span data-ttu-id="6ce7d-131">O identificador exclusivo do parceiro.</span><span class="sxs-lookup"><span data-stu-id="6ce7d-131">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="6ce7d-132">displayName</span><span class="sxs-lookup"><span data-stu-id="6ce7d-132">displayName</span></span>|<span data-ttu-id="6ce7d-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6ce7d-133">String</span></span>|<span data-ttu-id="6ce7d-134">Nome de exibição do parceiro.</span><span class="sxs-lookup"><span data-stu-id="6ce7d-134">Display name of the partner.</span></span>|
|<span data-ttu-id="6ce7d-135">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="6ce7d-135">onboardingUrl</span></span>|<span data-ttu-id="6ce7d-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6ce7d-136">String</span></span>|<span data-ttu-id="6ce7d-137">URL do portal de integração do parceiro, no qual um administrador pode configurar o serviço de assistência remota.</span><span class="sxs-lookup"><span data-stu-id="6ce7d-137">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="6ce7d-138">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="6ce7d-138">onboardingStatus</span></span>|[<span data-ttu-id="6ce7d-139">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="6ce7d-139">remoteAssistanceOnboardingStatus</span></span>](../resources/intune_remoteassistance_remoteassistanceonboardingstatus.md)|<span data-ttu-id="6ce7d-140">TBD.</span><span class="sxs-lookup"><span data-stu-id="6ce7d-140">TBD.</span></span> <span data-ttu-id="6ce7d-141">Os valores possíveis são: `notOnboarded`, `onboarding`, `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="6ce7d-141">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="6ce7d-142">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="6ce7d-142">lastConnectionDateTime</span></span>|<span data-ttu-id="6ce7d-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ce7d-143">DateTimeOffset</span></span>|<span data-ttu-id="6ce7d-144">Carimbo de data/hora da última solicitação enviada ao Intune pelo parceiro TEM.</span><span class="sxs-lookup"><span data-stu-id="6ce7d-144">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="6ce7d-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ce7d-145">Response</span></span>
<span data-ttu-id="6ce7d-146">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ce7d-146">If successful, this method returns a `201 Created` response code and a [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ce7d-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6ce7d-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="6ce7d-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ce7d-148">Request</span></span>
<span data-ttu-id="6ce7d-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6ce7d-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners
Content-type: application/json
Content-length: 266

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="6ce7d-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ce7d-150">Response</span></span>
<span data-ttu-id="6ce7d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6ce7d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 315

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "7443c8b9-c8b9-7443-b9c8-4374b9c84374",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```



