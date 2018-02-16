# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="e87cb-101">Tipo de recurso iosHomeScreenItem</span><span class="sxs-lookup"><span data-stu-id="e87cb-101">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="e87cb-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e87cb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e87cb-103">Representa um item na tela inicial do iOS</span><span class="sxs-lookup"><span data-stu-id="e87cb-103">Represents an item on the iOS Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="e87cb-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e87cb-104">Properties</span></span>
|<span data-ttu-id="e87cb-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e87cb-105">Property</span></span>|<span data-ttu-id="e87cb-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="e87cb-106">Type</span></span>|<span data-ttu-id="e87cb-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="e87cb-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e87cb-108">displayName</span><span class="sxs-lookup"><span data-stu-id="e87cb-108">displayName</span></span>|<span data-ttu-id="e87cb-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e87cb-109">String</span></span>|<span data-ttu-id="e87cb-110">Nome do aplicativo</span><span class="sxs-lookup"><span data-stu-id="e87cb-110">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="e87cb-111">Relações</span><span class="sxs-lookup"><span data-stu-id="e87cb-111">Relationships</span></span>
<span data-ttu-id="e87cb-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e87cb-112">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e87cb-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e87cb-113">JSON Representation</span></span>
<span data-ttu-id="e87cb-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e87cb-114">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosHomeScreenItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenItem",
  "displayName": "String"
}
```



