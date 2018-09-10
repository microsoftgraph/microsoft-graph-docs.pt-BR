# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="3254e-101">Tipo de recurso eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="3254e-101">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="3254e-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3254e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3254e-103">Contém propriedades do resumo da instalação de um livro para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3254e-103">Contains properties for the installation summary of a book for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="3254e-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="3254e-104">Methods</span></span>
|<span data-ttu-id="3254e-105">Método</span><span class="sxs-lookup"><span data-stu-id="3254e-105">Method</span></span>|<span data-ttu-id="3254e-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3254e-106">Return Type</span></span>|<span data-ttu-id="3254e-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="3254e-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3254e-108">Obter eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="3254e-108">Get eBookInstallSummary</span></span>](../api/intune_books_ebookinstallsummary_get.md)|[<span data-ttu-id="3254e-109">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="3254e-109">eBookInstallSummary</span></span>](../resources/intune_books_ebookinstallsummary.md)|<span data-ttu-id="3254e-110">Ler propriedades e relações de objetos de [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="3254e-110">Read properties and relationships of the [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="3254e-111">Atualizar eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="3254e-111">Update eBookInstallSummary</span></span>](../api/intune_books_ebookinstallsummary_update.md)|[<span data-ttu-id="3254e-112">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="3254e-112">eBookInstallSummary</span></span>](../resources/intune_books_ebookinstallsummary.md)|<span data-ttu-id="3254e-113">Atualizar as propriedades de um objeto de [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="3254e-113">Update the properties of a [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3254e-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3254e-114">Properties</span></span>
|<span data-ttu-id="3254e-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3254e-115">Property</span></span>|<span data-ttu-id="3254e-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="3254e-116">Type</span></span>|<span data-ttu-id="3254e-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="3254e-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3254e-118">id</span><span class="sxs-lookup"><span data-stu-id="3254e-118">id</span></span>|<span data-ttu-id="3254e-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3254e-119">String</span></span>|<span data-ttu-id="3254e-120">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3254e-120">Key of the entity.</span></span>|
|<span data-ttu-id="3254e-121">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3254e-121">installedDeviceCount</span></span>|<span data-ttu-id="3254e-122">Int32</span><span class="sxs-lookup"><span data-stu-id="3254e-122">Int32</span></span>|<span data-ttu-id="3254e-123">Número de dispositivos que instalaram este livro com êxito.</span><span class="sxs-lookup"><span data-stu-id="3254e-123">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="3254e-124">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3254e-124">failedDeviceCount</span></span>|<span data-ttu-id="3254e-125">Int32</span><span class="sxs-lookup"><span data-stu-id="3254e-125">Int32</span></span>|<span data-ttu-id="3254e-126">Número de dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="3254e-126">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="3254e-127">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3254e-127">notInstalledDeviceCount</span></span>|<span data-ttu-id="3254e-128">Int32</span><span class="sxs-lookup"><span data-stu-id="3254e-128">Int32</span></span>|<span data-ttu-id="3254e-129">Número de dispositivos que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="3254e-129">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="3254e-130">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="3254e-130">installedUserCount</span></span>|<span data-ttu-id="3254e-131">Int32</span><span class="sxs-lookup"><span data-stu-id="3254e-131">Int32</span></span>|<span data-ttu-id="3254e-132">Número de usuários cujos dispositivos tiveram êxito ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="3254e-132">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="3254e-133">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="3254e-133">failedUserCount</span></span>|<span data-ttu-id="3254e-134">Int32</span><span class="sxs-lookup"><span data-stu-id="3254e-134">Int32</span></span>|<span data-ttu-id="3254e-135">Número de usuários que têm um ou mais dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="3254e-135">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="3254e-136">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="3254e-136">notInstalledUserCount</span></span>|<span data-ttu-id="3254e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="3254e-137">Int32</span></span>|<span data-ttu-id="3254e-138">Número de usuários que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="3254e-138">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3254e-139">Relações</span><span class="sxs-lookup"><span data-stu-id="3254e-139">Relationships</span></span>
<span data-ttu-id="3254e-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3254e-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3254e-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3254e-141">JSON Representation</span></span>
<span data-ttu-id="3254e-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3254e-142">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.eBookInstallSummary"
}-->
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








