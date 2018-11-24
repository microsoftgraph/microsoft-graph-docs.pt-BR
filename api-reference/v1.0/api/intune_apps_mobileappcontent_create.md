# <a name="create-mobileappcontent"></a><span data-ttu-id="da341-101">Criar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="da341-101">Create mobileAppContent</span></span>

> <span data-ttu-id="da341-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="da341-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="da341-103">Criar um novo objeto [mobileAppContent](../resources/intune_apps_mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="da341-103">Create a new [mobileAppContent](../resources/intune_apps_mobileappcontent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="da341-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="da341-104">Prerequisites</span></span>
<span data-ttu-id="da341-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="da341-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="da341-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da341-107">Permission type</span></span>|<span data-ttu-id="da341-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="da341-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da341-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da341-109">Delegated (work or school account)</span></span>|<span data-ttu-id="da341-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da341-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="da341-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da341-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da341-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da341-112">Not supported.</span></span>|
|<span data-ttu-id="da341-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da341-113">Application</span></span>|<span data-ttu-id="da341-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da341-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da341-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da341-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="da341-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da341-116">Request headers</span></span>
|<span data-ttu-id="da341-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="da341-117">Header</span></span>|<span data-ttu-id="da341-118">Valor</span><span class="sxs-lookup"><span data-stu-id="da341-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da341-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="da341-119">Authorization</span></span>|<span data-ttu-id="da341-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da341-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da341-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="da341-121">Accept</span></span>|<span data-ttu-id="da341-122">application/json</span><span class="sxs-lookup"><span data-stu-id="da341-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da341-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da341-123">Request body</span></span>
<span data-ttu-id="da341-124">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppContent.</span><span class="sxs-lookup"><span data-stu-id="da341-124">In the request body, supply a JSON representation for the mobileAppContent object.</span></span>

<span data-ttu-id="da341-125">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppContent.</span><span class="sxs-lookup"><span data-stu-id="da341-125">The following table shows the properties that are required when you create the mobileAppContent.</span></span>

|<span data-ttu-id="da341-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da341-126">Property</span></span>|<span data-ttu-id="da341-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="da341-127">Type</span></span>|<span data-ttu-id="da341-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="da341-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da341-129">id</span><span class="sxs-lookup"><span data-stu-id="da341-129">id</span></span>|<span data-ttu-id="da341-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="da341-130">String</span></span>|<span data-ttu-id="da341-131">A versão do conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="da341-131">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="da341-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="da341-132">Response</span></span>
<span data-ttu-id="da341-133">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileAppContent](../resources/intune_apps_mobileappcontent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da341-133">If successful, this method returns a `201 Created` response code and a [mobileAppContent](../resources/intune_apps_mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da341-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da341-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="da341-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da341-135">Request</span></span>
<span data-ttu-id="da341-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da341-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="da341-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="da341-137">Response</span></span>
<span data-ttu-id="da341-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="da341-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```



