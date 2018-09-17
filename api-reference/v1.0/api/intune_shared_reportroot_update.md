# <a name="update-reportroot"></a><span data-ttu-id="5ea2f-101">Atualizar reportRoot</span><span class="sxs-lookup"><span data-stu-id="5ea2f-101">Update reportRoot</span></span>

> <span data-ttu-id="5ea2f-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5ea2f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5ea2f-103">Atualizar as propriedades de um objeto [reportRoot](../resources/intune_shared_reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="5ea2f-103">Update the properties of a [reportRoot](../resources/intune_shared_reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5ea2f-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5ea2f-104">Prerequisites</span></span>
<span data-ttu-id="5ea2f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5ea2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5ea2f-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ea2f-107">Permission type</span></span>|<span data-ttu-id="5ea2f-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5ea2f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ea2f-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ea2f-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5ea2f-110">&nbsp; &nbsp; Configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5ea2f-110">&nbsp; &nbsp;Device Configuration.</span></span> | <span data-ttu-id="5ea2f-111">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ea2f-111">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="5ea2f-112">&nbsp; &nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="5ea2f-112">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="5ea2f-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ea2f-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5ea2f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ea2f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ea2f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ea2f-115">Not supported.</span></span>|
|<span data-ttu-id="5ea2f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ea2f-116">Application</span></span>|<span data-ttu-id="5ea2f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ea2f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ea2f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ea2f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="5ea2f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ea2f-119">Request headers</span></span>
|<span data-ttu-id="5ea2f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ea2f-120">Header</span></span>|<span data-ttu-id="5ea2f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5ea2f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ea2f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ea2f-122">Authorization</span></span>|<span data-ttu-id="5ea2f-123">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="5ea2f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ea2f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5ea2f-124">Accept</span></span>|<span data-ttu-id="5ea2f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5ea2f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ea2f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ea2f-126">Request body</span></span>
<span data-ttu-id="5ea2f-127">No corpo da solicitação, forneça uma representação JSON do objeto [reportRoot](../resources/intune_shared_reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="5ea2f-127">In the request body, supply a JSON representation for the [reportRoot](../resources/intune_shared_reportroot.md) object.</span></span>

<span data-ttu-id="5ea2f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [reportRoot](../resources/intune_shared_reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="5ea2f-128">The following table shows the properties that are required when you create the [reportRoot](../resources/intune_shared_reportroot.md).</span></span>

|<span data-ttu-id="5ea2f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ea2f-129">Property</span></span>|<span data-ttu-id="5ea2f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ea2f-130">Type</span></span>|<span data-ttu-id="5ea2f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ea2f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ea2f-132">id</span><span class="sxs-lookup"><span data-stu-id="5ea2f-132">id</span></span>|<span data-ttu-id="5ea2f-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ea2f-133">String</span></span>|<span data-ttu-id="5ea2f-134">O identificador exclusivo dessa entidade.</span><span class="sxs-lookup"><span data-stu-id="5ea2f-134">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="5ea2f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ea2f-135">Response</span></span>
<span data-ttu-id="5ea2f-136">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [reportRoot](../resources/intune_shared_reportroot.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ea2f-136">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune_shared_reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ea2f-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ea2f-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="5ea2f-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ea2f-138">Request</span></span>
<span data-ttu-id="5ea2f-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ea2f-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="5ea2f-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ea2f-140">Response</span></span>
<span data-ttu-id="5ea2f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ea2f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```








