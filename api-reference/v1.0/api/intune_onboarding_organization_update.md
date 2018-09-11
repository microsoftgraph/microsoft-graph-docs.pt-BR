# <a name="update-organization"></a><span data-ttu-id="01006-101">Atualize a organização</span><span class="sxs-lookup"><span data-stu-id="01006-101">Update organization</span></span>

> <span data-ttu-id="01006-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="01006-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="01006-103">Atualizar as propriedades de um objeto [organização](../resources/intune_onboarding_organization.md).</span><span class="sxs-lookup"><span data-stu-id="01006-103">Update the properties of a [organization](../resources/intune_onboarding_organization.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="01006-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="01006-104">Prerequisites</span></span>
<span data-ttu-id="01006-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="01006-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="01006-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01006-107">Permission type</span></span>|<span data-ttu-id="01006-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="01006-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01006-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01006-109">Delegated (work or school account)</span></span>|<span data-ttu-id="01006-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01006-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="01006-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01006-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01006-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01006-112">Not supported.</span></span>|
|<span data-ttu-id="01006-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01006-113">Application</span></span>|<span data-ttu-id="01006-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01006-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01006-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01006-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="01006-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01006-116">Request headers</span></span>
|<span data-ttu-id="01006-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="01006-117">Header</span></span>|<span data-ttu-id="01006-118">Valor</span><span class="sxs-lookup"><span data-stu-id="01006-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01006-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="01006-119">Authorization</span></span>|<span data-ttu-id="01006-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="01006-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01006-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="01006-121">Accept</span></span>|<span data-ttu-id="01006-122">aplicativo/json</span><span class="sxs-lookup"><span data-stu-id="01006-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01006-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01006-123">Request body</span></span>
<span data-ttu-id="01006-124">No corpo da solicitação, forneça uma representação JSON do objeto [organization](../resources/intune_onboarding_organization.md).</span><span class="sxs-lookup"><span data-stu-id="01006-124">In the request body, supply a JSON representation for the [organization](../resources/intune_onboarding_organization.md) object.</span></span>

<span data-ttu-id="01006-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [organization](../resources/intune_onboarding_organization.md).</span><span class="sxs-lookup"><span data-stu-id="01006-125">The following table shows the properties that are required when you create the [organization](../resources/intune_onboarding_organization.md).</span></span>

|<span data-ttu-id="01006-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01006-126">Property</span></span>|<span data-ttu-id="01006-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="01006-127">Type</span></span>|<span data-ttu-id="01006-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="01006-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01006-129">id</span><span class="sxs-lookup"><span data-stu-id="01006-129">id</span></span>|<span data-ttu-id="01006-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="01006-130">String</span></span>|<span data-ttu-id="01006-131">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="01006-131">The GUID for the object.</span></span>|
|<span data-ttu-id="01006-132">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="01006-132">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="01006-133">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="01006-133">mdmAuthority</span></span>](../resources/intune_onboarding_mdmauthority.md)|<span data-ttu-id="01006-p102">Autoridade de gerenciamento de dispositivo móvel. Os valores possíveis são: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="01006-p102">Mobile device management authority. The possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|



## <a name="response"></a><span data-ttu-id="01006-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="01006-136">Response</span></span>
<span data-ttu-id="01006-137">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [organization](../resources/intune_onboarding_organization.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01006-137">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune_onboarding_organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01006-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01006-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="01006-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01006-139">Request</span></span>
<span data-ttu-id="01006-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="01006-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/organization/{organizationId}
Content-type: application/json
Content-length: 51

{
  "mobileDeviceManagementAuthority": "intune"
}
```

### <a name="response"></a><span data-ttu-id="01006-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="01006-141">Response</span></span>
<span data-ttu-id="01006-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01006-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 151

{
  "@odata.type": "#microsoft.graph.organization",
  "id": "9efe224a-224a-9efe-4a22-fe9e4a22fe9e",
  "mobileDeviceManagementAuthority": "intune"
}
```








