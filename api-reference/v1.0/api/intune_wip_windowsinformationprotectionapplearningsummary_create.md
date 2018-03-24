# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="78a64-101">Criar windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="78a64-101">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="78a64-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="78a64-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="78a64-103">Criar um novo objeto [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="78a64-103">Create a new [plannerBucket](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="78a64-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="78a64-104">Prerequisites</span></span>
<span data-ttu-id="78a64-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="78a64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="78a64-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78a64-107">Permission type</span></span>|<span data-ttu-id="78a64-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="78a64-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78a64-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78a64-109">Delegated (work or school account)</span></span>|<span data-ttu-id="78a64-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78a64-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="78a64-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78a64-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78a64-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78a64-112">Not supported.</span></span>|
|<span data-ttu-id="78a64-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78a64-113">Application</span></span>|<span data-ttu-id="78a64-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78a64-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="78a64-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78a64-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="78a64-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78a64-116">Request headers</span></span>
|<span data-ttu-id="78a64-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="78a64-117">Header</span></span>|<span data-ttu-id="78a64-118">Valor</span><span class="sxs-lookup"><span data-stu-id="78a64-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78a64-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="78a64-119">Authorization</span></span>|<span data-ttu-id="78a64-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78a64-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="78a64-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="78a64-121">Accept</span></span>|<span data-ttu-id="78a64-122">application/json</span><span class="sxs-lookup"><span data-stu-id="78a64-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78a64-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78a64-123">Request body</span></span>
<span data-ttu-id="78a64-124">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="78a64-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="78a64-125">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="78a64-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="78a64-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="78a64-126">Property</span></span>|<span data-ttu-id="78a64-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="78a64-127">Type</span></span>|<span data-ttu-id="78a64-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="78a64-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78a64-129">id</span><span class="sxs-lookup"><span data-stu-id="78a64-129">id</span></span>|<span data-ttu-id="78a64-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="78a64-130">String</span></span>|<span data-ttu-id="78a64-131">Identificador exclusivo do WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="78a64-131">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="78a64-132">applicationName</span><span class="sxs-lookup"><span data-stu-id="78a64-132">applicationName</span></span>|<span data-ttu-id="78a64-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="78a64-133">String</span></span>|<span data-ttu-id="78a64-134">Nome do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78a64-134">Application Name</span></span>|
|<span data-ttu-id="78a64-135">applicationType</span><span class="sxs-lookup"><span data-stu-id="78a64-135">applicationType</span></span>|<span data-ttu-id="78a64-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="78a64-136">String</span></span>|<span data-ttu-id="78a64-137">Tipo de aplicativo Os valores possíveis são: `universal`, `desktop`.</span><span class="sxs-lookup"><span data-stu-id="78a64-137">Application Type Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="78a64-138">deviceCount</span><span class="sxs-lookup"><span data-stu-id="78a64-138">deviceCount</span></span>|<span data-ttu-id="78a64-139">Int32</span><span class="sxs-lookup"><span data-stu-id="78a64-139">Int32</span></span>|<span data-ttu-id="78a64-140">Contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="78a64-140">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="78a64-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="78a64-141">Response</span></span>
<span data-ttu-id="78a64-142">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78a64-142">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78a64-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78a64-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="78a64-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78a64-144">Request</span></span>
<span data-ttu-id="78a64-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="78a64-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="78a64-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="78a64-146">Response</span></span>
<span data-ttu-id="78a64-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="78a64-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 240

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "id": "063baf50-af50-063b-50af-3b0650af3b06",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```



