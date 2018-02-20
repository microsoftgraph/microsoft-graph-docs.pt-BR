# <a name="managedebook-resource-type"></a><span data-ttu-id="26075-101">Tipo de recurso managedEBook</span><span class="sxs-lookup"><span data-stu-id="26075-101">managedEBook resource type</span></span>

> <span data-ttu-id="26075-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="26075-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="26075-103">Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.</span><span class="sxs-lookup"><span data-stu-id="26075-103">An abstract class containing the base properties for Managed eBook.</span></span>
## <a name="methods"></a><span data-ttu-id="26075-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="26075-104">Methods</span></span>
|<span data-ttu-id="26075-105">Método</span><span class="sxs-lookup"><span data-stu-id="26075-105">Method</span></span>|<span data-ttu-id="26075-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="26075-106">Return Type</span></span>|<span data-ttu-id="26075-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="26075-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="26075-108">Listar managedEBooks</span><span class="sxs-lookup"><span data-stu-id="26075-108">List managedEBooks</span></span>](../api/intune_books_managedebook_list.md)|<span data-ttu-id="26075-109">Coleção [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="26075-109">[managedEBook](../resources/intune_books_managedebook.md) collection</span></span>|<span data-ttu-id="26075-110">Lista propriedades e relações dos objetos [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="26075-110">List properties and relationships of the [managedEBook](../resources/intune_books_managedebook.md) objects.</span></span>|
|[<span data-ttu-id="26075-111">Obter managedEBook</span><span class="sxs-lookup"><span data-stu-id="26075-111">Get managedEBook</span></span>](../api/intune_books_managedebook_get.md)|[<span data-ttu-id="26075-112">managedEBook</span><span class="sxs-lookup"><span data-stu-id="26075-112">managedEBook</span></span>](../resources/intune_books_managedebook.md)|<span data-ttu-id="26075-113">Propriedades de leitura e relações do objeto [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="26075-113">Read properties and relationships of [plannerPlanDetails](../resources/intune_books_managedebook.md) object.</span></span>|
|[<span data-ttu-id="26075-114">ação assign</span><span class="sxs-lookup"><span data-stu-id="26075-114">assign action</span></span>](../api/intune_books_managedebook_assign.md)|<span data-ttu-id="26075-115">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="26075-115">None</span></span>|<span data-ttu-id="26075-116">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="26075-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="26075-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="26075-117">Properties</span></span>
|<span data-ttu-id="26075-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26075-118">Property</span></span>|<span data-ttu-id="26075-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="26075-119">Type</span></span>|<span data-ttu-id="26075-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="26075-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26075-121">id</span><span class="sxs-lookup"><span data-stu-id="26075-121">id</span></span>|<span data-ttu-id="26075-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26075-122">String</span></span>|<span data-ttu-id="26075-123">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="26075-123">Key of the setting.</span></span>|
|<span data-ttu-id="26075-124">displayName</span><span class="sxs-lookup"><span data-stu-id="26075-124">displayName</span></span>|<span data-ttu-id="26075-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26075-125">String</span></span>|<span data-ttu-id="26075-126">Nome do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="26075-126">Name of the component.</span></span>|
|<span data-ttu-id="26075-127">description</span><span class="sxs-lookup"><span data-stu-id="26075-127">description</span></span>|<span data-ttu-id="26075-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26075-128">String</span></span>|<span data-ttu-id="26075-129">Descrição.</span><span class="sxs-lookup"><span data-stu-id="26075-129">Description.</span></span>|
|<span data-ttu-id="26075-130">publisher</span><span class="sxs-lookup"><span data-stu-id="26075-130">Publisher</span></span>|<span data-ttu-id="26075-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26075-131">String</span></span>|<span data-ttu-id="26075-132">Publicador.</span><span class="sxs-lookup"><span data-stu-id="26075-132">Publisher</span></span>|
|<span data-ttu-id="26075-133">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="26075-133">publishedDateTime</span></span>|<span data-ttu-id="26075-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26075-134">DateTimeOffset</span></span>|<span data-ttu-id="26075-135">A data e hora em que o livro eletrônico foi publicado.</span><span class="sxs-lookup"><span data-stu-id="26075-135">The date and time when the notebook was created.</span></span>|
|<span data-ttu-id="26075-136">largeCover</span><span class="sxs-lookup"><span data-stu-id="26075-136">largeCover</span></span>|[<span data-ttu-id="26075-137">mimeContent</span><span class="sxs-lookup"><span data-stu-id="26075-137">mimeContent</span></span>](../resources/intune_books_mimecontent.md)|<span data-ttu-id="26075-138">Capa do livro.</span><span class="sxs-lookup"><span data-stu-id="26075-138">Book cover.</span></span>|
|<span data-ttu-id="26075-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="26075-139">createdDateTime</span></span>|<span data-ttu-id="26075-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26075-140">DateTimeOffset</span></span>|<span data-ttu-id="26075-141">A data e hora em que o livro eletrônico foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="26075-141">The date and time when the notebook was created.</span></span>|
|<span data-ttu-id="26075-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="26075-142">lastModifiedDateTime</span></span>|<span data-ttu-id="26075-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26075-143">DateTimeOffset</span></span>|<span data-ttu-id="26075-144">A data e hora da última modificação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="26075-144">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="26075-145">informationUrl</span><span class="sxs-lookup"><span data-stu-id="26075-145">informationUrl</span></span>|<span data-ttu-id="26075-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26075-146">String</span></span>|<span data-ttu-id="26075-147">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="26075-147">The more information Url.</span></span>|
|<span data-ttu-id="26075-148">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="26075-148">privacyInformationUrl</span></span>|<span data-ttu-id="26075-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26075-149">String</span></span>|<span data-ttu-id="26075-150">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="26075-150">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26075-151">Relações</span><span class="sxs-lookup"><span data-stu-id="26075-151">Relationships</span></span>
|<span data-ttu-id="26075-152">Relação</span><span class="sxs-lookup"><span data-stu-id="26075-152">Relationship</span></span>|<span data-ttu-id="26075-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="26075-153">Type</span></span>|<span data-ttu-id="26075-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="26075-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26075-155">assignments</span><span class="sxs-lookup"><span data-stu-id="26075-155">assignments</span></span>|<span data-ttu-id="26075-156">Coleção [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="26075-156">[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) collection</span></span>|<span data-ttu-id="26075-157">A lista de atribuições para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="26075-157">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="26075-158">installSummary</span><span class="sxs-lookup"><span data-stu-id="26075-158">installSummary</span></span>|[<span data-ttu-id="26075-159">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="26075-159">eBookInstallSummary</span></span>](../resources/intune_books_ebookinstallsummary.md)|<span data-ttu-id="26075-160">Resumo de instalação do aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="26075-160">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="26075-161">deviceStates</span><span class="sxs-lookup"><span data-stu-id="26075-161">deviceStates</span></span>|<span data-ttu-id="26075-162">Coleção [deviceInstallState](../resources/intune_books_deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="26075-162">[deviceInstallState](../resources/intune_books_deviceinstallstate.md) collection</span></span>|<span data-ttu-id="26075-163">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="26075-163">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="26075-164">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="26075-164">userStateSummary</span></span>|<span data-ttu-id="26075-165">Coleção [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="26075-165">[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="26075-166">A lista de estados de instalação para este livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="26075-166">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="26075-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="26075-167">JSON Representation</span></span>
<span data-ttu-id="26075-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="26075-168">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBook",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "publishedDateTime": "String (timestamp)",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "informationUrl": "String",
  "privacyInformationUrl": "String"
}
```



