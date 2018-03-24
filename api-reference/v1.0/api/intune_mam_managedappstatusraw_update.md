# <a name="update-managedappstatusraw"></a><span data-ttu-id="1635b-101">Atualizar managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="1635b-101">Update managedAppStatusRaw</span></span>

> <span data-ttu-id="1635b-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1635b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1635b-103">Atualizar as propriedades de um objeto [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="1635b-103">Update the properties of a [calendar](../resources/intune_mam_managedappstatusraw.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1635b-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1635b-104">Prerequisites</span></span>
<span data-ttu-id="1635b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1635b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1635b-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1635b-107">Permission type</span></span>|<span data-ttu-id="1635b-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1635b-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1635b-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1635b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1635b-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1635b-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1635b-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1635b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1635b-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1635b-112">Not supported.</span></span>|
|<span data-ttu-id="1635b-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1635b-113">Application</span></span>|<span data-ttu-id="1635b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1635b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1635b-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1635b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="1635b-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1635b-116">Request headers</span></span>
|<span data-ttu-id="1635b-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1635b-117">Header</span></span>|<span data-ttu-id="1635b-118">Valor</span><span class="sxs-lookup"><span data-stu-id="1635b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1635b-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="1635b-119">Authorization</span></span>|<span data-ttu-id="1635b-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1635b-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1635b-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1635b-121">Accept</span></span>|<span data-ttu-id="1635b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1635b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1635b-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1635b-123">Request body</span></span>
<span data-ttu-id="1635b-124">No corpo da solicitação, forneça uma representação JSON do objeto [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="1635b-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_mam_managedappstatusraw.md) object.</span></span>

<span data-ttu-id="1635b-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="1635b-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="1635b-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1635b-126">Property</span></span>|<span data-ttu-id="1635b-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="1635b-127">Type</span></span>|<span data-ttu-id="1635b-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="1635b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1635b-129">displayName</span><span class="sxs-lookup"><span data-stu-id="1635b-129">displayName</span></span>|<span data-ttu-id="1635b-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1635b-130">String</span></span>|<span data-ttu-id="1635b-131">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="1635b-131">Friendly name of the status report.</span></span> <span data-ttu-id="1635b-132">Herda de [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="1635b-132">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="1635b-133">id</span><span class="sxs-lookup"><span data-stu-id="1635b-133">id</span></span>|<span data-ttu-id="1635b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1635b-134">String</span></span>|<span data-ttu-id="1635b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1635b-135">Key of the setting.</span></span> <span data-ttu-id="1635b-136">Herda de [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="1635b-136">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="1635b-137">version</span><span class="sxs-lookup"><span data-stu-id="1635b-137">version</span></span>|<span data-ttu-id="1635b-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1635b-138">String</span></span>|<span data-ttu-id="1635b-139">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="1635b-139">Version of the entity.</span></span> <span data-ttu-id="1635b-140">Herda de [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="1635b-140">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="1635b-141">content</span><span class="sxs-lookup"><span data-stu-id="1635b-141">content</span></span>|[<span data-ttu-id="1635b-142">Json</span><span class="sxs-lookup"><span data-stu-id="1635b-142">json</span></span>](../resources/intune_mam_json.md)|<span data-ttu-id="1635b-143">Conteúdo do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="1635b-143">Status report content.</span></span>|



## <a name="response"></a><span data-ttu-id="1635b-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="1635b-144">Response</span></span>
<span data-ttu-id="1635b-145">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1635b-145">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_mam_managedappstatusraw.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1635b-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1635b-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="1635b-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1635b-147">Request</span></span>
<span data-ttu-id="1635b-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1635b-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppStatuses/{managedAppStatusId}
Content-type: application/json
Content-length: 139

{
  "displayName": "Display Name value",
  "version": "Version value",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

### <a name="response"></a><span data-ttu-id="1635b-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="1635b-149">Response</span></span>
<span data-ttu-id="1635b-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1635b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 246

{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "displayName": "Display Name value",
  "id": "80847581-7581-8084-8175-848081758480",
  "version": "Version value",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```



