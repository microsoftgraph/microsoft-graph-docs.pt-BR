# <a name="create-termsandconditionsacceptancestatus"></a><span data-ttu-id="beea2-101">Criar termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="beea2-101">Create termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="beea2-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="beea2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="beea2-103">Cria um novo objeto [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="beea2-103">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="beea2-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="beea2-104">Prerequisites</span></span>
<span data-ttu-id="beea2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="beea2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="beea2-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="beea2-107">Permission type</span></span>|<span data-ttu-id="beea2-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="beea2-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="beea2-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="beea2-109">Delegated (work or school account)</span></span>|<span data-ttu-id="beea2-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="beea2-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="beea2-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="beea2-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="beea2-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="beea2-112">Not supported.</span></span>|
|<span data-ttu-id="beea2-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="beea2-113">Application</span></span>|<span data-ttu-id="beea2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="beea2-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="beea2-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="beea2-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="beea2-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="beea2-116">Request headers</span></span>
|<span data-ttu-id="beea2-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="beea2-117">Header</span></span>|<span data-ttu-id="beea2-118">Valor</span><span class="sxs-lookup"><span data-stu-id="beea2-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="beea2-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="beea2-119">Authorization</span></span>|<span data-ttu-id="beea2-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="beea2-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="beea2-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="beea2-121">Accept</span></span>|<span data-ttu-id="beea2-122">application/json</span><span class="sxs-lookup"><span data-stu-id="beea2-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="beea2-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="beea2-123">Request body</span></span>
<span data-ttu-id="beea2-124">No corpo da solicitação, forneça uma representação JSON do objeto termsAndConditionsAcceptanceStatus.</span><span class="sxs-lookup"><span data-stu-id="beea2-124">In the request body, supply a JSON representation for the termsAndConditionsAcceptanceStatus object.</span></span>

<span data-ttu-id="beea2-125">A tabela a seguir mostra as propriedades que são necessárias ao criar termsAndConditionsAcceptanceStatus.</span><span class="sxs-lookup"><span data-stu-id="beea2-125">The following table shows the properties that are required when you create the termsAndConditionsAcceptanceStatus.</span></span>

|<span data-ttu-id="beea2-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="beea2-126">Property</span></span>|<span data-ttu-id="beea2-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="beea2-127">Type</span></span>|<span data-ttu-id="beea2-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="beea2-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="beea2-129">id</span><span class="sxs-lookup"><span data-stu-id="beea2-129">id</span></span>|<span data-ttu-id="beea2-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="beea2-130">String</span></span>|<span data-ttu-id="beea2-131">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="beea2-131">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="beea2-132">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="beea2-132">userDisplayName</span></span>|<span data-ttu-id="beea2-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="beea2-133">String</span></span>|<span data-ttu-id="beea2-134">Nome de exibição do usuário cuja aceitação a entidade representa.</span><span class="sxs-lookup"><span data-stu-id="beea2-134">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="beea2-135">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="beea2-135">acceptedVersion</span></span>|<span data-ttu-id="beea2-136">Int32</span><span class="sxs-lookup"><span data-stu-id="beea2-136">Int32</span></span>|<span data-ttu-id="beea2-137">Número da versão mais recente dos T&C aceitos pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="beea2-137">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="beea2-138">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="beea2-138">acceptedDateTime</span></span>|<span data-ttu-id="beea2-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="beea2-139">DateTimeOffset</span></span>|<span data-ttu-id="beea2-140">A data e a hora em que os termos foram aceitos pela última vez pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="beea2-140">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="beea2-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="beea2-141">Response</span></span>
<span data-ttu-id="beea2-142">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="beea2-142">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="beea2-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="beea2-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="beea2-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="beea2-144">Request</span></span>
<span data-ttu-id="beea2-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="beea2-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="beea2-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="beea2-146">Response</span></span>
<span data-ttu-id="beea2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="beea2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```



