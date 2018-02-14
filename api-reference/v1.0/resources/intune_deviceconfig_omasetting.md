# <a name="omasetting-resource-type"></a><span data-ttu-id="808c3-101">Tipo de recurso omaSetting</span><span class="sxs-lookup"><span data-stu-id="808c3-101">omaSetting resource type</span></span>

> <span data-ttu-id="808c3-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="808c3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="808c3-103">Configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="808c3-103">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="808c3-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="808c3-104">Properties</span></span>
|<span data-ttu-id="808c3-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="808c3-105">Property</span></span>|<span data-ttu-id="808c3-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="808c3-106">Type</span></span>|<span data-ttu-id="808c3-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="808c3-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="808c3-108">displayName</span><span class="sxs-lookup"><span data-stu-id="808c3-108">displayName</span></span>|<span data-ttu-id="808c3-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="808c3-109">String</span></span>|<span data-ttu-id="808c3-110">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="808c3-110">Display Name</span></span>|
|<span data-ttu-id="808c3-111">descrição</span><span class="sxs-lookup"><span data-stu-id="808c3-111">description</span></span>|<span data-ttu-id="808c3-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="808c3-112">String</span></span>|<span data-ttu-id="808c3-113">Descrição.</span><span class="sxs-lookup"><span data-stu-id="808c3-113">Description.</span></span>|
|<span data-ttu-id="808c3-114">omaUri</span><span class="sxs-lookup"><span data-stu-id="808c3-114">omaUri</span></span>|<span data-ttu-id="808c3-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="808c3-115">String</span></span>|<span data-ttu-id="808c3-116">OMA.</span><span class="sxs-lookup"><span data-stu-id="808c3-116">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="808c3-117">Relações</span><span class="sxs-lookup"><span data-stu-id="808c3-117">Relationships</span></span>
<span data-ttu-id="808c3-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="808c3-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="808c3-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="808c3-119">JSON Representation</span></span>
<span data-ttu-id="808c3-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="808c3-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```



