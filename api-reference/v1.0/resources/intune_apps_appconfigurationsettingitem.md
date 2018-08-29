# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="92aa2-101">Tipo de recurso appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="92aa2-101">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="92aa2-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="92aa2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="92aa2-103">Contém propriedades do item de configuração de Configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="92aa2-103">Contains properties for App configuration setting item.</span></span>
## <a name="properties"></a><span data-ttu-id="92aa2-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="92aa2-104">Properties</span></span>
|<span data-ttu-id="92aa2-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92aa2-105">Property</span></span>|<span data-ttu-id="92aa2-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="92aa2-106">Type</span></span>|<span data-ttu-id="92aa2-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="92aa2-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92aa2-108">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="92aa2-108">appConfigKey</span></span>|<span data-ttu-id="92aa2-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92aa2-109">String</span></span>|<span data-ttu-id="92aa2-110">chave de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="92aa2-110">app configuration key.</span></span>|
|<span data-ttu-id="92aa2-111">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="92aa2-111">appConfigKeyType</span></span>|<span data-ttu-id="92aa2-112">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="92aa2-112">mdmAppConfigKeyType</span></span>|<span data-ttu-id="92aa2-113">tipo de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="92aa2-113">app configuration key type.</span></span> <span data-ttu-id="92aa2-114">Os valores possíveis são: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="92aa2-114">The possible values are `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`, , , , , , , or .</span></span>|
|<span data-ttu-id="92aa2-115">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="92aa2-115">appConfigKeyValue</span></span>|<span data-ttu-id="92aa2-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92aa2-116">String</span></span>|<span data-ttu-id="92aa2-117">valor de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="92aa2-117">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="92aa2-118">Relações</span><span class="sxs-lookup"><span data-stu-id="92aa2-118">Relationships</span></span>
<span data-ttu-id="92aa2-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="92aa2-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="92aa2-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="92aa2-120">JSON Representation</span></span>
<span data-ttu-id="92aa2-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="92aa2-121">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appConfigurationSettingItem"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.appConfigurationSettingItem",
  "appConfigKey": "String",
  "appConfigKeyType": "String",
  "appConfigKeyValue": "String"
}
```



