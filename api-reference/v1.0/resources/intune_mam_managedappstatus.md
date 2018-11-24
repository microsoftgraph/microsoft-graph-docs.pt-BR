# <a name="managedappstatus-resource-type"></a><span data-ttu-id="b3319-101">Tipo de recurso managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="b3319-101">managedAppStatus resource type</span></span>

> <span data-ttu-id="b3319-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b3319-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3319-103">Representa o status de proteção e configuração do aplicativo para a organização.</span><span class="sxs-lookup"><span data-stu-id="b3319-103">Represents app protection and configuration status for the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="b3319-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="b3319-104">Methods</span></span>
|<span data-ttu-id="b3319-105">Método</span><span class="sxs-lookup"><span data-stu-id="b3319-105">Method</span></span>|<span data-ttu-id="b3319-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b3319-106">Return Type</span></span>|<span data-ttu-id="b3319-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3319-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b3319-108">Listar managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="b3319-108">List managedAppStatuses</span></span>](../api/intune_mam_managedappstatus_list.md)|<span data-ttu-id="b3319-109">Conjunto [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="b3319-109">[managedAppStatus](../resources/intune_mam_managedappstatus.md) collection</span></span>|<span data-ttu-id="b3319-110">Listar propriedades e as relações de objetos de [managedAppStatus](../resources/intune_mam_managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="b3319-110">List properties and relationships of the [managedAppStatus](../resources/intune_mam_managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="b3319-111">Obter managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="b3319-111">Get managedAppStatus</span></span>](../api/intune_mam_managedappstatus_get.md)|[<span data-ttu-id="b3319-112">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="b3319-112">managedAppStatus</span></span>](../resources/intune_mam_managedappstatus.md)|<span data-ttu-id="b3319-113">Ler propriedades e relações de objetos de [managedAppStatus](../resources/intune_mam_managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="b3319-113">Read properties and relationships of the [managedAppStatus](../resources/intune_mam_managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b3319-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b3319-114">Properties</span></span>
|<span data-ttu-id="b3319-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b3319-115">Property</span></span>|<span data-ttu-id="b3319-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3319-116">Type</span></span>|<span data-ttu-id="b3319-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3319-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3319-118">displayName</span><span class="sxs-lookup"><span data-stu-id="b3319-118">displayName</span></span>|<span data-ttu-id="b3319-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3319-119">String</span></span>|<span data-ttu-id="b3319-120">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="b3319-120">Friendly name of the status report.</span></span>|
|<span data-ttu-id="b3319-121">id</span><span class="sxs-lookup"><span data-stu-id="b3319-121">id</span></span>|<span data-ttu-id="b3319-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3319-122">String</span></span>|<span data-ttu-id="b3319-123">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b3319-123">Key of the entity.</span></span>|
|<span data-ttu-id="b3319-124">versão</span><span class="sxs-lookup"><span data-stu-id="b3319-124">version</span></span>|<span data-ttu-id="b3319-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3319-125">String</span></span>|<span data-ttu-id="b3319-126">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="b3319-126">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3319-127">Relações</span><span class="sxs-lookup"><span data-stu-id="b3319-127">Relationships</span></span>
<span data-ttu-id="b3319-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b3319-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b3319-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b3319-129">JSON Representation</span></span>
<span data-ttu-id="b3319-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b3319-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatus",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String"
}
```



