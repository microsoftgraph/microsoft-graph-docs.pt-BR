# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="817de-101">tipo de recurso managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="817de-101">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="817de-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="817de-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="817de-103">Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.</span><span class="sxs-lookup"><span data-stu-id="817de-103">Represents an un-typed status report about organizations app protection and configuration.</span></span>

<span data-ttu-id="817de-104">Herda de [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="817de-104">Inherits from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="817de-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="817de-105">Methods</span></span>
|<span data-ttu-id="817de-106">Método</span><span class="sxs-lookup"><span data-stu-id="817de-106">Method</span></span>|<span data-ttu-id="817de-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="817de-107">Return Type</span></span>|<span data-ttu-id="817de-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="817de-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="817de-109">Listar managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="817de-109">List managedAppStatusRaws</span></span>](../api/intune_mam_managedappstatusraw_list.md)|<span data-ttu-id="817de-110">Conjunto [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md)</span><span class="sxs-lookup"><span data-stu-id="817de-110">[managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) collection</span></span>|<span data-ttu-id="817de-111">Listar propriedades e relações de objetos de [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="817de-111">List properties and relationships of the [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="817de-112">Obter managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="817de-112">Get managedAppStatusRaw</span></span>](../api/intune_mam_managedappstatusraw_get.md)|[<span data-ttu-id="817de-113">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="817de-113">managedAppStatusRaw</span></span>](../resources/intune_mam_managedappstatusraw.md)|<span data-ttu-id="817de-114">Ler propriedades e relações do objeto [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="817de-114">Read properties and relationships of the [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="817de-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="817de-115">Properties</span></span>
|<span data-ttu-id="817de-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="817de-116">Property</span></span>|<span data-ttu-id="817de-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="817de-117">Type</span></span>|<span data-ttu-id="817de-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="817de-118">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="817de-119">displayName</span><span class="sxs-lookup"><span data-stu-id="817de-119">displayName</span></span>|<span data-ttu-id="817de-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="817de-120">String</span></span>|<span data-ttu-id="817de-121">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="817de-121">Friendly name of the status report.</span></span> <span data-ttu-id="817de-122">Herda de [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="817de-122">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="817de-123">id</span><span class="sxs-lookup"><span data-stu-id="817de-123">id</span></span>|<span data-ttu-id="817de-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="817de-124">String</span></span>|<span data-ttu-id="817de-125">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="817de-125">Key of the entity.</span></span> <span data-ttu-id="817de-126">Herda de [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="817de-126">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="817de-127">version</span><span class="sxs-lookup"><span data-stu-id="817de-127">version</span></span>|<span data-ttu-id="817de-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="817de-128">String</span></span>|<span data-ttu-id="817de-129">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="817de-129">Version of the entity.</span></span> <span data-ttu-id="817de-130">Herda de [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="817de-130">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="817de-131">content</span><span class="sxs-lookup"><span data-stu-id="817de-131">content</span></span>|[<span data-ttu-id="817de-132">Json</span><span class="sxs-lookup"><span data-stu-id="817de-132">Json</span></span>](../resources/intune_mam_json.md)|<span data-ttu-id="817de-133">Conteúdo do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="817de-133">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="817de-134">Relações</span><span class="sxs-lookup"><span data-stu-id="817de-134">Relationships</span></span>
<span data-ttu-id="817de-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="817de-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="817de-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="817de-136">JSON Representation</span></span>
<span data-ttu-id="817de-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="817de-137">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.managedAppStatus",
  "@odata.type": "microsoft.graph.managedAppStatusRaw"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```



