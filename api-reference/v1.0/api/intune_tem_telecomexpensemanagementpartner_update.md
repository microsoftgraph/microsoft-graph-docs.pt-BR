# <a name="update-telecomexpensemanagementpartner"></a><span data-ttu-id="9b289-101">Atualizar telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="9b289-101">Update telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="9b289-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9b289-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9b289-103">Atualizar as propriedades de um objeto [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="9b289-103">Update the properties of a [calendar](../resources/intune_tem_telecomexpensemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9b289-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9b289-104">Prerequisites</span></span>
<span data-ttu-id="9b289-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9b289-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9b289-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b289-107">Permission type</span></span>|<span data-ttu-id="9b289-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9b289-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b289-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b289-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9b289-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b289-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9b289-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b289-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b289-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b289-112">Not supported.</span></span>|
|<span data-ttu-id="9b289-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b289-113">Application</span></span>|<span data-ttu-id="9b289-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b289-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b289-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b289-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="9b289-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b289-116">Request headers</span></span>
|<span data-ttu-id="9b289-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9b289-117">Header</span></span>|<span data-ttu-id="9b289-118">Valor</span><span class="sxs-lookup"><span data-stu-id="9b289-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b289-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b289-119">Authorization</span></span>|<span data-ttu-id="9b289-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b289-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9b289-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9b289-121">Accept</span></span>|<span data-ttu-id="9b289-122">application/json</span><span class="sxs-lookup"><span data-stu-id="9b289-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b289-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b289-123">Request body</span></span>
<span data-ttu-id="9b289-124">No corpo da solicitação, forneça uma representação JSON do objeto [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="9b289-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_tem_telecomexpensemanagementpartner.md) object.</span></span>

<span data-ttu-id="9b289-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="9b289-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="9b289-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b289-126">Property</span></span>|<span data-ttu-id="9b289-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b289-127">Type</span></span>|<span data-ttu-id="9b289-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b289-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b289-129">id</span><span class="sxs-lookup"><span data-stu-id="9b289-129">id</span></span>|<span data-ttu-id="9b289-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b289-130">String</span></span>|<span data-ttu-id="9b289-131">O identificador exclusivo do parceiro TEM.</span><span class="sxs-lookup"><span data-stu-id="9b289-131">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="9b289-132">displayName</span><span class="sxs-lookup"><span data-stu-id="9b289-132">displayName</span></span>|<span data-ttu-id="9b289-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b289-133">String</span></span>|<span data-ttu-id="9b289-134">Nome de exibição do parceiro TEM.</span><span class="sxs-lookup"><span data-stu-id="9b289-134">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="9b289-135">url</span><span class="sxs-lookup"><span data-stu-id="9b289-135">url</span></span>|<span data-ttu-id="9b289-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b289-136">String</span></span>|<span data-ttu-id="9b289-137">URL do painel de controle administrativo do parceiro TEM, em que um administrador pode configurar o serviço TEM.</span><span class="sxs-lookup"><span data-stu-id="9b289-137">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="9b289-138">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="9b289-138">appAuthorized</span></span>|<span data-ttu-id="9b289-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="9b289-139">Boolean</span></span>|<span data-ttu-id="9b289-140">Se aplicativo AAD do parceiro foi autorizado a acessar o Intune.</span><span class="sxs-lookup"><span data-stu-id="9b289-140">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="9b289-141">enabled</span><span class="sxs-lookup"><span data-stu-id="9b289-141">enabled</span></span>|<span data-ttu-id="9b289-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="9b289-142">Boolean</span></span>|<span data-ttu-id="9b289-143">Se a conexão do Intune com o serviço TEM está habilitada ou desabilitada no momento.</span><span class="sxs-lookup"><span data-stu-id="9b289-143">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="9b289-144">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="9b289-144">lastConnectionDateTime</span></span>|<span data-ttu-id="9b289-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b289-145">DateTimeOffset</span></span>|<span data-ttu-id="9b289-146">Carimbo de data/hora da última solicitação enviada ao Intune pelo parceiro TEM.</span><span class="sxs-lookup"><span data-stu-id="9b289-146">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="9b289-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b289-147">Response</span></span>
<span data-ttu-id="9b289-148">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b289-148">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_tem_telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b289-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b289-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="9b289-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b289-150">Request</span></span>
<span data-ttu-id="9b289-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b289-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
Content-type: application/json
Content-length: 178

{
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="9b289-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b289-152">Response</span></span>
<span data-ttu-id="9b289-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9b289-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



