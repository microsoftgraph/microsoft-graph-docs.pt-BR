# <a name="update-devicemanagement"></a><span data-ttu-id="d3017-101">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="d3017-101">Update deviceManagement</span></span>

> <span data-ttu-id="d3017-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d3017-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d3017-103">Atualizar as propriedades de um objeto [deviceManagement](../resources/intune_deviceconfig_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="d3017-103">Update the properties of a [calendar](../resources/intune_deviceconfig_devicemanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d3017-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d3017-104">Prerequisites</span></span>
<span data-ttu-id="d3017-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d3017-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d3017-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3017-107">Permission type</span></span>|<span data-ttu-id="d3017-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d3017-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3017-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3017-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d3017-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3017-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d3017-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3017-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3017-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3017-112">Not supported.</span></span>|
|<span data-ttu-id="d3017-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3017-113">Application</span></span>|<span data-ttu-id="d3017-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3017-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3017-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3017-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="d3017-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3017-116">Request headers</span></span>
|<span data-ttu-id="d3017-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d3017-117">Header</span></span>|<span data-ttu-id="d3017-118">Valor</span><span class="sxs-lookup"><span data-stu-id="d3017-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3017-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3017-119">Authorization</span></span>|<span data-ttu-id="d3017-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3017-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d3017-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d3017-121">Accept</span></span>|<span data-ttu-id="d3017-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d3017-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3017-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3017-123">Request body</span></span>
<span data-ttu-id="d3017-124">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagement](../resources/intune_deviceconfig_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="d3017-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_devicemanagement.md) object.</span></span>

<span data-ttu-id="d3017-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagement](../resources/intune_deviceconfig_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="d3017-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="d3017-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3017-126">Property</span></span>|<span data-ttu-id="d3017-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3017-127">Type</span></span>|<span data-ttu-id="d3017-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3017-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3017-129">id</span><span class="sxs-lookup"><span data-stu-id="d3017-129">id</span></span>|<span data-ttu-id="d3017-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3017-130">String</span></span>|<span data-ttu-id="d3017-131">Identificador exclusivo</span><span class="sxs-lookup"><span data-stu-id="d3017-131">Unique Identifier</span></span>|
|<span data-ttu-id="d3017-132">configurações</span><span class="sxs-lookup"><span data-stu-id="d3017-132">settings</span></span>|[<span data-ttu-id="d3017-133">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="d3017-133">deviceManagementSettings</span></span>](../resources/intune_deviceconfig_devicemanagementsettings.md)|<span data-ttu-id="d3017-134">Configurações de nível da conta.</span><span class="sxs-lookup"><span data-stu-id="d3017-134">Account level settings.</span></span>|



## <a name="response"></a><span data-ttu-id="d3017-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3017-135">Response</span></span>
<span data-ttu-id="d3017-136">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagement](../resources/intune_deviceconfig_devicemanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3017-136">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3017-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3017-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="d3017-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3017-138">Request</span></span>
<span data-ttu-id="d3017-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3017-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement
Content-type: application/json
Content-length: 206

{
  "settings": {
    "@odata.type": "microsoft.graph.deviceManagementSettings",
    "deviceComplianceCheckinThresholdDays": 4,
    "isScheduledActionEnabled": true,
    "secureByDefault": true
  }
}
```

### <a name="response"></a><span data-ttu-id="d3017-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3017-140">Response</span></span>
<span data-ttu-id="d3017-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3017-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 310

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "0b283420-3420-0b28-2034-280b2034280b",
  "settings": {
    "@odata.type": "microsoft.graph.deviceManagementSettings",
    "deviceComplianceCheckinThresholdDays": 4,
    "isScheduledActionEnabled": true,
    "secureByDefault": true
  }
}
```



