# <a name="assign-action"></a><span data-ttu-id="0bddf-101">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="0bddf-101">assign action</span></span>

> <span data-ttu-id="0bddf-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0bddf-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0bddf-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0bddf-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0bddf-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0bddf-104">Prerequisites</span></span>
<span data-ttu-id="0bddf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0bddf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0bddf-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0bddf-107">Permission type</span></span>|<span data-ttu-id="0bddf-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0bddf-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0bddf-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0bddf-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0bddf-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bddf-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0bddf-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0bddf-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0bddf-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0bddf-112">Not supported.</span></span>|
|<span data-ttu-id="0bddf-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0bddf-113">Application</span></span>|<span data-ttu-id="0bddf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0bddf-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0bddf-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0bddf-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="0bddf-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0bddf-116">Request headers</span></span>
|<span data-ttu-id="0bddf-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0bddf-117">Header</span></span>|<span data-ttu-id="0bddf-118">Valor</span><span class="sxs-lookup"><span data-stu-id="0bddf-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0bddf-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="0bddf-119">Authorization</span></span>|<span data-ttu-id="0bddf-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="0bddf-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0bddf-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0bddf-121">Accept</span></span>|<span data-ttu-id="0bddf-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0bddf-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bddf-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0bddf-123">Request body</span></span>
<span data-ttu-id="0bddf-124">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="0bddf-124">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0bddf-125">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="0bddf-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0bddf-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0bddf-126">Property</span></span>|<span data-ttu-id="0bddf-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="0bddf-127">Type</span></span>|<span data-ttu-id="0bddf-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bddf-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bddf-129">assignments</span><span class="sxs-lookup"><span data-stu-id="0bddf-129">assignments</span></span>|<span data-ttu-id="0bddf-130">Coleção [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="0bddf-130">[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="0bddf-131">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0bddf-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0bddf-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bddf-132">Response</span></span>
<span data-ttu-id="0bddf-133">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0bddf-133">If successful, this action returns a `200 OK` response code and a [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bddf-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0bddf-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="0bddf-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0bddf-135">Request</span></span>
<span data-ttu-id="0bddf-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0bddf-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign

Content-type: application/json
Content-length: 277

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="0bddf-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bddf-137">Response</span></span>
<span data-ttu-id="0bddf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0bddf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 271

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```








