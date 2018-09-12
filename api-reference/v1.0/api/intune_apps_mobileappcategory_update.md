# <a name="update-mobileappcategory"></a><span data-ttu-id="31e68-101">Atualizar mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="31e68-101">Update mobileAppCategory</span></span>

> <span data-ttu-id="31e68-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="31e68-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31e68-103">Atualizar as propriedades de um objeto [mobileAppCategory](../resources/intune_apps_mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="31e68-103">Update the properties of a [mobileAppCategory](../resources/intune_apps_mobileappcategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="31e68-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="31e68-104">Prerequisites</span></span>
<span data-ttu-id="31e68-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="31e68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="31e68-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31e68-107">Permission type</span></span>|<span data-ttu-id="31e68-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="31e68-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31e68-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31e68-109">Delegated (work or school account)</span></span>|<span data-ttu-id="31e68-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31e68-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="31e68-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31e68-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31e68-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31e68-112">Not supported.</span></span>|
|<span data-ttu-id="31e68-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31e68-113">Application</span></span>|<span data-ttu-id="31e68-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31e68-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31e68-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31e68-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="31e68-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31e68-116">Request headers</span></span>
|<span data-ttu-id="31e68-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="31e68-117">Header</span></span>|<span data-ttu-id="31e68-118">Valor</span><span class="sxs-lookup"><span data-stu-id="31e68-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31e68-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="31e68-119">Authorization</span></span>|<span data-ttu-id="31e68-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="31e68-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31e68-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="31e68-121">Accept</span></span>|<span data-ttu-id="31e68-122">application/json</span><span class="sxs-lookup"><span data-stu-id="31e68-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31e68-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31e68-123">Request body</span></span>
<span data-ttu-id="31e68-124">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppCategory](../resources/intune_apps_mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="31e68-124">In the request body, supply a JSON representation for the [mobileAppCategory](../resources/intune_apps_mobileappcategory.md) object.</span></span>

<span data-ttu-id="31e68-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppCategory](../resources/intune_apps_mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="31e68-125">The following table shows the properties that are required when you create the [mobileAppCategory](../resources/intune_apps_mobileappcategory.md).</span></span>

|<span data-ttu-id="31e68-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="31e68-126">Property</span></span>|<span data-ttu-id="31e68-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="31e68-127">Type</span></span>|<span data-ttu-id="31e68-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="31e68-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31e68-129">id</span><span class="sxs-lookup"><span data-stu-id="31e68-129">id</span></span>|<span data-ttu-id="31e68-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="31e68-130">String</span></span>|<span data-ttu-id="31e68-131">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="31e68-131">The key of the entity.</span></span>|
|<span data-ttu-id="31e68-132">displayName</span><span class="sxs-lookup"><span data-stu-id="31e68-132">displayName</span></span>|<span data-ttu-id="31e68-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="31e68-133">String</span></span>|<span data-ttu-id="31e68-134">O nome da categoria do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="31e68-134">The name of the app category.</span></span>|
|<span data-ttu-id="31e68-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="31e68-135">lastModifiedDateTime</span></span>|<span data-ttu-id="31e68-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31e68-136">DateTimeOffset</span></span>|<span data-ttu-id="31e68-137">A data e hora que a mobileAppCategory foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="31e68-137">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="31e68-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="31e68-138">Response</span></span>
<span data-ttu-id="31e68-139">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [mobileAppCategory](../resources/intune_apps_mobileappcategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31e68-139">If successful, this method returns a `200 OK` response code and an updated [mobileAppCategory](../resources/intune_apps_mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31e68-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="31e68-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="31e68-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31e68-141">Request</span></span>
<span data-ttu-id="31e68-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="31e68-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
Content-type: application/json
Content-length: 107

{
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```

### <a name="response"></a><span data-ttu-id="31e68-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="31e68-143">Response</span></span>
<span data-ttu-id="31e68-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="31e68-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 212

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```








