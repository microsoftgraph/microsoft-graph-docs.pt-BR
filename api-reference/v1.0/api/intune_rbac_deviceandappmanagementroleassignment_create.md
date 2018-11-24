# <a name="create-deviceandappmanagementroleassignment"></a><span data-ttu-id="b41dc-101">Criar deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="b41dc-101">Create deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="b41dc-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b41dc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b41dc-103">Cria um novo objeto [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b41dc-103">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b41dc-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b41dc-104">Prerequisites</span></span>
<span data-ttu-id="b41dc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b41dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b41dc-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b41dc-107">Permission type</span></span>|<span data-ttu-id="b41dc-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b41dc-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b41dc-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b41dc-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b41dc-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b41dc-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="b41dc-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b41dc-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b41dc-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b41dc-112">Not supported.</span></span>|
|<span data-ttu-id="b41dc-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b41dc-113">Application</span></span>|<span data-ttu-id="b41dc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b41dc-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b41dc-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b41dc-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="b41dc-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b41dc-116">Request headers</span></span>
|<span data-ttu-id="b41dc-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b41dc-117">Header</span></span>|<span data-ttu-id="b41dc-118">Valor</span><span class="sxs-lookup"><span data-stu-id="b41dc-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b41dc-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="b41dc-119">Authorization</span></span>|<span data-ttu-id="b41dc-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b41dc-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b41dc-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b41dc-121">Accept</span></span>|<span data-ttu-id="b41dc-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b41dc-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b41dc-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b41dc-123">Request body</span></span>
<span data-ttu-id="b41dc-124">No corpo da solicitação, forneça uma representação JSON do objeto deviceAndAppManagementRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="b41dc-124">In the request body, supply a JSON representation for the deviceAndAppManagementRoleAssignment object.</span></span>

<span data-ttu-id="b41dc-125">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceAndAppManagementRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="b41dc-125">The following table shows the properties that are required when you create the deviceAndAppManagementRoleAssignment.</span></span>

|<span data-ttu-id="b41dc-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b41dc-126">Property</span></span>|<span data-ttu-id="b41dc-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="b41dc-127">Type</span></span>|<span data-ttu-id="b41dc-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="b41dc-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b41dc-129">id</span><span class="sxs-lookup"><span data-stu-id="b41dc-129">id</span></span>|<span data-ttu-id="b41dc-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b41dc-130">String</span></span>|<span data-ttu-id="b41dc-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b41dc-131">Key of the entity.</span></span> <span data-ttu-id="b41dc-132">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="b41dc-132">This is read-only and automatically generated.</span></span> <span data-ttu-id="b41dc-133">Herdado de [roleAssignment](../resources/intune_rbac_roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b41dc-133">Inherited from [roleAssignment](../resources/intune_rbac_roleassignment.md)</span></span>|
|<span data-ttu-id="b41dc-134">displayName</span><span class="sxs-lookup"><span data-stu-id="b41dc-134">displayName</span></span>|<span data-ttu-id="b41dc-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b41dc-135">String</span></span>|<span data-ttu-id="b41dc-136">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="b41dc-136">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="b41dc-137">Herdado de [roleAssignment](../resources/intune_rbac_roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b41dc-137">Inherited from [roleAssignment](../resources/intune_rbac_roleassignment.md)</span></span>|
|<span data-ttu-id="b41dc-138">descrição</span><span class="sxs-lookup"><span data-stu-id="b41dc-138">description</span></span>|<span data-ttu-id="b41dc-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b41dc-139">String</span></span>|<span data-ttu-id="b41dc-140">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="b41dc-140">Description of the Role Assignment.</span></span> <span data-ttu-id="b41dc-141">Herdado de [roleAssignment](../resources/intune_rbac_roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b41dc-141">Inherited from [roleAssignment](../resources/intune_rbac_roleassignment.md)</span></span>|
|<span data-ttu-id="b41dc-142">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="b41dc-142">resourceScopes</span></span>|<span data-ttu-id="b41dc-143">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b41dc-143">String collection</span></span>|<span data-ttu-id="b41dc-144">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="b41dc-144">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="b41dc-145">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b41dc-145">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="b41dc-146">Herdado de [roleAssignment](../resources/intune_rbac_roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b41dc-146">Inherited from [roleAssignment](../resources/intune_rbac_roleassignment.md)</span></span>|
|<span data-ttu-id="b41dc-147">membros</span><span class="sxs-lookup"><span data-stu-id="b41dc-147">members</span></span>|<span data-ttu-id="b41dc-148">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b41dc-148">String collection</span></span>|<span data-ttu-id="b41dc-149">A lista de IDs de grupos de segurança de membros da função.</span><span class="sxs-lookup"><span data-stu-id="b41dc-149">The list of ids of role member security groups.</span></span> <span data-ttu-id="b41dc-150">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b41dc-150">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="b41dc-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="b41dc-151">Response</span></span>
<span data-ttu-id="b41dc-152">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b41dc-152">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b41dc-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b41dc-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="b41dc-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b41dc-154">Request</span></span>
<span data-ttu-id="b41dc-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b41dc-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments
Content-type: application/json
Content-length: 258

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="b41dc-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="b41dc-156">Response</span></span>
<span data-ttu-id="b41dc-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b41dc-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 307

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```



