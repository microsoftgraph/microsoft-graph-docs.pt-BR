# <a name="update-iosvppebookassignment"></a><span data-ttu-id="dd604-101">Atualizar iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="dd604-101">Update iosVppEBookAssignment</span></span>

> <span data-ttu-id="dd604-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="dd604-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dd604-103">Atualizar as propriedades de um objeto [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="dd604-103">Update the properties of a [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dd604-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dd604-104">Prerequisites</span></span>
<span data-ttu-id="dd604-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="dd604-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="dd604-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd604-107">Permission type</span></span>|<span data-ttu-id="dd604-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dd604-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd604-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd604-109">Delegated (work or school account)</span></span>|<span data-ttu-id="dd604-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd604-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dd604-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd604-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd604-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd604-112">Not supported.</span></span>|
|<span data-ttu-id="dd604-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd604-113">Application</span></span>|<span data-ttu-id="dd604-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd604-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd604-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd604-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="dd604-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd604-116">Request headers</span></span>
|<span data-ttu-id="dd604-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dd604-117">Header</span></span>|<span data-ttu-id="dd604-118">Valor</span><span class="sxs-lookup"><span data-stu-id="dd604-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd604-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd604-119">Authorization</span></span>|<span data-ttu-id="dd604-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="dd604-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd604-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dd604-121">Accept</span></span>|<span data-ttu-id="dd604-122">application/json</span><span class="sxs-lookup"><span data-stu-id="dd604-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd604-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dd604-123">Request body</span></span>
<span data-ttu-id="dd604-124">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="dd604-124">In the request body, supply a JSON representation for the [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="dd604-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="dd604-125">The following table shows the properties that are required when you create the [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md).</span></span>

|<span data-ttu-id="dd604-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd604-126">Property</span></span>|<span data-ttu-id="dd604-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd604-127">Type</span></span>|<span data-ttu-id="dd604-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd604-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd604-129">id</span><span class="sxs-lookup"><span data-stu-id="dd604-129">id</span></span>|<span data-ttu-id="dd604-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd604-130">String</span></span>|<span data-ttu-id="dd604-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="dd604-131">Key of the entity.</span></span> <span data-ttu-id="dd604-132">Herda do [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="dd604-132">Inherited from [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span></span>|
|<span data-ttu-id="dd604-133">destino</span><span class="sxs-lookup"><span data-stu-id="dd604-133">target</span></span>|[<span data-ttu-id="dd604-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="dd604-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="dd604-135">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="dd604-135">The assignment target for eBook.</span></span> <span data-ttu-id="dd604-136">Herda do [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="dd604-136">Inherited from [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span></span>|
|<span data-ttu-id="dd604-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="dd604-137">installIntent</span></span>|[<span data-ttu-id="dd604-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="dd604-138">installIntent</span></span>](../resources/intune_shared_installintent.md)|<span data-ttu-id="dd604-139">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="dd604-139">The install intent for eBook.</span></span> <span data-ttu-id="dd604-140">Herdado de [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="dd604-140">Inherited from [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span></span> <span data-ttu-id="dd604-141">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="dd604-141">The possible values are `available`, `required`, `uninstall`, `availableWithoutEnrollment`, , , , , , , , or .</span></span>|



## <a name="response"></a><span data-ttu-id="dd604-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd604-142">Response</span></span>
<span data-ttu-id="dd604-143">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd604-143">If successful, this method returns a `200 OK` response code and an updated [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd604-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dd604-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="dd604-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd604-145">Request</span></span>
<span data-ttu-id="dd604-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd604-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
Content-type: application/json
Content-length: 133

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="dd604-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd604-147">Response</span></span>
<span data-ttu-id="dd604-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dd604-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "id": "48f05789-5789-48f0-8957-f0488957f048",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```



