# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="6ee75-101">Tipo de recurso keyValuePair</span><span class="sxs-lookup"><span data-stu-id="6ee75-101">keyValuePair resource type</span></span>

> <span data-ttu-id="6ee75-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6ee75-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6ee75-103">Par chave-valor para armazenar configurações personalizadas</span><span class="sxs-lookup"><span data-stu-id="6ee75-103">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="6ee75-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6ee75-104">Properties</span></span>
|<span data-ttu-id="6ee75-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6ee75-105">Property</span></span>|<span data-ttu-id="6ee75-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ee75-106">Type</span></span>|<span data-ttu-id="6ee75-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ee75-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ee75-108">nome</span><span class="sxs-lookup"><span data-stu-id="6ee75-108">name</span></span>|<span data-ttu-id="6ee75-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6ee75-109">String</span></span>|<span data-ttu-id="6ee75-110">Nome deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="6ee75-110">Name for this key-value pair</span></span>|
|<span data-ttu-id="6ee75-111">valor</span><span class="sxs-lookup"><span data-stu-id="6ee75-111">value</span></span>|<span data-ttu-id="6ee75-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6ee75-112">String</span></span>|<span data-ttu-id="6ee75-113">Valor deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="6ee75-113">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ee75-114">Relações</span><span class="sxs-lookup"><span data-stu-id="6ee75-114">Relationships</span></span>
<span data-ttu-id="6ee75-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6ee75-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6ee75-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6ee75-116">JSON Representation</span></span>
<span data-ttu-id="6ee75-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6ee75-117">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValuePair"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValuePair",
  "name": "String",
  "value": "String"
}
```








