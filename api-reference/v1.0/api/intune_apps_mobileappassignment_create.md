# <a name="create-mobileappassignment"></a><span data-ttu-id="22579-101">Criar mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="22579-101">Create mobileAppAssignment</span></span>

> <span data-ttu-id="22579-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="22579-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="22579-103">Criar um novo objeto [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="22579-103">Create a new [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="22579-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="22579-104">Prerequisites</span></span>
<span data-ttu-id="22579-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="22579-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="22579-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22579-107">Permission type</span></span>|<span data-ttu-id="22579-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="22579-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22579-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22579-109">Delegated (work or school account)</span></span>|<span data-ttu-id="22579-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22579-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="22579-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22579-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22579-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22579-112">Not supported.</span></span>|
|<span data-ttu-id="22579-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22579-113">Application</span></span>|<span data-ttu-id="22579-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22579-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22579-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22579-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="22579-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22579-116">Request headers</span></span>
|<span data-ttu-id="22579-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="22579-117">Header</span></span>|<span data-ttu-id="22579-118">Valor</span><span class="sxs-lookup"><span data-stu-id="22579-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22579-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="22579-119">Authorization</span></span>|<span data-ttu-id="22579-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="22579-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22579-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="22579-121">Accept</span></span>|<span data-ttu-id="22579-122">aplicativo/json</span><span class="sxs-lookup"><span data-stu-id="22579-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22579-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22579-123">Request body</span></span>
<span data-ttu-id="22579-124">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppAssignment.</span><span class="sxs-lookup"><span data-stu-id="22579-124">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="22579-125">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppAssignment.</span><span class="sxs-lookup"><span data-stu-id="22579-125">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="22579-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22579-126">Property</span></span>|<span data-ttu-id="22579-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="22579-127">Type</span></span>|<span data-ttu-id="22579-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="22579-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22579-129">id</span><span class="sxs-lookup"><span data-stu-id="22579-129">id</span></span>|<span data-ttu-id="22579-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22579-130">String</span></span>|<span data-ttu-id="22579-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="22579-131">Key of the entity.</span></span>|
|<span data-ttu-id="22579-132">intent</span><span class="sxs-lookup"><span data-stu-id="22579-132">intent</span></span>|[<span data-ttu-id="22579-133">installIntent</span><span class="sxs-lookup"><span data-stu-id="22579-133">installIntent</span></span>](../resources/intune_shared_installintent.md)|<span data-ttu-id="22579-134">A intenção de instalação definida pelo administrador. Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="22579-134">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="22579-135">target</span><span class="sxs-lookup"><span data-stu-id="22579-135">target</span></span>|[<span data-ttu-id="22579-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="22579-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="22579-137">A atribuição do grupo de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="22579-137">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="22579-138">configurações</span><span class="sxs-lookup"><span data-stu-id="22579-138">settings</span></span>|[<span data-ttu-id="22579-139">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="22579-139">mobileAppAssignmentSettings</span></span>](../resources/intune_apps_mobileappassignmentsettings.md)|<span data-ttu-id="22579-140">As configurações para a atribuição de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="22579-140">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="22579-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="22579-141">Response</span></span>
<span data-ttu-id="22579-142">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22579-142">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22579-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22579-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="22579-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22579-144">Request</span></span>
<span data-ttu-id="22579-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="22579-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments
Content-type: application/json
Content-length: 273

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```

### <a name="response"></a><span data-ttu-id="22579-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="22579-146">Response</span></span>
<span data-ttu-id="22579-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22579-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 322

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "591620b7-20b7-5916-b720-1659b7201659",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```



