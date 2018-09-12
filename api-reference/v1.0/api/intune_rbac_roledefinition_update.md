# <a name="update-roledefinition"></a><span data-ttu-id="771d8-101">Atualizar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="771d8-101">Update roleDefinition</span></span>

> <span data-ttu-id="771d8-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="771d8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="771d8-103">Atualizar as propriedades de um objeto [roleDefinition](../resources/intune_rbac_roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="771d8-103">Update the properties of a [roleDefinition](../resources/intune_rbac_roledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="771d8-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="771d8-104">Prerequisites</span></span>
<span data-ttu-id="771d8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="771d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="771d8-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="771d8-107">Permission type</span></span>|<span data-ttu-id="771d8-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="771d8-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="771d8-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="771d8-109">Delegated (work or school account)</span></span>|<span data-ttu-id="771d8-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="771d8-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="771d8-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="771d8-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="771d8-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="771d8-112">Not supported.</span></span>|
|<span data-ttu-id="771d8-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="771d8-113">Application</span></span>|<span data-ttu-id="771d8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="771d8-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="771d8-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="771d8-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="771d8-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="771d8-116">Request headers</span></span>
|<span data-ttu-id="771d8-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="771d8-117">Header</span></span>|<span data-ttu-id="771d8-118">Valor</span><span class="sxs-lookup"><span data-stu-id="771d8-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="771d8-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="771d8-119">Authorization</span></span>|<span data-ttu-id="771d8-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="771d8-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="771d8-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="771d8-121">Accept</span></span>|<span data-ttu-id="771d8-122">application/json</span><span class="sxs-lookup"><span data-stu-id="771d8-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="771d8-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="771d8-123">Request body</span></span>
<span data-ttu-id="771d8-124">No corpo da solicitação, forneça uma representação JSON do objeto [roleDefinition](../resources/intune_rbac_roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="771d8-124">In the request body, supply a JSON representation for the [roleDefinition](../resources/intune_rbac_roledefinition.md) object.</span></span>

<span data-ttu-id="771d8-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [roleDefinition](../resources/intune_rbac_roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="771d8-125">The following table shows the properties that are required when you create the [roleDefinition](../resources/intune_rbac_roledefinition.md).</span></span>

|<span data-ttu-id="771d8-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="771d8-126">Property</span></span>|<span data-ttu-id="771d8-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="771d8-127">Type</span></span>|<span data-ttu-id="771d8-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="771d8-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="771d8-129">id</span><span class="sxs-lookup"><span data-stu-id="771d8-129">id</span></span>|<span data-ttu-id="771d8-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="771d8-130">String</span></span>|<span data-ttu-id="771d8-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="771d8-131">Key of the entity.</span></span> <span data-ttu-id="771d8-132">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="771d8-132">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="771d8-133">displayName</span><span class="sxs-lookup"><span data-stu-id="771d8-133">displayName</span></span>|<span data-ttu-id="771d8-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="771d8-134">String</span></span>|<span data-ttu-id="771d8-135">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="771d8-135">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="771d8-136">description</span><span class="sxs-lookup"><span data-stu-id="771d8-136">description</span></span>|<span data-ttu-id="771d8-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="771d8-137">String</span></span>|<span data-ttu-id="771d8-138">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="771d8-138">Description of the Role definition.</span></span>|
|<span data-ttu-id="771d8-139">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="771d8-139">rolePermissions</span></span>|<span data-ttu-id="771d8-140">Coleção [rolePermission](../resources/intune_rbac_rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="771d8-140">[rolePermission](../resources/intune_rbac_rolepermission.md) collection</span></span>|<span data-ttu-id="771d8-141">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="771d8-141">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="771d8-142">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="771d8-142">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="771d8-143">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="771d8-143">isBuiltIn</span></span>|<span data-ttu-id="771d8-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="771d8-144">Boolean</span></span>|<span data-ttu-id="771d8-145">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="771d8-145">Type of Role.</span></span> <span data-ttu-id="771d8-146">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="771d8-146">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|



## <a name="response"></a><span data-ttu-id="771d8-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="771d8-147">Response</span></span>
<span data-ttu-id="771d8-148">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [roleDefinition](../resources/intune_rbac_roledefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="771d8-148">If successful, this method returns a `200 OK` response code and an updated [roleDefinition](../resources/intune_rbac_roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="771d8-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="771d8-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="771d8-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="771d8-150">Request</span></span>
<span data-ttu-id="771d8-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="771d8-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}
Content-type: application/json
Content-length: 527

{
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

### <a name="response"></a><span data-ttu-id="771d8-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="771d8-152">Response</span></span>
<span data-ttu-id="771d8-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="771d8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 629

{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "id": "70fdcd08-cd08-70fd-08cd-fd7008cdfd70",
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








