# <a name="update-devicemanagement"></a><span data-ttu-id="d6bde-101">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="d6bde-101">Update deviceManagement</span></span>

> <span data-ttu-id="d6bde-102">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d6bde-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6bde-103">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d6bde-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d6bde-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d6bde-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6bde-105">Atualizar as propriedades de um objeto [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="d6bde-105">Update the properties of a [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d6bde-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d6bde-106">Prerequisites</span></span>
<span data-ttu-id="d6bde-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d6bde-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d6bde-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6bde-109">Permission type</span></span>|<span data-ttu-id="d6bde-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d6bde-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6bde-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6bde-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d6bde-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6bde-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d6bde-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6bde-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6bde-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6bde-114">Not supported.</span></span>|
|<span data-ttu-id="d6bde-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6bde-115">Application</span></span>|<span data-ttu-id="d6bde-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6bde-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6bde-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6bde-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="d6bde-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6bde-118">Request headers</span></span>
|<span data-ttu-id="d6bde-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d6bde-119">Header</span></span>|<span data-ttu-id="d6bde-120">Valor</span><span class="sxs-lookup"><span data-stu-id="d6bde-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6bde-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6bde-121">Authorization</span></span>|<span data-ttu-id="d6bde-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6bde-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6bde-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d6bde-123">Accept</span></span>|<span data-ttu-id="d6bde-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d6bde-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6bde-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6bde-125">Request body</span></span>
<span data-ttu-id="d6bde-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="d6bde-126">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) object.</span></span>

<span data-ttu-id="d6bde-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="d6bde-127">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md).</span></span>

|<span data-ttu-id="d6bde-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6bde-128">Property</span></span>|<span data-ttu-id="d6bde-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6bde-129">Type</span></span>|<span data-ttu-id="d6bde-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6bde-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6bde-131">id</span><span class="sxs-lookup"><span data-stu-id="d6bde-131">id</span></span>|<span data-ttu-id="d6bde-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6bde-132">String</span></span>|<span data-ttu-id="d6bde-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d6bde-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d6bde-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6bde-134">Response</span></span>
<span data-ttu-id="d6bde-135">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6bde-135">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6bde-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6bde-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="d6bde-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6bde-137">Request</span></span>
<span data-ttu-id="d6bde-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6bde-138">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="d6bde-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6bde-139">Response</span></span>
<span data-ttu-id="d6bde-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d6bde-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "0b283420-3420-0b28-2034-280b2034280b"
}
```



