# <a name="update-managedebookassignment"></a><span data-ttu-id="9c81b-101">Atualizar managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="9c81b-101">Update managedEBookAssignment</span></span>

> <span data-ttu-id="9c81b-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9c81b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9c81b-103">Atualizar as propriedades de um objeto [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9c81b-103">Update the properties of a [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9c81b-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9c81b-104">Prerequisites</span></span>
<span data-ttu-id="9c81b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9c81b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9c81b-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c81b-107">Permission type</span></span>|<span data-ttu-id="9c81b-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9c81b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c81b-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c81b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9c81b-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c81b-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9c81b-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c81b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c81b-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c81b-112">Not supported.</span></span>|
|<span data-ttu-id="9c81b-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c81b-113">Application</span></span>|<span data-ttu-id="9c81b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c81b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c81b-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c81b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="9c81b-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c81b-116">Request headers</span></span>
|<span data-ttu-id="9c81b-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9c81b-117">Header</span></span>|<span data-ttu-id="9c81b-118">Valor</span><span class="sxs-lookup"><span data-stu-id="9c81b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c81b-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c81b-119">Authorization</span></span>|<span data-ttu-id="9c81b-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c81b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c81b-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9c81b-121">Accept</span></span>|<span data-ttu-id="9c81b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="9c81b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c81b-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c81b-123">Request body</span></span>
<span data-ttu-id="9c81b-124">No corpo da solicitação, forneça uma representação JSON do objeto [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9c81b-124">In the request body, supply a JSON representation for the [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) object.</span></span>

<span data-ttu-id="9c81b-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9c81b-125">The following table shows the properties that are required when you create the [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).</span></span>

|<span data-ttu-id="9c81b-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c81b-126">Property</span></span>|<span data-ttu-id="9c81b-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c81b-127">Type</span></span>|<span data-ttu-id="9c81b-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c81b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c81b-129">id</span><span class="sxs-lookup"><span data-stu-id="9c81b-129">id</span></span>|<span data-ttu-id="9c81b-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c81b-130">String</span></span>|<span data-ttu-id="9c81b-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9c81b-131">Key of the entity.</span></span>|
|<span data-ttu-id="9c81b-132">target</span><span class="sxs-lookup"><span data-stu-id="9c81b-132">target</span></span>|[<span data-ttu-id="9c81b-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9c81b-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9c81b-134">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="9c81b-134">The assignment target for eBook.</span></span>|
|<span data-ttu-id="9c81b-135">installIntent</span><span class="sxs-lookup"><span data-stu-id="9c81b-135">installIntent</span></span>|[<span data-ttu-id="9c81b-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="9c81b-136">installIntent</span></span>](../resources/intune_shared_installintent.md)|<span data-ttu-id="9c81b-137">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="9c81b-137">The install intent for eBook.</span></span> <span data-ttu-id="9c81b-138">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="9c81b-138">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="9c81b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c81b-139">Response</span></span>
<span data-ttu-id="9c81b-140">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c81b-140">If successful, this method returns a `200 OK` response code and an updated [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c81b-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9c81b-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="9c81b-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c81b-142">Request</span></span>
<span data-ttu-id="9c81b-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c81b-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
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

### <a name="response"></a><span data-ttu-id="9c81b-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c81b-144">Response</span></span>
<span data-ttu-id="9c81b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9c81b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



