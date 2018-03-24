# <a name="update-roleassignment"></a><span data-ttu-id="250c5-101">Atualizar roleAssignment</span><span class="sxs-lookup"><span data-stu-id="250c5-101">Update roleAssignment</span></span>

> <span data-ttu-id="250c5-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="250c5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="250c5-103">Atualizar as propriedades de um objeto [roleAssignment](../resources/intune_rbac_roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="250c5-103">Update the properties of a [calendar](../resources/intune_rbac_roleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="250c5-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="250c5-104">Prerequisites</span></span>
<span data-ttu-id="250c5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="250c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="250c5-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="250c5-107">Permission type</span></span>|<span data-ttu-id="250c5-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="250c5-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="250c5-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="250c5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="250c5-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="250c5-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="250c5-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="250c5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="250c5-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="250c5-112">Not supported.</span></span>|
|<span data-ttu-id="250c5-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="250c5-113">Application</span></span>|<span data-ttu-id="250c5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="250c5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="250c5-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="250c5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="250c5-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="250c5-116">Request headers</span></span>
|<span data-ttu-id="250c5-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="250c5-117">Header</span></span>|<span data-ttu-id="250c5-118">Valor</span><span class="sxs-lookup"><span data-stu-id="250c5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="250c5-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="250c5-119">Authorization</span></span>|<span data-ttu-id="250c5-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="250c5-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="250c5-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="250c5-121">Accept</span></span>|<span data-ttu-id="250c5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="250c5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="250c5-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="250c5-123">Request body</span></span>
<span data-ttu-id="250c5-124">No corpo da solicitação, forneça uma representação JSON do objeto [roleAssignment](../resources/intune_rbac_roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="250c5-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_rbac_roleassignment.md) object.</span></span>

<span data-ttu-id="250c5-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [roleAssignment](../resources/intune_rbac_roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="250c5-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="250c5-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="250c5-126">Property</span></span>|<span data-ttu-id="250c5-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="250c5-127">Type</span></span>|<span data-ttu-id="250c5-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="250c5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="250c5-129">id</span><span class="sxs-lookup"><span data-stu-id="250c5-129">id</span></span>|<span data-ttu-id="250c5-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="250c5-130">String</span></span>|<span data-ttu-id="250c5-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="250c5-131">Key of the setting.</span></span> <span data-ttu-id="250c5-132">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="250c5-132">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="250c5-133">displayName</span><span class="sxs-lookup"><span data-stu-id="250c5-133">displayName</span></span>|<span data-ttu-id="250c5-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="250c5-134">String</span></span>|<span data-ttu-id="250c5-135">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="250c5-135">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="250c5-136">descrição</span><span class="sxs-lookup"><span data-stu-id="250c5-136">description</span></span>|<span data-ttu-id="250c5-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="250c5-137">String</span></span>|<span data-ttu-id="250c5-138">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="250c5-138">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="250c5-139">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="250c5-139">resourceScopes</span></span>|<span data-ttu-id="250c5-140">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="250c5-140">String collection</span></span>|<span data-ttu-id="250c5-141">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="250c5-141">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="250c5-142">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="250c5-142">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="250c5-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="250c5-143">Response</span></span>
<span data-ttu-id="250c5-144">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [roleAssignment](../resources/intune_rbac_roleassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="250c5-144">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_rbac_roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="250c5-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="250c5-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="250c5-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="250c5-146">Request</span></span>
<span data-ttu-id="250c5-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="250c5-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
Content-type: application/json
Content-length: 140

{
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="250c5-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="250c5-148">Response</span></span>
<span data-ttu-id="250c5-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="250c5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



