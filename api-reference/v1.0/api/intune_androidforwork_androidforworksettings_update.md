# <a name="update-androidforworksettings"></a><span data-ttu-id="d7c03-101">Atualizar androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="d7c03-101">Update androidForWorkSettings</span></span>

> <span data-ttu-id="d7c03-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d7c03-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d7c03-103">Atualizar as propriedades de um objeto de [androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="d7c03-103">Update the properties of a [calendar](../resources/intune_androidforwork_androidforworksettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d7c03-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d7c03-104">Prerequisites</span></span>
<span data-ttu-id="d7c03-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d7c03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d7c03-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7c03-107">Permission type</span></span>|<span data-ttu-id="d7c03-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d7c03-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7c03-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7c03-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d7c03-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7c03-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d7c03-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d7c03-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7c03-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7c03-112">Not supported.</span></span>|
|<span data-ttu-id="d7c03-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7c03-113">Application</span></span>|<span data-ttu-id="d7c03-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7c03-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7c03-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7c03-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkSettings
```

## <a name="request-headers"></a><span data-ttu-id="d7c03-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7c03-116">Request headers</span></span>
|<span data-ttu-id="d7c03-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d7c03-117">Header</span></span>|<span data-ttu-id="d7c03-118">Valor</span><span class="sxs-lookup"><span data-stu-id="d7c03-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7c03-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7c03-119">Authorization</span></span>|<span data-ttu-id="d7c03-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7c03-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d7c03-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d7c03-121">Accept</span></span>|<span data-ttu-id="d7c03-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d7c03-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7c03-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7c03-123">Request body</span></span>
<span data-ttu-id="d7c03-124">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="d7c03-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_androidforwork_androidforworksettings.md) object.</span></span>

<span data-ttu-id="d7c03-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="d7c03-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="d7c03-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d7c03-126">Property</span></span>|<span data-ttu-id="d7c03-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7c03-127">Type</span></span>|<span data-ttu-id="d7c03-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7c03-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7c03-129">id</span><span class="sxs-lookup"><span data-stu-id="d7c03-129">id</span></span>|<span data-ttu-id="d7c03-130">String</span><span class="sxs-lookup"><span data-stu-id="d7c03-130">String</span></span>|<span data-ttu-id="d7c03-131">O identificador de configurações do Android for Work</span><span class="sxs-lookup"><span data-stu-id="d7c03-131">The Android for Work settings identifier</span></span>|
|<span data-ttu-id="d7c03-132">bindStatus</span><span class="sxs-lookup"><span data-stu-id="d7c03-132">bindStatus</span></span>|<span data-ttu-id="d7c03-133">String</span><span class="sxs-lookup"><span data-stu-id="d7c03-133">String</span></span>|<span data-ttu-id="d7c03-134">Associa o status do locatário com a API do Google EMM Os valores possíveis são: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span><span class="sxs-lookup"><span data-stu-id="d7c03-134">Bind status of the tenant with the Google EMM API Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="d7c03-135">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d7c03-135">lastAppSyncDateTime</span></span>|<span data-ttu-id="d7c03-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7c03-136">DateTimeOffset</span></span>|<span data-ttu-id="d7c03-137">Hora da conclusão da última sincronização do aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7c03-137">Last completion time for app sync</span></span>|
|<span data-ttu-id="d7c03-138">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="d7c03-138">lastAppSyncStatus</span></span>|<span data-ttu-id="d7c03-139">String</span><span class="sxs-lookup"><span data-stu-id="d7c03-139">String</span></span>|<span data-ttu-id="d7c03-140">Resultado da última sincronização do aplicativo Os valores possíveis são: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="d7c03-140">Last application sync result Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="d7c03-141">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d7c03-141">ownerUserPrincipalName</span></span>|<span data-ttu-id="d7c03-142">String</span><span class="sxs-lookup"><span data-stu-id="d7c03-142">String</span></span>|<span data-ttu-id="d7c03-143">UPN proprietária que criou a empresa</span><span class="sxs-lookup"><span data-stu-id="d7c03-143">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="d7c03-144">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="d7c03-144">ownerOrganizationName</span></span>|<span data-ttu-id="d7c03-145">String</span><span class="sxs-lookup"><span data-stu-id="d7c03-145">String</span></span>|<span data-ttu-id="d7c03-146">Nome da organização usada ao integrar o Android for Work</span><span class="sxs-lookup"><span data-stu-id="d7c03-146">Organization name used when onboarding Android for Work</span></span>|
|<span data-ttu-id="d7c03-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d7c03-147">lastModifiedDateTime</span></span>|<span data-ttu-id="d7c03-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7c03-148">DateTimeOffset</span></span>|<span data-ttu-id="d7c03-149">Hora da última modificação das configurações do Android for Work</span><span class="sxs-lookup"><span data-stu-id="d7c03-149">Last modification time for Android for Work settings</span></span>|
|<span data-ttu-id="d7c03-150">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="d7c03-150">enrollmentTarget</span></span>|<span data-ttu-id="d7c03-151">String</span><span class="sxs-lookup"><span data-stu-id="d7c03-151">String</span></span>|<span data-ttu-id="d7c03-152">Indica quais usuários podem registrar dispositivos no gerenciamento de dispositivos do Android for Work Os valores possíveis são: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="d7c03-152">Indicates which users can enroll devices in Android for Work device management Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="d7c03-153">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="d7c03-153">targetGroupIds</span></span>|<span data-ttu-id="d7c03-154">String collection</span><span class="sxs-lookup"><span data-stu-id="d7c03-154">String collection</span></span>|<span data-ttu-id="d7c03-155">Especifica a quais grupos AAD podem registrar dispositivos no gerenciamento de dispositivos do Android for Work se enrollmentTarget estiver definido como 'Direcionado'</span><span class="sxs-lookup"><span data-stu-id="d7c03-155">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|



## <a name="response"></a><span data-ttu-id="d7c03-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7c03-156">Response</span></span>
<span data-ttu-id="d7c03-157">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7c03-157">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_androidforwork_androidforworksettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7c03-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d7c03-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="d7c03-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7c03-159">Request</span></span>
<span data-ttu-id="d7c03-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7c03-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkSettings
Content-type: application/json
Content-length: 417

{
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="d7c03-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7c03-161">Response</span></span>
<span data-ttu-id="d7c03-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d7c03-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 527

{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "id": "97adc169-c169-97ad-69c1-ad9769c1ad97",
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ]
}
```



