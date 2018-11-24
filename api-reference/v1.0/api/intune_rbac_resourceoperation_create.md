# <a name="create-resourceoperation"></a><span data-ttu-id="29c64-101">Criar resourceOperation</span><span class="sxs-lookup"><span data-stu-id="29c64-101">Create resourceOperation</span></span>

> <span data-ttu-id="29c64-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="29c64-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="29c64-103">Criar um novo objeto [resourceOperation](../resources/intune_rbac_resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="29c64-103">Create a new [resourceOperation](../resources/intune_rbac_resourceoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="29c64-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="29c64-104">Prerequisites</span></span>
<span data-ttu-id="29c64-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="29c64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="29c64-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29c64-107">Permission type</span></span>|<span data-ttu-id="29c64-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="29c64-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29c64-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29c64-109">Delegated (work or school account)</span></span>|<span data-ttu-id="29c64-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29c64-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="29c64-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29c64-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29c64-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29c64-112">Not supported.</span></span>|
|<span data-ttu-id="29c64-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29c64-113">Application</span></span>|<span data-ttu-id="29c64-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29c64-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="29c64-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29c64-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="29c64-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29c64-116">Request headers</span></span>
|<span data-ttu-id="29c64-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="29c64-117">Header</span></span>|<span data-ttu-id="29c64-118">Valor</span><span class="sxs-lookup"><span data-stu-id="29c64-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29c64-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="29c64-119">Authorization</span></span>|<span data-ttu-id="29c64-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29c64-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29c64-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="29c64-121">Accept</span></span>|<span data-ttu-id="29c64-122">application/json</span><span class="sxs-lookup"><span data-stu-id="29c64-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29c64-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29c64-123">Request body</span></span>
<span data-ttu-id="29c64-124">No corpo da solicitação, forneça uma representação JSON do objeto resourceOperation.</span><span class="sxs-lookup"><span data-stu-id="29c64-124">In the request body, supply a JSON representation for the resourceOperation object.</span></span>

<span data-ttu-id="29c64-125">A tabela a seguir mostra as propriedades que são necessárias ao criar resourceOperation.</span><span class="sxs-lookup"><span data-stu-id="29c64-125">The following table shows the properties that are required when you create the resourceOperation.</span></span>

|<span data-ttu-id="29c64-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29c64-126">Property</span></span>|<span data-ttu-id="29c64-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="29c64-127">Type</span></span>|<span data-ttu-id="29c64-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="29c64-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29c64-129">id</span><span class="sxs-lookup"><span data-stu-id="29c64-129">id</span></span>|<span data-ttu-id="29c64-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29c64-130">String</span></span>|<span data-ttu-id="29c64-131">Chave da operação de recurso.</span><span class="sxs-lookup"><span data-stu-id="29c64-131">Key of the Resource Operation.</span></span> <span data-ttu-id="29c64-132">Somente leitura, gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="29c64-132">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="29c64-133">resourceName</span><span class="sxs-lookup"><span data-stu-id="29c64-133">resourceName</span></span>|<span data-ttu-id="29c64-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29c64-134">String</span></span>|<span data-ttu-id="29c64-135">Nome do recurso em que essa operação é executada.</span><span class="sxs-lookup"><span data-stu-id="29c64-135">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="29c64-136">actionName</span><span class="sxs-lookup"><span data-stu-id="29c64-136">actionName</span></span>|<span data-ttu-id="29c64-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29c64-137">String</span></span>|<span data-ttu-id="29c64-138">Tipo de ação em que essa operação será executada.</span><span class="sxs-lookup"><span data-stu-id="29c64-138">Type of action this operation is going to perform.</span></span> <span data-ttu-id="29c64-139">O actionName deve ser conciso e limitado ao mínimo de palavras possível.</span><span class="sxs-lookup"><span data-stu-id="29c64-139">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="29c64-140">descrição</span><span class="sxs-lookup"><span data-stu-id="29c64-140">description</span></span>|<span data-ttu-id="29c64-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29c64-141">String</span></span>|<span data-ttu-id="29c64-142">Descrição da operação de recurso.</span><span class="sxs-lookup"><span data-stu-id="29c64-142">Description of the resource operation.</span></span> <span data-ttu-id="29c64-143">A descrição é usada no texto exibido com o passar o mouse para a operação quando exibida no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="29c64-143">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="29c64-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="29c64-144">Response</span></span>
<span data-ttu-id="29c64-145">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [resourceOperation](../resources/intune_rbac_resourceoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29c64-145">If successful, this method returns a `201 Created` response code and a [resourceOperation](../resources/intune_rbac_resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29c64-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29c64-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="29c64-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29c64-147">Request</span></span>
<span data-ttu-id="29c64-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29c64-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations
Content-type: application/json
Content-length: 178

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="29c64-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="29c64-149">Response</span></span>
<span data-ttu-id="29c64-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29c64-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 227

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value"
}
```



