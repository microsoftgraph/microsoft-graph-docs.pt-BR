# <a name="create-roleassignment"></a><span data-ttu-id="777d4-101">Criar roleAssignment</span><span class="sxs-lookup"><span data-stu-id="777d4-101">Create roleAssignment</span></span>

> <span data-ttu-id="777d4-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="777d4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="777d4-103">Criar um novo objeto [roleAssignment](../resources/intune_rbac_roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="777d4-103">Create a new [roleAssignment](../resources/intune_rbac_roleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="777d4-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="777d4-104">Prerequisites</span></span>
<span data-ttu-id="777d4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="777d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="777d4-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="777d4-107">Permission type</span></span>|<span data-ttu-id="777d4-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="777d4-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="777d4-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="777d4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="777d4-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="777d4-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="777d4-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="777d4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="777d4-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="777d4-112">Not supported.</span></span>|
|<span data-ttu-id="777d4-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="777d4-113">Application</span></span>|<span data-ttu-id="777d4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="777d4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="777d4-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="777d4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="777d4-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="777d4-116">Request headers</span></span>
|<span data-ttu-id="777d4-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="777d4-117">Header</span></span>|<span data-ttu-id="777d4-118">Valor</span><span class="sxs-lookup"><span data-stu-id="777d4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="777d4-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="777d4-119">Authorization</span></span>|<span data-ttu-id="777d4-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="777d4-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="777d4-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="777d4-121">Accept</span></span>|<span data-ttu-id="777d4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="777d4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="777d4-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="777d4-123">Request body</span></span>
<span data-ttu-id="777d4-124">No corpo da solicitação, forneça uma representação JSON do objeto roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="777d4-124">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="777d4-125">A tabela a seguir mostra as propriedades que são necessárias ao criar roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="777d4-125">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="777d4-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="777d4-126">Property</span></span>|<span data-ttu-id="777d4-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="777d4-127">Type</span></span>|<span data-ttu-id="777d4-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="777d4-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="777d4-129">id</span><span class="sxs-lookup"><span data-stu-id="777d4-129">id</span></span>|<span data-ttu-id="777d4-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="777d4-130">String</span></span>|<span data-ttu-id="777d4-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="777d4-131">Key of the entity.</span></span> <span data-ttu-id="777d4-132">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="777d4-132">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="777d4-133">displayName</span><span class="sxs-lookup"><span data-stu-id="777d4-133">displayName</span></span>|<span data-ttu-id="777d4-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="777d4-134">String</span></span>|<span data-ttu-id="777d4-135">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="777d4-135">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="777d4-136">descrição</span><span class="sxs-lookup"><span data-stu-id="777d4-136">description</span></span>|<span data-ttu-id="777d4-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="777d4-137">String</span></span>|<span data-ttu-id="777d4-138">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="777d4-138">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="777d4-139">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="777d4-139">resourceScopes</span></span>|<span data-ttu-id="777d4-140">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="777d4-140">String collection</span></span>|<span data-ttu-id="777d4-141">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="777d4-141">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="777d4-142">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="777d4-142">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="777d4-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="777d4-143">Response</span></span>
<span data-ttu-id="777d4-144">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [roleAssignment](../resources/intune_rbac_roleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="777d4-144">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune_rbac_roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="777d4-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="777d4-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="777d4-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="777d4-146">Request</span></span>
<span data-ttu-id="777d4-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="777d4-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
Content-type: application/json
Content-length: 193

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="777d4-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="777d4-148">Response</span></span>
<span data-ttu-id="777d4-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="777d4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```








