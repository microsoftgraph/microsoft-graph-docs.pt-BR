# <a name="update-onpremisesconditionalaccesssettings"></a><span data-ttu-id="aa9d3-101">Atualizar onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="aa9d3-101">Update onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="aa9d3-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="aa9d3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aa9d3-103">Atualizar as propriedades de um objeto [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="aa9d3-103">Update the properties of a [calendar](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aa9d3-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aa9d3-104">Prerequisites</span></span>
<span data-ttu-id="aa9d3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="aa9d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="aa9d3-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aa9d3-107">Permission type</span></span>|<span data-ttu-id="aa9d3-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aa9d3-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa9d3-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aa9d3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="aa9d3-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa9d3-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="aa9d3-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aa9d3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa9d3-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa9d3-112">Not supported.</span></span>|
|<span data-ttu-id="aa9d3-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aa9d3-113">Application</span></span>|<span data-ttu-id="aa9d3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa9d3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa9d3-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa9d3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/conditionalAccessSettings
```

## <a name="request-headers"></a><span data-ttu-id="aa9d3-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa9d3-116">Request headers</span></span>
|<span data-ttu-id="aa9d3-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aa9d3-117">Header</span></span>|<span data-ttu-id="aa9d3-118">Valor</span><span class="sxs-lookup"><span data-stu-id="aa9d3-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa9d3-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa9d3-119">Authorization</span></span>|<span data-ttu-id="aa9d3-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa9d3-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="aa9d3-121">Accept</span><span class="sxs-lookup"><span data-stu-id="aa9d3-121">Accept</span></span>|<span data-ttu-id="aa9d3-122">application/json</span><span class="sxs-lookup"><span data-stu-id="aa9d3-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa9d3-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa9d3-123">Request body</span></span>
<span data-ttu-id="aa9d3-124">No corpo da solicitação, forneça uma representação JSON do objeto [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="aa9d3-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object.</span></span>

<span data-ttu-id="aa9d3-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="aa9d3-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="aa9d3-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aa9d3-126">Property</span></span>|<span data-ttu-id="aa9d3-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa9d3-127">Type</span></span>|<span data-ttu-id="aa9d3-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa9d3-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa9d3-129">id</span><span class="sxs-lookup"><span data-stu-id="aa9d3-129">id</span></span>|<span data-ttu-id="aa9d3-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa9d3-130">String</span></span>|<span data-ttu-id="aa9d3-131">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="aa9d3-131">Not yet documented</span></span>|
|<span data-ttu-id="aa9d3-132">enabled</span><span class="sxs-lookup"><span data-stu-id="aa9d3-132">enabled</span></span>|<span data-ttu-id="aa9d3-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="aa9d3-133">Boolean</span></span>|<span data-ttu-id="aa9d3-134">Indica se o acesso condicional local está habilitado para esta organização</span><span class="sxs-lookup"><span data-stu-id="aa9d3-134">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="aa9d3-135">includedGroups</span><span class="sxs-lookup"><span data-stu-id="aa9d3-135">includedGroups</span></span>|<span data-ttu-id="aa9d3-136">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="aa9d3-136">Guid collection</span></span>|<span data-ttu-id="aa9d3-137">Grupos de usuários que serão direcionados pelo acesso condicional local.</span><span class="sxs-lookup"><span data-stu-id="aa9d3-137">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="aa9d3-138">Todos os usuários nesses grupos deverão ter dispositivos móveis gerenciados e compatíveis com o acesso a email.</span><span class="sxs-lookup"><span data-stu-id="aa9d3-138">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="aa9d3-139">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="aa9d3-139">excludedGroups</span></span>|<span data-ttu-id="aa9d3-140">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="aa9d3-140">Guid collection</span></span>|<span data-ttu-id="aa9d3-141">Grupos de usuários que estarão isentos ao acesso condicional local.</span><span class="sxs-lookup"><span data-stu-id="aa9d3-141">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="aa9d3-142">Todos os usuários desses grupos ficarão isentos da política de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="aa9d3-142">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="aa9d3-143">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="aa9d3-143">overrideDefaultRule</span></span>|<span data-ttu-id="aa9d3-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="aa9d3-144">Boolean</span></span>|<span data-ttu-id="aa9d3-145">Substitui as regras de acesso padrão ao permitir a um dispositivo que seja concedida a garantia de acesso.</span><span class="sxs-lookup"><span data-stu-id="aa9d3-145">Override the default access rule when allowing a device to ensure access is granted.</span></span>|



## <a name="response"></a><span data-ttu-id="aa9d3-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa9d3-146">Response</span></span>
<span data-ttu-id="aa9d3-147">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa9d3-147">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa9d3-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aa9d3-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="aa9d3-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa9d3-149">Request</span></span>
<span data-ttu-id="aa9d3-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa9d3-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/conditionalAccessSettings
Content-type: application/json
Content-length: 195

{
  "enabled": true,
  "includedGroups": [
    "<Unknown Primitive Type Edm.Guid>"
  ],
  "excludedGroups": [
    "<Unknown Primitive Type Edm.Guid>"
  ],
  "overrideDefaultRule": true
}
```

### <a name="response"></a><span data-ttu-id="aa9d3-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa9d3-151">Response</span></span>
<span data-ttu-id="aa9d3-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aa9d3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 318

{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "a0efde21-de21-a0ef-21de-efa021deefa0",
  "enabled": true,
  "includedGroups": [
    "<Unknown Primitive Type Edm.Guid>"
  ],
  "excludedGroups": [
    "<Unknown Primitive Type Edm.Guid>"
  ],
  "overrideDefaultRule": true
}
```



