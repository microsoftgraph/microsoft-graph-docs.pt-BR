# <a name="managedappstatus-resource-type"></a><span data-ttu-id="44de6-101">Tipo de recurso managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="44de6-101">managedAppStatus resource type</span></span>

> <span data-ttu-id="44de6-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="44de6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="44de6-103">Representa o status de proteção e configuração do aplicativo para a organização.</span><span class="sxs-lookup"><span data-stu-id="44de6-103">Represents app protection and configuration status for the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="44de6-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="44de6-104">Methods</span></span>
|<span data-ttu-id="44de6-105">Método</span><span class="sxs-lookup"><span data-stu-id="44de6-105">Method</span></span>|<span data-ttu-id="44de6-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="44de6-106">Return Type</span></span>|<span data-ttu-id="44de6-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="44de6-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="44de6-108">Listar managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="44de6-108">List managedAppStatuses</span></span>](../api/intune_mam_managedappstatus_list.md)|<span data-ttu-id="44de6-109">Conjunto [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="44de6-109">[managedAppStatus](../resources/intune_mam_managedappstatus.md) collection</span></span>|<span data-ttu-id="44de6-110">Listar propriedades e as relações de objetos de [managedAppStatus](../resources/intune_mam_managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="44de6-110">List properties and relationships of the [managedAppStatus](../resources/intune_mam_managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="44de6-111">Obter managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="44de6-111">Get managedAppStatus</span></span>](../api/intune_mam_managedappstatus_get.md)|[<span data-ttu-id="44de6-112">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="44de6-112">managedAppStatus</span></span>](../resources/intune_mam_managedappstatus.md)|<span data-ttu-id="44de6-113">Ler propriedades e relações de objetos de [managedAppStatus](../resources/intune_mam_managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="44de6-113">Read properties and relationships of the [managedAppStatus](../resources/intune_mam_managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="44de6-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="44de6-114">Properties</span></span>
|<span data-ttu-id="44de6-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44de6-115">Property</span></span>|<span data-ttu-id="44de6-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="44de6-116">Type</span></span>|<span data-ttu-id="44de6-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="44de6-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44de6-118">displayName</span><span class="sxs-lookup"><span data-stu-id="44de6-118">displayName</span></span>|<span data-ttu-id="44de6-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44de6-119">String</span></span>|<span data-ttu-id="44de6-120">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="44de6-120">Friendly name of the status report.</span></span>|
|<span data-ttu-id="44de6-121">id</span><span class="sxs-lookup"><span data-stu-id="44de6-121">id</span></span>|<span data-ttu-id="44de6-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44de6-122">String</span></span>|<span data-ttu-id="44de6-123">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="44de6-123">Key of the entity.</span></span>|
|<span data-ttu-id="44de6-124">version</span><span class="sxs-lookup"><span data-stu-id="44de6-124">version</span></span>|<span data-ttu-id="44de6-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44de6-125">String</span></span>|<span data-ttu-id="44de6-126">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="44de6-126">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="44de6-127">Relações</span><span class="sxs-lookup"><span data-stu-id="44de6-127">Relationships</span></span>
<span data-ttu-id="44de6-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="44de6-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="44de6-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="44de6-129">JSON Representation</span></span>
<span data-ttu-id="44de6-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="44de6-130">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "abstract": true,
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.managedAppStatus"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatus",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String"
}
```



