# <a name="create-telecomexpensemanagementpartner"></a><span data-ttu-id="518be-101">Criar telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="518be-101">Create telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="518be-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="518be-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="518be-103">Cria um novo objeto [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="518be-103">Create a new [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="518be-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="518be-104">Prerequisites</span></span>
<span data-ttu-id="518be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="518be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="518be-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="518be-107">Permission type</span></span>|<span data-ttu-id="518be-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="518be-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="518be-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="518be-109">Delegated (work or school account)</span></span>|<span data-ttu-id="518be-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="518be-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="518be-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="518be-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="518be-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="518be-112">Not supported.</span></span>|
|<span data-ttu-id="518be-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="518be-113">Application</span></span>|<span data-ttu-id="518be-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="518be-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="518be-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="518be-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="518be-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="518be-116">Request headers</span></span>
|<span data-ttu-id="518be-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="518be-117">Header</span></span>|<span data-ttu-id="518be-118">Valor</span><span class="sxs-lookup"><span data-stu-id="518be-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="518be-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="518be-119">Authorization</span></span>|<span data-ttu-id="518be-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="518be-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="518be-121">Accept</span><span class="sxs-lookup"><span data-stu-id="518be-121">Accept</span></span>|<span data-ttu-id="518be-122">application/json</span><span class="sxs-lookup"><span data-stu-id="518be-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="518be-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="518be-123">Request body</span></span>
<span data-ttu-id="518be-124">No corpo da solicitação, forneça uma representação JSON do objeto telecomExpenseManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="518be-124">In the request body, supply a JSON representation for the telecomExpenseManagementPartner object.</span></span>

<span data-ttu-id="518be-125">A tabela a seguir mostra as propriedades obrigatórias ao criar telecomExpenseManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="518be-125">The following table shows the properties that are required when you create the telecomExpenseManagementPartner.</span></span>

|<span data-ttu-id="518be-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="518be-126">Property</span></span>|<span data-ttu-id="518be-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="518be-127">Type</span></span>|<span data-ttu-id="518be-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="518be-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="518be-129">id</span><span class="sxs-lookup"><span data-stu-id="518be-129">id</span></span>|<span data-ttu-id="518be-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="518be-130">String</span></span>|<span data-ttu-id="518be-131">O identificador exclusivo do parceiro TEM.</span><span class="sxs-lookup"><span data-stu-id="518be-131">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="518be-132">displayName</span><span class="sxs-lookup"><span data-stu-id="518be-132">displayName</span></span>|<span data-ttu-id="518be-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="518be-133">String</span></span>|<span data-ttu-id="518be-134">Nome de exibição do parceiro TEM.</span><span class="sxs-lookup"><span data-stu-id="518be-134">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="518be-135">url</span><span class="sxs-lookup"><span data-stu-id="518be-135">url</span></span>|<span data-ttu-id="518be-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="518be-136">String</span></span>|<span data-ttu-id="518be-137">URL do painel de controle administrativo do parceiro TEM, em que um administrador pode configurar o serviço TEM.</span><span class="sxs-lookup"><span data-stu-id="518be-137">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="518be-138">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="518be-138">appAuthorized</span></span>|<span data-ttu-id="518be-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="518be-139">Boolean</span></span>|<span data-ttu-id="518be-140">Se aplicativo AAD do parceiro foi autorizado a acessar o Intune.</span><span class="sxs-lookup"><span data-stu-id="518be-140">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="518be-141">enabled</span><span class="sxs-lookup"><span data-stu-id="518be-141">enabled</span></span>|<span data-ttu-id="518be-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="518be-142">Boolean</span></span>|<span data-ttu-id="518be-143">Se a conexão do Intune com o serviço TEM está habilitada ou desabilitada no momento.</span><span class="sxs-lookup"><span data-stu-id="518be-143">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="518be-144">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="518be-144">lastConnectionDateTime</span></span>|<span data-ttu-id="518be-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="518be-145">DateTimeOffset</span></span>|<span data-ttu-id="518be-146">Carimbo de data/hora da última solicitação enviada ao Intune pelo parceiro TEM.</span><span class="sxs-lookup"><span data-stu-id="518be-146">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="518be-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="518be-147">Response</span></span>
<span data-ttu-id="518be-148">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="518be-148">If successful, this method returns a `201 Created` response code and a [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="518be-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="518be-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="518be-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="518be-150">Request</span></span>
<span data-ttu-id="518be-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="518be-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners
Content-type: application/json
Content-length: 248

{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="518be-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="518be-152">Response</span></span>
<span data-ttu-id="518be-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="518be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 297

{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "id": "47a3b399-b399-47a3-99b3-a34799b3a347",
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```



