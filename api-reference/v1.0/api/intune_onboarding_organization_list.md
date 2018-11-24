# <a name="list-organizations"></a><span data-ttu-id="3d963-101">Listar organizations</span><span class="sxs-lookup"><span data-stu-id="3d963-101">List organizations</span></span>

> <span data-ttu-id="3d963-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3d963-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3d963-103">Listar propriedades e relações de objetos de [organização](../resources/intune_onboarding_organization.md).</span><span class="sxs-lookup"><span data-stu-id="3d963-103">List properties and relationships of the [organization](../resources/intune_onboarding_organization.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3d963-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3d963-104">Prerequisites</span></span>
<span data-ttu-id="3d963-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3d963-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3d963-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3d963-107">Permission type</span></span>|<span data-ttu-id="3d963-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3d963-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d963-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3d963-109">Delegated (work or school account)</span></span>|<span data-ttu-id="3d963-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d963-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="3d963-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3d963-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d963-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d963-112">Not supported.</span></span>|
|<span data-ttu-id="3d963-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3d963-113">Application</span></span>|<span data-ttu-id="3d963-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d963-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d963-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d963-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization
```

## <a name="request-headers"></a><span data-ttu-id="3d963-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3d963-116">Request headers</span></span>
|<span data-ttu-id="3d963-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3d963-117">Header</span></span>|<span data-ttu-id="3d963-118">Valor</span><span class="sxs-lookup"><span data-stu-id="3d963-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d963-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="3d963-119">Authorization</span></span>|<span data-ttu-id="3d963-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d963-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d963-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3d963-121">Accept</span></span>|<span data-ttu-id="3d963-122">application/json</span><span class="sxs-lookup"><span data-stu-id="3d963-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d963-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3d963-123">Request body</span></span>
<span data-ttu-id="3d963-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3d963-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d963-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d963-125">Response</span></span>
<span data-ttu-id="3d963-126">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [organization](../resources/intune_onboarding_organization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d963-126">If successful, this method returns a `200 OK` response code and a collection of [organization](../resources/intune_onboarding_organization.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d963-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3d963-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="3d963-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d963-128">Request</span></span>
<span data-ttu-id="3d963-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3d963-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/organization
```

### <a name="response"></a><span data-ttu-id="3d963-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d963-130">Response</span></span>
<span data-ttu-id="3d963-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3d963-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 196

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.organization",
      "id": "9efe224a-224a-9efe-4a22-fe9e4a22fe9e",
      "mobileDeviceManagementAuthority": "intune"
    }
  ]
}
```



