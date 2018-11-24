# <a name="create-deviceandappmanagementroledefinition"></a><span data-ttu-id="7f7e9-101">Criar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7f7e9-101">Create deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="7f7e9-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7f7e9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7f7e9-103">Cria um novo objeto [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="7f7e9-103">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7f7e9-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7f7e9-104">Prerequisites</span></span>
<span data-ttu-id="7f7e9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7f7e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7f7e9-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f7e9-107">Permission type</span></span>|<span data-ttu-id="7f7e9-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7f7e9-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f7e9-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f7e9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7f7e9-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f7e9-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="7f7e9-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f7e9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f7e9-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f7e9-112">Not supported.</span></span>|
|<span data-ttu-id="7f7e9-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f7e9-113">Application</span></span>|<span data-ttu-id="7f7e9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f7e9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f7e9-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f7e9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="7f7e9-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f7e9-116">Request headers</span></span>
|<span data-ttu-id="7f7e9-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7f7e9-117">Header</span></span>|<span data-ttu-id="7f7e9-118">Valor</span><span class="sxs-lookup"><span data-stu-id="7f7e9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f7e9-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f7e9-119">Authorization</span></span>|<span data-ttu-id="7f7e9-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f7e9-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f7e9-121">Accept</span><span class="sxs-lookup"><span data-stu-id="7f7e9-121">Accept</span></span>|<span data-ttu-id="7f7e9-122">application/json</span><span class="sxs-lookup"><span data-stu-id="7f7e9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f7e9-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f7e9-123">Request body</span></span>
<span data-ttu-id="7f7e9-124">No corpo da solicitação, forneça uma representação JSON do objeto deviceAndAppManagementRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="7f7e9-124">In the request body, supply a JSON representation for the deviceAndAppManagementRoleDefinition object.</span></span>

<span data-ttu-id="7f7e9-125">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceAndAppManagementRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="7f7e9-125">The following table shows the properties that are required when you create the deviceAndAppManagementRoleDefinition.</span></span>

|<span data-ttu-id="7f7e9-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f7e9-126">Property</span></span>|<span data-ttu-id="7f7e9-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f7e9-127">Type</span></span>|<span data-ttu-id="7f7e9-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f7e9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f7e9-129">id</span><span class="sxs-lookup"><span data-stu-id="7f7e9-129">id</span></span>|<span data-ttu-id="7f7e9-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f7e9-130">String</span></span>|<span data-ttu-id="7f7e9-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7f7e9-131">Key of the entity.</span></span> <span data-ttu-id="7f7e9-132">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="7f7e9-132">This is read-only and automatically generated.</span></span> <span data-ttu-id="7f7e9-133">Herdado de [roleDefinition](../resources/intune_rbac_roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7f7e9-133">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|
|<span data-ttu-id="7f7e9-134">displayName</span><span class="sxs-lookup"><span data-stu-id="7f7e9-134">displayName</span></span>|<span data-ttu-id="7f7e9-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f7e9-135">String</span></span>|<span data-ttu-id="7f7e9-136">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="7f7e9-136">Display Name of the Role definition.</span></span> <span data-ttu-id="7f7e9-137">Herdado de [roleDefinition](../resources/intune_rbac_roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7f7e9-137">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|
|<span data-ttu-id="7f7e9-138">description</span><span class="sxs-lookup"><span data-stu-id="7f7e9-138">description</span></span>|<span data-ttu-id="7f7e9-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f7e9-139">String</span></span>|<span data-ttu-id="7f7e9-140">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="7f7e9-140">Description of the Role definition.</span></span> <span data-ttu-id="7f7e9-141">Herdado de [roleDefinition](../resources/intune_rbac_roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7f7e9-141">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|
|<span data-ttu-id="7f7e9-142">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="7f7e9-142">rolePermissions</span></span>|<span data-ttu-id="7f7e9-143">Coleção [rolePermission](../resources/intune_rbac_rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="7f7e9-143">[rolePermission](../resources/intune_rbac_rolepermission.md) collection</span></span>|<span data-ttu-id="7f7e9-144">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="7f7e9-144">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="7f7e9-145">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="7f7e9-145">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="7f7e9-146">Herdado de [roleDefinition](../resources/intune_rbac_roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7f7e9-146">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|
|<span data-ttu-id="7f7e9-147">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="7f7e9-147">isBuiltIn</span></span>|<span data-ttu-id="7f7e9-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="7f7e9-148">Boolean</span></span>|<span data-ttu-id="7f7e9-149">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="7f7e9-149">Type of Role.</span></span> <span data-ttu-id="7f7e9-150">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="7f7e9-150">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="7f7e9-151">Herdado de [roleDefinition](../resources/intune_rbac_roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7f7e9-151">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="7f7e9-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f7e9-152">Response</span></span>
<span data-ttu-id="7f7e9-153">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f7e9-153">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f7e9-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f7e9-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="7f7e9-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f7e9-155">Request</span></span>
<span data-ttu-id="7f7e9-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f7e9-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions
Content-type: application/json
Content-length: 602

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "displayName": "Display Name value",
  "description": "Description value",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="7f7e9-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f7e9-157">Response</span></span>
<span data-ttu-id="7f7e9-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7f7e9-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 651

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "id": "bca1dfb5-dfb5-bca1-b5df-a1bcb5dfa1bc",
  "displayName": "Display Name value",
  "description": "Description value",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```



