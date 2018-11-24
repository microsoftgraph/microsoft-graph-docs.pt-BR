# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="204ae-101">tipo de recurso managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="204ae-101">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="204ae-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="204ae-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="204ae-103">Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.</span><span class="sxs-lookup"><span data-stu-id="204ae-103">Represents an un-typed status report about organizations app protection and configuration.</span></span>

<span data-ttu-id="204ae-104">Herda de [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="204ae-104">Inherits from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="204ae-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="204ae-105">Methods</span></span>
|<span data-ttu-id="204ae-106">Método</span><span class="sxs-lookup"><span data-stu-id="204ae-106">Method</span></span>|<span data-ttu-id="204ae-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="204ae-107">Return Type</span></span>|<span data-ttu-id="204ae-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="204ae-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="204ae-109">Listar managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="204ae-109">List managedAppStatusRaws</span></span>](../api/intune_mam_managedappstatusraw_list.md)|<span data-ttu-id="204ae-110">Conjunto [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md)</span><span class="sxs-lookup"><span data-stu-id="204ae-110">[managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) collection</span></span>|<span data-ttu-id="204ae-111">Listar propriedades e relações de objetos de [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="204ae-111">List properties and relationships of the [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="204ae-112">Obter managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="204ae-112">Get managedAppStatusRaw</span></span>](../api/intune_mam_managedappstatusraw_get.md)|[<span data-ttu-id="204ae-113">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="204ae-113">managedAppStatusRaw</span></span>](../resources/intune_mam_managedappstatusraw.md)|<span data-ttu-id="204ae-114">Ler propriedades e relações do objeto [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="204ae-114">Read properties and relationships of the [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="204ae-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="204ae-115">Properties</span></span>
|<span data-ttu-id="204ae-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="204ae-116">Property</span></span>|<span data-ttu-id="204ae-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="204ae-117">Type</span></span>|<span data-ttu-id="204ae-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="204ae-118">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="204ae-119">displayName</span><span class="sxs-lookup"><span data-stu-id="204ae-119">displayName</span></span>|<span data-ttu-id="204ae-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="204ae-120">String</span></span>|<span data-ttu-id="204ae-121">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="204ae-121">Friendly name of the status report.</span></span> <span data-ttu-id="204ae-122">Herda de [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="204ae-122">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="204ae-123">id</span><span class="sxs-lookup"><span data-stu-id="204ae-123">id</span></span>|<span data-ttu-id="204ae-124">String</span><span class="sxs-lookup"><span data-stu-id="204ae-124">String</span></span>|<span data-ttu-id="204ae-125">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="204ae-125">Key of the entity.</span></span> <span data-ttu-id="204ae-126">Herda de [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="204ae-126">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="204ae-127">version</span><span class="sxs-lookup"><span data-stu-id="204ae-127">version</span></span>|<span data-ttu-id="204ae-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="204ae-128">String</span></span>|<span data-ttu-id="204ae-129">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="204ae-129">Version of the entity.</span></span> <span data-ttu-id="204ae-130">Herda de [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="204ae-130">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="204ae-131">content</span><span class="sxs-lookup"><span data-stu-id="204ae-131">content</span></span>|[<span data-ttu-id="204ae-132">Json</span><span class="sxs-lookup"><span data-stu-id="204ae-132">Json</span></span>](../resources/intune_mam_json.md)|<span data-ttu-id="204ae-133">Conteúdo do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="204ae-133">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="204ae-134">Relações</span><span class="sxs-lookup"><span data-stu-id="204ae-134">Relationships</span></span>
<span data-ttu-id="204ae-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="204ae-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="204ae-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="204ae-136">JSON Representation</span></span>
<span data-ttu-id="204ae-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="204ae-137">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatusRaw"
}
-->
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



