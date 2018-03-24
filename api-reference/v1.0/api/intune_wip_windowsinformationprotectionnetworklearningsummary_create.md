# <a name="create-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="37118-101">Criar windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="37118-101">Create windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="37118-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="37118-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="37118-103">Criar um novo objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="37118-103">Create a new [plannerBucket](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="37118-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="37118-104">Prerequisites</span></span>
<span data-ttu-id="37118-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="37118-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="37118-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37118-107">Permission type</span></span>|<span data-ttu-id="37118-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="37118-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37118-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37118-109">Delegated (work or school account)</span></span>|<span data-ttu-id="37118-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37118-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="37118-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37118-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37118-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37118-112">Not supported.</span></span>|
|<span data-ttu-id="37118-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37118-113">Application</span></span>|<span data-ttu-id="37118-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37118-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37118-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37118-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="37118-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37118-116">Request headers</span></span>
|<span data-ttu-id="37118-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="37118-117">Header</span></span>|<span data-ttu-id="37118-118">Valor</span><span class="sxs-lookup"><span data-stu-id="37118-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37118-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="37118-119">Authorization</span></span>|<span data-ttu-id="37118-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37118-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="37118-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="37118-121">Accept</span></span>|<span data-ttu-id="37118-122">application/json</span><span class="sxs-lookup"><span data-stu-id="37118-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37118-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37118-123">Request body</span></span>
<span data-ttu-id="37118-124">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="37118-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="37118-125">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="37118-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="37118-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37118-126">Property</span></span>|<span data-ttu-id="37118-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="37118-127">Type</span></span>|<span data-ttu-id="37118-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="37118-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37118-129">id</span><span class="sxs-lookup"><span data-stu-id="37118-129">id</span></span>|<span data-ttu-id="37118-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37118-130">String</span></span>|<span data-ttu-id="37118-131">Identificador exclusivo de WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="37118-131">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="37118-132">url</span><span class="sxs-lookup"><span data-stu-id="37118-132">url</span></span>|<span data-ttu-id="37118-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37118-133">String</span></span>|<span data-ttu-id="37118-134">Url do site</span><span class="sxs-lookup"><span data-stu-id="37118-134">Website url</span></span>|
|<span data-ttu-id="37118-135">deviceCount</span><span class="sxs-lookup"><span data-stu-id="37118-135">deviceCount</span></span>|<span data-ttu-id="37118-136">Int32</span><span class="sxs-lookup"><span data-stu-id="37118-136">Int32</span></span>|<span data-ttu-id="37118-137">Contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="37118-137">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="37118-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="37118-138">Response</span></span>
<span data-ttu-id="37118-139">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37118-139">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37118-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37118-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="37118-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37118-141">Request</span></span>
<span data-ttu-id="37118-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="37118-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="37118-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="37118-143">Response</span></span>
<span data-ttu-id="37118-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="37118-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 186

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "242108f7-08f7-2421-f708-2124f7082124",
  "url": "Url value",
  "deviceCount": 11
}
```



