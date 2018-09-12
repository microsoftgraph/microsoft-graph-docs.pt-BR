# <a name="update-iosvppebookassignment"></a><span data-ttu-id="16ccd-101">Atualizar iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="16ccd-101">Update iosVppEBookAssignment</span></span>

> <span data-ttu-id="16ccd-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="16ccd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16ccd-103">Atualizar as propriedades de um objeto [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="16ccd-103">Update the properties of a [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="16ccd-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="16ccd-104">Prerequisites</span></span>
<span data-ttu-id="16ccd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="16ccd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="16ccd-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16ccd-107">Permission type</span></span>|<span data-ttu-id="16ccd-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="16ccd-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16ccd-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16ccd-109">Delegated (work or school account)</span></span>|<span data-ttu-id="16ccd-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16ccd-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="16ccd-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16ccd-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16ccd-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16ccd-112">Not supported.</span></span>|
|<span data-ttu-id="16ccd-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16ccd-113">Application</span></span>|<span data-ttu-id="16ccd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16ccd-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16ccd-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16ccd-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="16ccd-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16ccd-116">Request headers</span></span>
|<span data-ttu-id="16ccd-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="16ccd-117">Header</span></span>|<span data-ttu-id="16ccd-118">Valor</span><span class="sxs-lookup"><span data-stu-id="16ccd-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16ccd-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="16ccd-119">Authorization</span></span>|<span data-ttu-id="16ccd-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="16ccd-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16ccd-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="16ccd-121">Accept</span></span>|<span data-ttu-id="16ccd-122">application/json</span><span class="sxs-lookup"><span data-stu-id="16ccd-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16ccd-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16ccd-123">Request body</span></span>
<span data-ttu-id="16ccd-124">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="16ccd-124">In the request body, supply a JSON representation for the [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="16ccd-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="16ccd-125">The following table shows the properties that are required when you create the [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md).</span></span>

|<span data-ttu-id="16ccd-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16ccd-126">Property</span></span>|<span data-ttu-id="16ccd-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="16ccd-127">Type</span></span>|<span data-ttu-id="16ccd-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="16ccd-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16ccd-129">id</span><span class="sxs-lookup"><span data-stu-id="16ccd-129">id</span></span>|<span data-ttu-id="16ccd-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16ccd-130">String</span></span>|<span data-ttu-id="16ccd-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="16ccd-131">Key of the entity.</span></span> <span data-ttu-id="16ccd-132">Herda do [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="16ccd-132">Inherited from [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span></span>|
|<span data-ttu-id="16ccd-133">destino</span><span class="sxs-lookup"><span data-stu-id="16ccd-133">target</span></span>|[<span data-ttu-id="16ccd-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="16ccd-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="16ccd-135">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="16ccd-135">The assignment target for eBook.</span></span> <span data-ttu-id="16ccd-136">Herda do [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="16ccd-136">Inherited from [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span></span>|
|<span data-ttu-id="16ccd-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="16ccd-137">installIntent</span></span>|[<span data-ttu-id="16ccd-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="16ccd-138">installIntent</span></span>](../resources/intune_shared_installintent.md)|<span data-ttu-id="16ccd-p104">A intenção de instalação para eBook. Herdada de [managedEBookAssignment](../resources/intune_books_managedebookassignment.md). os possíveis valores são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="16ccd-p104">The install intent for eBook. Inherited from [managedEBookAssignment](../resources/intune_books_managedebookassignment.md). The possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="16ccd-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="16ccd-142">Response</span></span>
<span data-ttu-id="16ccd-143">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16ccd-143">If successful, this method returns a `200 OK` response code and an updated [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16ccd-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="16ccd-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="16ccd-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16ccd-145">Request</span></span>
<span data-ttu-id="16ccd-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="16ccd-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="16ccd-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="16ccd-147">Response</span></span>
<span data-ttu-id="16ccd-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="16ccd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








