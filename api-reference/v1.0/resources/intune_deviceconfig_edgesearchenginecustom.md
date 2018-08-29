# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="270c7-101">Tipo de recurso edgeSearchEngineCustom</span><span class="sxs-lookup"><span data-stu-id="270c7-101">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="270c7-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="270c7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="270c7-103">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão personalizado para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="270c7-103">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="270c7-104">Herda de [edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="270c7-104">Inherits from [edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="270c7-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="270c7-105">Properties</span></span>
|<span data-ttu-id="270c7-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="270c7-106">Property</span></span>|<span data-ttu-id="270c7-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="270c7-107">Type</span></span>|<span data-ttu-id="270c7-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="270c7-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="270c7-109">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="270c7-109">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="270c7-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="270c7-110">String</span></span>|<span data-ttu-id="270c7-111">Aponta para um link https que contém o arquivo xml de OpenSearch que contém no mínimo o nome curto e a URL do mecanismo de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="270c7-111">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="270c7-112">Relações</span><span class="sxs-lookup"><span data-stu-id="270c7-112">Relationships</span></span>
<span data-ttu-id="270c7-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="270c7-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="270c7-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="270c7-114">JSON Representation</span></span>
<span data-ttu-id="270c7-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="270c7-115">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.edgeSearchEngineBase",
  "@odata.type": "microsoft.graph.edgeSearchEngineCustom"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngineCustom",
  "edgeSearchEngineOpenSearchXmlUrl": "String"
}
```



