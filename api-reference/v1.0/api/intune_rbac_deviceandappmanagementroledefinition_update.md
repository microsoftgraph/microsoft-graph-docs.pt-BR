# <a name="update-deviceandappmanagementroledefinition"></a><span data-ttu-id="804f6-101">Atualizar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="804f6-101">Update deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="804f6-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="804f6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="804f6-103">Atualizar as propriedades de um objeto [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="804f6-103">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="804f6-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="804f6-104">Prerequisites</span></span>
<span data-ttu-id="804f6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="804f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="804f6-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="804f6-107">Permission type</span></span>|<span data-ttu-id="804f6-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="804f6-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="804f6-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="804f6-109">Delegated (work or school account)</span></span>|<span data-ttu-id="804f6-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="804f6-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="804f6-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="804f6-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="804f6-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="804f6-112">Not supported.</span></span>|
|<span data-ttu-id="804f6-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="804f6-113">Application</span></span>|<span data-ttu-id="804f6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="804f6-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="804f6-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="804f6-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="804f6-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="804f6-116">Request headers</span></span>
|<span data-ttu-id="804f6-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="804f6-117">Header</span></span>|<span data-ttu-id="804f6-118">Valor</span><span class="sxs-lookup"><span data-stu-id="804f6-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="804f6-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="804f6-119">Authorization</span></span>|<span data-ttu-id="804f6-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="804f6-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="804f6-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="804f6-121">Accept</span></span>|<span data-ttu-id="804f6-122">application/json</span><span class="sxs-lookup"><span data-stu-id="804f6-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="804f6-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="804f6-123">Request body</span></span>
<span data-ttu-id="804f6-124">No corpo da solicitação, forneça uma representação JSON do objeto [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="804f6-124">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) object.</span></span>

<span data-ttu-id="804f6-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="804f6-125">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md).</span></span>

|<span data-ttu-id="804f6-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="804f6-126">Property</span></span>|<span data-ttu-id="804f6-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="804f6-127">Type</span></span>|<span data-ttu-id="804f6-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="804f6-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="804f6-129">id</span><span class="sxs-lookup"><span data-stu-id="804f6-129">id</span></span>|<span data-ttu-id="804f6-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="804f6-130">String</span></span>|<span data-ttu-id="804f6-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="804f6-131">Key of the entity.</span></span> <span data-ttu-id="804f6-132">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="804f6-132">This is read-only and automatically generated.</span></span> <span data-ttu-id="804f6-133">Herdada de [roleDefinition](../resources/intune_rbac_roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="804f6-133">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|
|<span data-ttu-id="804f6-134">displayName</span><span class="sxs-lookup"><span data-stu-id="804f6-134">displayName</span></span>|<span data-ttu-id="804f6-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="804f6-135">String</span></span>|<span data-ttu-id="804f6-136">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="804f6-136">Display Name of the Role definition.</span></span> <span data-ttu-id="804f6-137">Herdada de [roleDefinition](../resources/intune_rbac_roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="804f6-137">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|
|<span data-ttu-id="804f6-138">descrição</span><span class="sxs-lookup"><span data-stu-id="804f6-138">description</span></span>|<span data-ttu-id="804f6-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="804f6-139">String</span></span>|<span data-ttu-id="804f6-140">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="804f6-140">Description of the Role definition.</span></span> <span data-ttu-id="804f6-141">Herdada de [roleDefinition](../resources/intune_rbac_roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="804f6-141">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|
|<span data-ttu-id="804f6-142">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="804f6-142">rolePermissions</span></span>|<span data-ttu-id="804f6-143">Coleção [rolePermission](../resources/intune_rbac_rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="804f6-143">[rolePermission](../resources/intune_rbac_rolepermission.md) collection</span></span>|<span data-ttu-id="804f6-144">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="804f6-144">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="804f6-145">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="804f6-145">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="804f6-146">Herdada de [roleDefinition](../resources/intune_rbac_roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="804f6-146">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|
|<span data-ttu-id="804f6-147">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="804f6-147">isBuiltIn</span></span>|<span data-ttu-id="804f6-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="804f6-148">Boolean</span></span>|<span data-ttu-id="804f6-149">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="804f6-149">Type of Role.</span></span> <span data-ttu-id="804f6-150">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="804f6-150">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="804f6-151">Herdada de [roleDefinition](../resources/intune_rbac_roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="804f6-151">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="804f6-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="804f6-152">Response</span></span>
<span data-ttu-id="804f6-153">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="804f6-153">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="804f6-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="804f6-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="804f6-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="804f6-155">Request</span></span>
<span data-ttu-id="804f6-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="804f6-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}
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

### <a name="response"></a><span data-ttu-id="804f6-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="804f6-157">Response</span></span>
<span data-ttu-id="804f6-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="804f6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



