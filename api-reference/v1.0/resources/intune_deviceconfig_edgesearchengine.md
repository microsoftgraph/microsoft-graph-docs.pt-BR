# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="5caf5-101">Tipo de recurso edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="5caf5-101">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="5caf5-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5caf5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5caf5-103">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="5caf5-103">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="5caf5-104">Herda de [edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="5caf5-104">Inherits from [edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5caf5-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5caf5-105">Properties</span></span>
|<span data-ttu-id="5caf5-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5caf5-106">Property</span></span>|<span data-ttu-id="5caf5-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="5caf5-107">Type</span></span>|<span data-ttu-id="5caf5-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="5caf5-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5caf5-109">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="5caf5-109">edgeSearchEngineType</span></span>|[<span data-ttu-id="5caf5-110">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="5caf5-110">edgeSearchEngineType</span></span>](../resources/intune_deviceconfig_edgesearchenginetype.md)|<span data-ttu-id="5caf5-111">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="5caf5-111">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="5caf5-112">Os valores possíveis são: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="5caf5-112">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5caf5-113">Relações</span><span class="sxs-lookup"><span data-stu-id="5caf5-113">Relationships</span></span>
<span data-ttu-id="5caf5-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5caf5-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5caf5-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5caf5-115">JSON Representation</span></span>
<span data-ttu-id="5caf5-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5caf5-116">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngine"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngine",
  "edgeSearchEngineType": "String"
}
```



