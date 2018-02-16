# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="9bd8a-101">Tipo de recurso eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="9bd8a-101">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="9bd8a-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9bd8a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9bd8a-103">Contém propriedades do resumo da instalação de um livro para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9bd8a-103">Contains properties for the installation summary of a book for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="9bd8a-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="9bd8a-104">Methods</span></span>
|<span data-ttu-id="9bd8a-105">Método</span><span class="sxs-lookup"><span data-stu-id="9bd8a-105">Method</span></span>|<span data-ttu-id="9bd8a-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9bd8a-106">Return Type</span></span>|<span data-ttu-id="9bd8a-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bd8a-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9bd8a-108">Obter eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="9bd8a-108">Get eBookInstallSummary</span></span>](../api/intune_books_ebookinstallsummary_get.md)|[<span data-ttu-id="9bd8a-109">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="9bd8a-109">eBookInstallSummary</span></span>](../resources/intune_books_ebookinstallsummary.md)|<span data-ttu-id="9bd8a-110">Ler propriedades e relações de objetos de [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="9bd8a-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_books_ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="9bd8a-111">Atualizar eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="9bd8a-111">Update eBookInstallSummary</span></span>](../api/intune_books_ebookinstallsummary_update.md)|[<span data-ttu-id="9bd8a-112">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="9bd8a-112">eBookInstallSummary</span></span>](../resources/intune_books_ebookinstallsummary.md)|<span data-ttu-id="9bd8a-113">Atualizar as propriedades de um objeto de [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="9bd8a-113">Update the properties of a [calendar](../resources/intune_books_ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9bd8a-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9bd8a-114">Properties</span></span>
|<span data-ttu-id="9bd8a-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9bd8a-115">Property</span></span>|<span data-ttu-id="9bd8a-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="9bd8a-116">Type</span></span>|<span data-ttu-id="9bd8a-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bd8a-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bd8a-118">id</span><span class="sxs-lookup"><span data-stu-id="9bd8a-118">id</span></span>|<span data-ttu-id="9bd8a-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9bd8a-119">String</span></span>|<span data-ttu-id="9bd8a-120">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9bd8a-120">Key of the setting.</span></span>|
|<span data-ttu-id="9bd8a-121">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9bd8a-121">installedDeviceCount</span></span>|<span data-ttu-id="9bd8a-122">Int32</span><span class="sxs-lookup"><span data-stu-id="9bd8a-122">Int32</span></span>|<span data-ttu-id="9bd8a-123">Número de dispositivos que instalaram este livro com êxito.</span><span class="sxs-lookup"><span data-stu-id="9bd8a-123">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="9bd8a-124">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9bd8a-124">failedDeviceCount</span></span>|<span data-ttu-id="9bd8a-125">Int32</span><span class="sxs-lookup"><span data-stu-id="9bd8a-125">Int32</span></span>|<span data-ttu-id="9bd8a-126">Número de dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="9bd8a-126">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="9bd8a-127">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9bd8a-127">notInstalledDeviceCount</span></span>|<span data-ttu-id="9bd8a-128">Int32</span><span class="sxs-lookup"><span data-stu-id="9bd8a-128">Int32</span></span>|<span data-ttu-id="9bd8a-129">Número de dispositivos que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="9bd8a-129">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="9bd8a-130">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="9bd8a-130">installedUserCount</span></span>|<span data-ttu-id="9bd8a-131">Int32</span><span class="sxs-lookup"><span data-stu-id="9bd8a-131">Int32</span></span>|<span data-ttu-id="9bd8a-132">Número de usuários cujos dispositivos tiveram êxito ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="9bd8a-132">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="9bd8a-133">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="9bd8a-133">failedUserCount</span></span>|<span data-ttu-id="9bd8a-134">Int32</span><span class="sxs-lookup"><span data-stu-id="9bd8a-134">Int32</span></span>|<span data-ttu-id="9bd8a-135">Número de usuários que têm um ou mais dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="9bd8a-135">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="9bd8a-136">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="9bd8a-136">notInstalledUserCount</span></span>|<span data-ttu-id="9bd8a-137">Int32</span><span class="sxs-lookup"><span data-stu-id="9bd8a-137">Int32</span></span>|<span data-ttu-id="9bd8a-138">Número de usuários que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="9bd8a-138">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9bd8a-139">Relações</span><span class="sxs-lookup"><span data-stu-id="9bd8a-139">Relationships</span></span>
<span data-ttu-id="9bd8a-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9bd8a-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9bd8a-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9bd8a-141">JSON Representation</span></span>
<span data-ttu-id="9bd8a-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9bd8a-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.eBookInstallSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "id": "String (identifier)",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024,
  "installedUserCount": 1024,
  "failedUserCount": 1024,
  "notInstalledUserCount": 1024
}
```



