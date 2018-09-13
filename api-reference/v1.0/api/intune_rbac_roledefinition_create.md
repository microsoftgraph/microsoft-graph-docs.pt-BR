# <a name="create-roledefinition"></a><span data-ttu-id="eee50-101">Criar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="eee50-101">Create roleDefinition</span></span>

> <span data-ttu-id="eee50-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="eee50-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eee50-103">Criar um novo objeto [roleDefinition](../resources/intune_rbac_roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="eee50-103">Create a new [roleDefinition](../resources/intune_rbac_roledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eee50-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eee50-104">Prerequisites</span></span>
<span data-ttu-id="eee50-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="eee50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="eee50-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eee50-107">Permission type</span></span>|<span data-ttu-id="eee50-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eee50-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eee50-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eee50-109">Delegated (work or school account)</span></span>|<span data-ttu-id="eee50-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eee50-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="eee50-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eee50-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eee50-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eee50-112">Not supported.</span></span>|
|<span data-ttu-id="eee50-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eee50-113">Application</span></span>|<span data-ttu-id="eee50-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eee50-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eee50-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eee50-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="eee50-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eee50-116">Request headers</span></span>
|<span data-ttu-id="eee50-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eee50-117">Header</span></span>|<span data-ttu-id="eee50-118">Valor</span><span class="sxs-lookup"><span data-stu-id="eee50-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eee50-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="eee50-119">Authorization</span></span>|<span data-ttu-id="eee50-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="eee50-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eee50-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eee50-121">Accept</span></span>|<span data-ttu-id="eee50-122">application/json</span><span class="sxs-lookup"><span data-stu-id="eee50-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eee50-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eee50-123">Request body</span></span>
<span data-ttu-id="eee50-124">No corpo da solicitação, forneça uma representação JSON do objeto roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="eee50-124">In the request body, supply a JSON representation for the roleDefinition object.</span></span>

<span data-ttu-id="eee50-125">A tabela a seguir mostra as propriedades obrigatórias ao criar roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="eee50-125">The following table shows the properties that are required when you create the roleDefinition.</span></span>

|<span data-ttu-id="eee50-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eee50-126">Property</span></span>|<span data-ttu-id="eee50-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="eee50-127">Type</span></span>|<span data-ttu-id="eee50-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="eee50-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eee50-129">id</span><span class="sxs-lookup"><span data-stu-id="eee50-129">id</span></span>|<span data-ttu-id="eee50-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eee50-130">String</span></span>|<span data-ttu-id="eee50-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="eee50-131">Key of the entity.</span></span> <span data-ttu-id="eee50-132">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="eee50-132">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="eee50-133">displayName</span><span class="sxs-lookup"><span data-stu-id="eee50-133">displayName</span></span>|<span data-ttu-id="eee50-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eee50-134">String</span></span>|<span data-ttu-id="eee50-135">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="eee50-135">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="eee50-136">description</span><span class="sxs-lookup"><span data-stu-id="eee50-136">description</span></span>|<span data-ttu-id="eee50-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eee50-137">String</span></span>|<span data-ttu-id="eee50-138">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="eee50-138">Description of the Role definition.</span></span>|
|<span data-ttu-id="eee50-139">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="eee50-139">rolePermissions</span></span>|<span data-ttu-id="eee50-140">Coleção [rolePermission](../resources/intune_rbac_rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="eee50-140">[rolePermission](../resources/intune_rbac_rolepermission.md) collection</span></span>|<span data-ttu-id="eee50-141">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="eee50-141">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="eee50-142">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="eee50-142">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="eee50-143">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="eee50-143">isBuiltIn</span></span>|<span data-ttu-id="eee50-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="eee50-144">Boolean</span></span>|<span data-ttu-id="eee50-145">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="eee50-145">Type of Role.</span></span> <span data-ttu-id="eee50-146">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="eee50-146">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|



## <a name="response"></a><span data-ttu-id="eee50-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="eee50-147">Response</span></span>
<span data-ttu-id="eee50-148">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [roleDefinition](../resources/intune_rbac_roledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eee50-148">If successful, this method returns a `201 Created` response code and a [roleDefinition](../resources/intune_rbac_roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eee50-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eee50-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="eee50-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eee50-150">Request</span></span>
<span data-ttu-id="eee50-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eee50-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions
Content-type: application/json
Content-length: 580

{
  "@odata.type": "#microsoft.graph.roleDefinition",
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

### <a name="response"></a><span data-ttu-id="eee50-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="eee50-152">Response</span></span>
<span data-ttu-id="eee50-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eee50-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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








