# <a name="targetapps-action"></a><span data-ttu-id="71ada-101">Ação targetApps</span><span class="sxs-lookup"><span data-stu-id="71ada-101">targetApps action</span></span>

> <span data-ttu-id="71ada-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="71ada-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71ada-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="71ada-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="71ada-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="71ada-104">Prerequisites</span></span>
<span data-ttu-id="71ada-p101">Uma das permissões a seguir é obrigatória para chamar esta API. Para saber mais, inclusive como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="71ada-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="71ada-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71ada-107">Permission type</span></span>|<span data-ttu-id="71ada-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="71ada-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71ada-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71ada-109">Delegated (work or school account)</span></span>|<span data-ttu-id="71ada-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71ada-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="71ada-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71ada-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71ada-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71ada-112">Not supported.</span></span>|
|<span data-ttu-id="71ada-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71ada-113">Application</span></span>|<span data-ttu-id="71ada-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71ada-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71ada-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71ada-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="71ada-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71ada-116">Request headers</span></span>
|<span data-ttu-id="71ada-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="71ada-117">Header</span></span>|<span data-ttu-id="71ada-118">Valor</span><span class="sxs-lookup"><span data-stu-id="71ada-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71ada-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="71ada-119">Authorization</span></span>|<span data-ttu-id="71ada-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71ada-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="71ada-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="71ada-121">Accept</span></span>|<span data-ttu-id="71ada-122">application/json</span><span class="sxs-lookup"><span data-stu-id="71ada-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71ada-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71ada-123">Request body</span></span>
<span data-ttu-id="71ada-124">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="71ada-124">In the request body, supply a JSON representation of the Contact object.</span></span>

<span data-ttu-id="71ada-125">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="71ada-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="71ada-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71ada-126">Property</span></span>|<span data-ttu-id="71ada-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="71ada-127">Type</span></span>|<span data-ttu-id="71ada-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="71ada-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71ada-129">Aplicativos</span><span class="sxs-lookup"><span data-stu-id="71ada-129">apps</span></span>|<span data-ttu-id="71ada-130">Coleção [managedMobileApp](../resources/intune_mam_managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="71ada-130">[managedMobileApp](../resources/intune_mam_managedmobileapp.md) collection</span></span>|<span data-ttu-id="71ada-131">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="71ada-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="71ada-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="71ada-132">Response</span></span>
<span data-ttu-id="71ada-133">Se tiver êxito, esta ação retornará o código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="71ada-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="71ada-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71ada-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="71ada-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71ada-135">Request</span></span>
<span data-ttu-id="71ada-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="71ada-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps

Content-type: application/json
Content-length: 286

{
  "apps": [
    {
      "@odata.type": "#microsoft.graph.managedMobileApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.mobileAppIdentifier"
      },
      "id": "0a129715-9715-0a12-1597-120a1597120a",
      "version": "Version value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="71ada-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="71ada-137">Response</span></span>
<span data-ttu-id="71ada-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="71ada-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



