# <a name="update-remoteassistancepartner"></a><span data-ttu-id="01a61-101">Atualizar remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="01a61-101">Update remoteAssistancePartner</span></span>

> <span data-ttu-id="01a61-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="01a61-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="01a61-103">Atualizar as propriedades de um objeto [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="01a61-103">Update the properties of a [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="01a61-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="01a61-104">Prerequisites</span></span>
<span data-ttu-id="01a61-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="01a61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="01a61-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01a61-107">Permission type</span></span>|<span data-ttu-id="01a61-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="01a61-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01a61-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01a61-109">Delegated (work or school account)</span></span>|<span data-ttu-id="01a61-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01a61-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="01a61-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01a61-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01a61-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01a61-112">Not supported.</span></span>|
|<span data-ttu-id="01a61-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01a61-113">Application</span></span>|<span data-ttu-id="01a61-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01a61-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01a61-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01a61-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="01a61-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01a61-116">Request headers</span></span>
|<span data-ttu-id="01a61-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="01a61-117">Header</span></span>|<span data-ttu-id="01a61-118">Valor</span><span class="sxs-lookup"><span data-stu-id="01a61-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01a61-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="01a61-119">Authorization</span></span>|<span data-ttu-id="01a61-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01a61-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01a61-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="01a61-121">Accept</span></span>|<span data-ttu-id="01a61-122">application/json</span><span class="sxs-lookup"><span data-stu-id="01a61-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01a61-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01a61-123">Request body</span></span>
<span data-ttu-id="01a61-124">No corpo da solicitação, forneça uma representação JSON do objeto [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="01a61-124">In the request body, supply a JSON representation for the [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) object.</span></span>

<span data-ttu-id="01a61-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="01a61-125">The following table shows the properties that are required when you create the [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md).</span></span>

|<span data-ttu-id="01a61-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01a61-126">Property</span></span>|<span data-ttu-id="01a61-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="01a61-127">Type</span></span>|<span data-ttu-id="01a61-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="01a61-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01a61-129">id</span><span class="sxs-lookup"><span data-stu-id="01a61-129">id</span></span>|<span data-ttu-id="01a61-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="01a61-130">String</span></span>|<span data-ttu-id="01a61-131">O identificador exclusivo do parceiro.</span><span class="sxs-lookup"><span data-stu-id="01a61-131">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="01a61-132">displayName</span><span class="sxs-lookup"><span data-stu-id="01a61-132">displayName</span></span>|<span data-ttu-id="01a61-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="01a61-133">String</span></span>|<span data-ttu-id="01a61-134">Nome de exibição do parceiro.</span><span class="sxs-lookup"><span data-stu-id="01a61-134">Display name of the partner.</span></span>|
|<span data-ttu-id="01a61-135">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="01a61-135">onboardingUrl</span></span>|<span data-ttu-id="01a61-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="01a61-136">String</span></span>|<span data-ttu-id="01a61-137">URL do portal de integração do parceiro, no qual um administrador pode configurar o serviço de assistência remota.</span><span class="sxs-lookup"><span data-stu-id="01a61-137">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="01a61-138">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="01a61-138">onboardingStatus</span></span>|[<span data-ttu-id="01a61-139">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="01a61-139">remoteAssistanceOnboardingStatus</span></span>](../resources/intune_remoteassistance_remoteassistanceonboardingstatus.md)|<span data-ttu-id="01a61-140">TBD.</span><span class="sxs-lookup"><span data-stu-id="01a61-140">TBD.</span></span> <span data-ttu-id="01a61-141">Os valores possíveis são: `notOnboarded`, `onboarding`, `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="01a61-141">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="01a61-142">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="01a61-142">lastConnectionDateTime</span></span>|<span data-ttu-id="01a61-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01a61-143">DateTimeOffset</span></span>|<span data-ttu-id="01a61-144">Carimbo de data/hora da última solicitação enviada ao Intune pelo parceiro TEM.</span><span class="sxs-lookup"><span data-stu-id="01a61-144">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="01a61-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="01a61-145">Response</span></span>
<span data-ttu-id="01a61-146">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01a61-146">If successful, this method returns a `200 OK` response code and an updated [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01a61-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01a61-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="01a61-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01a61-148">Request</span></span>
<span data-ttu-id="01a61-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="01a61-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
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

### <a name="response"></a><span data-ttu-id="01a61-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="01a61-150">Response</span></span>
<span data-ttu-id="01a61-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01a61-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



