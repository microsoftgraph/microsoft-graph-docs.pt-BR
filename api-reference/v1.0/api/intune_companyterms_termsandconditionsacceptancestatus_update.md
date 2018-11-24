# <a name="update-termsandconditionsacceptancestatus"></a><span data-ttu-id="01099-101">Atualizar termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="01099-101">Update termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="01099-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="01099-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="01099-103">Atualizar as propriedades de um objeto [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="01099-103">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="01099-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="01099-104">Prerequisites</span></span>
<span data-ttu-id="01099-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="01099-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="01099-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01099-107">Permission type</span></span>|<span data-ttu-id="01099-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="01099-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01099-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01099-109">Delegated (work or school account)</span></span>|<span data-ttu-id="01099-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01099-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="01099-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01099-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01099-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01099-112">Not supported.</span></span>|
|<span data-ttu-id="01099-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01099-113">Application</span></span>|<span data-ttu-id="01099-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01099-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01099-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01099-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="01099-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01099-116">Request headers</span></span>
|<span data-ttu-id="01099-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="01099-117">Header</span></span>|<span data-ttu-id="01099-118">Valor</span><span class="sxs-lookup"><span data-stu-id="01099-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01099-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="01099-119">Authorization</span></span>|<span data-ttu-id="01099-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01099-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01099-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="01099-121">Accept</span></span>|<span data-ttu-id="01099-122">application/json</span><span class="sxs-lookup"><span data-stu-id="01099-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01099-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01099-123">Request body</span></span>
<span data-ttu-id="01099-124">No corpo da solicitação, forneça uma representação JSON do objeto [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="01099-124">In the request body, supply a JSON representation for the [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object.</span></span>

<span data-ttu-id="01099-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="01099-125">The following table shows the properties that are required when you create the [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md).</span></span>

|<span data-ttu-id="01099-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01099-126">Property</span></span>|<span data-ttu-id="01099-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="01099-127">Type</span></span>|<span data-ttu-id="01099-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="01099-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01099-129">id</span><span class="sxs-lookup"><span data-stu-id="01099-129">id</span></span>|<span data-ttu-id="01099-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="01099-130">String</span></span>|<span data-ttu-id="01099-131">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="01099-131">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="01099-132">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="01099-132">userDisplayName</span></span>|<span data-ttu-id="01099-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="01099-133">String</span></span>|<span data-ttu-id="01099-134">Nome de exibição do usuário cuja aceitação a entidade representa.</span><span class="sxs-lookup"><span data-stu-id="01099-134">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="01099-135">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="01099-135">acceptedVersion</span></span>|<span data-ttu-id="01099-136">Int32</span><span class="sxs-lookup"><span data-stu-id="01099-136">Int32</span></span>|<span data-ttu-id="01099-137">Número da versão mais recente dos T&C aceitos pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="01099-137">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="01099-138">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="01099-138">acceptedDateTime</span></span>|<span data-ttu-id="01099-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01099-139">DateTimeOffset</span></span>|<span data-ttu-id="01099-140">A data e a hora em que os termos foram aceitos pela última vez pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="01099-140">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="01099-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="01099-141">Response</span></span>
<span data-ttu-id="01099-142">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01099-142">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01099-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01099-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="01099-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01099-144">Request</span></span>
<span data-ttu-id="01099-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="01099-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="01099-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="01099-146">Response</span></span>
<span data-ttu-id="01099-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01099-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



