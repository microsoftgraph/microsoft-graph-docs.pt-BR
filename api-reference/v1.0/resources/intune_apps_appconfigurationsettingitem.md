# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="a8f08-101">Tipo de recurso appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="a8f08-101">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="a8f08-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a8f08-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8f08-103">Contém propriedades do item de configuração de Configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a8f08-103">Contains properties for App configuration setting item.</span></span>
## <a name="properties"></a><span data-ttu-id="a8f08-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a8f08-104">Properties</span></span>
|<span data-ttu-id="a8f08-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8f08-105">Property</span></span>|<span data-ttu-id="a8f08-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8f08-106">Type</span></span>|<span data-ttu-id="a8f08-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8f08-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8f08-108">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="a8f08-108">appConfigKey</span></span>|<span data-ttu-id="a8f08-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8f08-109">String</span></span>|<span data-ttu-id="a8f08-110">chave de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a8f08-110">app configuration key.</span></span>|
|<span data-ttu-id="a8f08-111">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="a8f08-111">appConfigKeyType</span></span>|<span data-ttu-id="a8f08-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8f08-112">String</span></span>|<span data-ttu-id="a8f08-113">tipo de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a8f08-113">app configuration key type.</span></span> <span data-ttu-id="a8f08-114">Os valores possíveis são: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="a8f08-114">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="a8f08-115">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="a8f08-115">appConfigKeyValue</span></span>|<span data-ttu-id="a8f08-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8f08-116">String</span></span>|<span data-ttu-id="a8f08-117">valor de chave de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a8f08-117">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8f08-118">Relações</span><span class="sxs-lookup"><span data-stu-id="a8f08-118">Relationships</span></span>
<span data-ttu-id="a8f08-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a8f08-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a8f08-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a8f08-120">JSON Representation</span></span>
<span data-ttu-id="a8f08-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a8f08-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appConfigurationSettingItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appConfigurationSettingItem",
  "appConfigKey": "String",
  "appConfigKeyType": "String",
  "appConfigKeyValue": "String"
}
```



