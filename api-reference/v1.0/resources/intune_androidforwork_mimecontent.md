# <a name="mimecontent-resource-type"></a><span data-ttu-id="3ddae-101">Tipo de recurso mimeContent</span><span class="sxs-lookup"><span data-stu-id="3ddae-101">mimeContent resource type</span></span>

> <span data-ttu-id="3ddae-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3ddae-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3ddae-103">Contém as propriedades de um conteúdo genérico MIME.</span><span class="sxs-lookup"><span data-stu-id="3ddae-103">Contains properties for a generic mime content.</span></span>
## <a name="properties"></a><span data-ttu-id="3ddae-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3ddae-104">Properties</span></span>
|<span data-ttu-id="3ddae-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3ddae-105">Property</span></span>|<span data-ttu-id="3ddae-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ddae-106">Type</span></span>|<span data-ttu-id="3ddae-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ddae-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ddae-108">type</span><span class="sxs-lookup"><span data-stu-id="3ddae-108">type</span></span>|<span data-ttu-id="3ddae-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3ddae-109">String</span></span>|<span data-ttu-id="3ddae-110">Indica o tipo de conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="3ddae-110">Indicates the content mime type.</span></span>|
|<span data-ttu-id="3ddae-111">valor</span><span class="sxs-lookup"><span data-stu-id="3ddae-111">value</span></span>|<span data-ttu-id="3ddae-112">Binário</span><span class="sxs-lookup"><span data-stu-id="3ddae-112">Binary</span></span>|<span data-ttu-id="3ddae-113">A matriz de byte que contém o conteúdo atual.</span><span class="sxs-lookup"><span data-stu-id="3ddae-113">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ddae-114">Relações</span><span class="sxs-lookup"><span data-stu-id="3ddae-114">Relationships</span></span>
<span data-ttu-id="3ddae-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3ddae-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3ddae-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3ddae-116">JSON Representation</span></span>
<span data-ttu-id="3ddae-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3ddae-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mimeContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mimeContent",
  "type": "String",
  "value": "binary"
}
```



