# <a name="update-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="296f5-101">Atualizar windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="296f5-101">Update windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="296f5-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="296f5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="296f5-103">Atualizar as propriedades de um objeto [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="296f5-103">Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="296f5-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="296f5-104">Prerequisites</span></span>
<span data-ttu-id="296f5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="296f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="296f5-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="296f5-107">Permission type</span></span>|<span data-ttu-id="296f5-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="296f5-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="296f5-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="296f5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="296f5-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="296f5-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="296f5-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="296f5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="296f5-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="296f5-112">Not supported.</span></span>|
|<span data-ttu-id="296f5-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="296f5-113">Application</span></span>|<span data-ttu-id="296f5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="296f5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="296f5-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="296f5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="296f5-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="296f5-116">Request headers</span></span>
|<span data-ttu-id="296f5-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="296f5-117">Header</span></span>|<span data-ttu-id="296f5-118">Valor</span><span class="sxs-lookup"><span data-stu-id="296f5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="296f5-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="296f5-119">Authorization</span></span>|<span data-ttu-id="296f5-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="296f5-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="296f5-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="296f5-121">Accept</span></span>|<span data-ttu-id="296f5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="296f5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="296f5-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="296f5-123">Request body</span></span>
<span data-ttu-id="296f5-124">No corpo da solicitação, forneça uma representação JSON do objeto [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="296f5-124">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) object.</span></span>

<span data-ttu-id="296f5-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="296f5-125">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md).</span></span>

|<span data-ttu-id="296f5-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="296f5-126">Property</span></span>|<span data-ttu-id="296f5-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="296f5-127">Type</span></span>|<span data-ttu-id="296f5-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="296f5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="296f5-129">id</span><span class="sxs-lookup"><span data-stu-id="296f5-129">id</span></span>|<span data-ttu-id="296f5-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="296f5-130">String</span></span>|<span data-ttu-id="296f5-131">Identificador exclusivo do WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="296f5-131">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="296f5-132">applicationName</span><span class="sxs-lookup"><span data-stu-id="296f5-132">applicationName</span></span>|<span data-ttu-id="296f5-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="296f5-133">String</span></span>|<span data-ttu-id="296f5-134">Nome do Aplicativo</span><span class="sxs-lookup"><span data-stu-id="296f5-134">Application Name</span></span>|
|<span data-ttu-id="296f5-135">applicationType</span><span class="sxs-lookup"><span data-stu-id="296f5-135">applicationType</span></span>|[<span data-ttu-id="296f5-136">applicationType</span><span class="sxs-lookup"><span data-stu-id="296f5-136">applicationType</span></span>](../resources/intune_wip_applicationtype.md)|<span data-ttu-id="296f5-p102">|||UNTRANSLATED_CONTENT_START|||Application Type. Possible values are: `universal`, `desktop`.|||UNTRANSLATED_CONTENT_END|||</span><span class="sxs-lookup"><span data-stu-id="296f5-p102">Application Type Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="296f5-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="296f5-139">deviceCount</span></span>|<span data-ttu-id="296f5-140">Int32</span><span class="sxs-lookup"><span data-stu-id="296f5-140">Int32</span></span>|<span data-ttu-id="296f5-141">Contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="296f5-141">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="296f5-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="296f5-142">Response</span></span>
<span data-ttu-id="296f5-143">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="296f5-143">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="296f5-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="296f5-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="296f5-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="296f5-145">Request</span></span>
<span data-ttu-id="296f5-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="296f5-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
Content-type: application/json
Content-length: 106

{
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="296f5-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="296f5-147">Response</span></span>
<span data-ttu-id="296f5-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="296f5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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








