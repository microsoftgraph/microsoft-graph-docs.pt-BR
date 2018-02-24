# <a name="androidforworkappconfigurationschemaitem-resource-type"></a><span data-ttu-id="4d1d4-101">Tipo de recurso androidForWorkAppConfigurationSchemaItem</span><span class="sxs-lookup"><span data-stu-id="4d1d4-101">androidForWorkAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="4d1d4-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4d1d4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4d1d4-103">Item de configuração único dentro de um esquema de configurações personalizadas de um aplicativo do Android for Work.</span><span class="sxs-lookup"><span data-stu-id="4d1d4-103">Single configuration item inside an Android for Work application's custom configuration schema.</span></span>
## <a name="properties"></a><span data-ttu-id="4d1d4-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4d1d4-104">Properties</span></span>
|<span data-ttu-id="4d1d4-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4d1d4-105">Property</span></span>|<span data-ttu-id="4d1d4-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d1d4-106">Type</span></span>|<span data-ttu-id="4d1d4-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d1d4-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d1d4-108">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="4d1d4-108">schemaItemKey</span></span>|<span data-ttu-id="4d1d4-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d1d4-109">String</span></span>|<span data-ttu-id="4d1d4-110">Chave exclusiva que o aplicativo usa para identificar o item</span><span class="sxs-lookup"><span data-stu-id="4d1d4-110">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="4d1d4-111">displayName</span><span class="sxs-lookup"><span data-stu-id="4d1d4-111">displayName</span></span>|<span data-ttu-id="4d1d4-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d1d4-112">String</span></span>|<span data-ttu-id="4d1d4-113">Nome legível por humanos</span><span class="sxs-lookup"><span data-stu-id="4d1d4-113">Human readable name</span></span>|
|<span data-ttu-id="4d1d4-114">description</span><span class="sxs-lookup"><span data-stu-id="4d1d4-114">description</span></span>|<span data-ttu-id="4d1d4-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d1d4-115">String</span></span>|<span data-ttu-id="4d1d4-116">Descrição do que o item controla dentro do aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d1d4-116">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="4d1d4-117">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="4d1d4-117">defaultBoolValue</span></span>|<span data-ttu-id="4d1d4-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="4d1d4-118">Boolean</span></span>|<span data-ttu-id="4d1d4-119">Valor padrão para itens do tipo booliano, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d1d4-119">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="4d1d4-120">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="4d1d4-120">defaultIntValue</span></span>|<span data-ttu-id="4d1d4-121">Int32</span><span class="sxs-lookup"><span data-stu-id="4d1d4-121">Int32</span></span>|<span data-ttu-id="4d1d4-122">Valor padrão para itens do tipo inteiro, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d1d4-122">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="4d1d4-123">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="4d1d4-123">defaultStringValue</span></span>|<span data-ttu-id="4d1d4-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d1d4-124">String</span></span>|<span data-ttu-id="4d1d4-125">Valor padrão para itens do tipo cadeia de caracteres, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d1d4-125">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="4d1d4-126">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="4d1d4-126">defaultStringArrayValue</span></span>|<span data-ttu-id="4d1d4-127">Coleção String</span><span class="sxs-lookup"><span data-stu-id="4d1d4-127">String collection</span></span>|<span data-ttu-id="4d1d4-128">Valor padrão para itens do tipo matriz, se especificado pelo desenvolvedor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d1d4-128">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="4d1d4-129">dataType</span><span class="sxs-lookup"><span data-stu-id="4d1d4-129">datatype</span></span>|<span data-ttu-id="4d1d4-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d1d4-130">String</span></span>|<span data-ttu-id="4d1d4-131">O tipo de valor que esse item descreve Os valores possíveis são: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span><span class="sxs-lookup"><span data-stu-id="4d1d4-131">The type of value this item describes Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="4d1d4-132">selections</span><span class="sxs-lookup"><span data-stu-id="4d1d4-132">selections</span></span>|<span data-ttu-id="4d1d4-133">Coleção [keyValuePair](../resources/intune_androidforwork_keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="4d1d4-133">[keyValuePair](../resources/intune_androidforwork_keyvaluepair.md) collection</span></span>|<span data-ttu-id="4d1d4-134">Lista de pares nome/valor legíveis por humanos dos valores válidos que podem ser definidos para esse item (somente itens de Escolha e Múltipla escolha)</span><span class="sxs-lookup"><span data-stu-id="4d1d4-134">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d1d4-135">Relações</span><span class="sxs-lookup"><span data-stu-id="4d1d4-135">Relationships</span></span>
<span data-ttu-id="4d1d4-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4d1d4-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4d1d4-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4d1d4-137">JSON Representation</span></span>
<span data-ttu-id="4d1d4-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4d1d4-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchemaItem",
  "schemaItemKey": "String",
  "displayName": "String",
  "description": "String",
  "defaultBoolValue": true,
  "defaultIntValue": 1024,
  "defaultStringValue": "String",
  "defaultStringArrayValue": [
    "String"
  ],
  "dataType": "String",
  "selections": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```



