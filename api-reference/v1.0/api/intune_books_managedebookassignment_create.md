# <a name="create-managedebookassignment"></a><span data-ttu-id="0f598-101">Criar managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="0f598-101">Create managedEBookAssignment</span></span>

> <span data-ttu-id="0f598-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0f598-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f598-103">Criar um novo objeto [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0f598-103">Create a new [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0f598-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0f598-104">Prerequisites</span></span>
<span data-ttu-id="0f598-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0f598-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0f598-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f598-107">Permission type</span></span>|<span data-ttu-id="0f598-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0f598-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f598-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f598-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0f598-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f598-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0f598-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f598-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f598-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f598-112">Not supported.</span></span>|
|<span data-ttu-id="0f598-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f598-113">Application</span></span>|<span data-ttu-id="0f598-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f598-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f598-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f598-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="0f598-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f598-116">Request headers</span></span>
|<span data-ttu-id="0f598-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0f598-117">Header</span></span>|<span data-ttu-id="0f598-118">Valor</span><span class="sxs-lookup"><span data-stu-id="0f598-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f598-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f598-119">Authorization</span></span>|<span data-ttu-id="0f598-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="0f598-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f598-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0f598-121">Accept</span></span>|<span data-ttu-id="0f598-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0f598-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f598-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f598-123">Request body</span></span>
<span data-ttu-id="0f598-124">No corpo da solicitação, forneça uma representação JSON do objeto managedEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="0f598-124">In the request body, supply a JSON representation for the managedEBookAssignment object.</span></span>

<span data-ttu-id="0f598-125">A tabela a seguir mostra as propriedades que são necessárias ao criar managedEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="0f598-125">The following table shows the properties that are required when you create the managedEBookAssignment.</span></span>

|<span data-ttu-id="0f598-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f598-126">Property</span></span>|<span data-ttu-id="0f598-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f598-127">Type</span></span>|<span data-ttu-id="0f598-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f598-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f598-129">id</span><span class="sxs-lookup"><span data-stu-id="0f598-129">id</span></span>|<span data-ttu-id="0f598-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f598-130">String</span></span>|<span data-ttu-id="0f598-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0f598-131">Key of the entity.</span></span>|
|<span data-ttu-id="0f598-132">destino</span><span class="sxs-lookup"><span data-stu-id="0f598-132">target</span></span>|[<span data-ttu-id="0f598-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="0f598-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="0f598-134">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="0f598-134">The assignment target for eBook.</span></span>|
|<span data-ttu-id="0f598-135">installIntent</span><span class="sxs-lookup"><span data-stu-id="0f598-135">installIntent</span></span>|[<span data-ttu-id="0f598-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="0f598-136">installIntent</span></span>](../resources/intune_shared_installintent.md)|<span data-ttu-id="0f598-137">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="0f598-137">The install intent for eBook.</span></span> <span data-ttu-id="0f598-138">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="0f598-138">The possible values are `available`, `required`, `uninstall`, `availableWithoutEnrollment`, , , , , , , , or .</span></span>|



## <a name="response"></a><span data-ttu-id="0f598-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f598-139">Response</span></span>
<span data-ttu-id="0f598-140">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f598-140">If successful, this method returns a `201 Created` response code and a [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f598-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0f598-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="0f598-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f598-142">Request</span></span>
<span data-ttu-id="0f598-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f598-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
Content-type: application/json
Content-length: 194

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="0f598-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f598-144">Response</span></span>
<span data-ttu-id="0f598-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0f598-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 243

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```



