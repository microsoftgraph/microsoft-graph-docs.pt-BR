# <a name="resourceaction-resource-type"></a><span data-ttu-id="1ea63-101">Tipo de recurso resourceAction</span><span class="sxs-lookup"><span data-stu-id="1ea63-101">resourceAction resource type</span></span>

> <span data-ttu-id="1ea63-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1ea63-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ea63-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1ea63-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="1ea63-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1ea63-104">Properties</span></span>
|<span data-ttu-id="1ea63-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ea63-105">Property</span></span>|<span data-ttu-id="1ea63-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ea63-106">Type</span></span>|<span data-ttu-id="1ea63-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ea63-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ea63-108">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="1ea63-108">allowedResourceActions</span></span>|<span data-ttu-id="1ea63-109">String collection</span><span class="sxs-lookup"><span data-stu-id="1ea63-109">String collection</span></span>|<span data-ttu-id="1ea63-110">Ações permitidas</span><span class="sxs-lookup"><span data-stu-id="1ea63-110">Allowed Actions</span></span>|
|<span data-ttu-id="1ea63-111">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="1ea63-111">notAllowedResourceActions</span></span>|<span data-ttu-id="1ea63-112">String collection</span><span class="sxs-lookup"><span data-stu-id="1ea63-112">String collection</span></span>|<span data-ttu-id="1ea63-113">Ações não permitidas</span><span class="sxs-lookup"><span data-stu-id="1ea63-113">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ea63-114">Relações</span><span class="sxs-lookup"><span data-stu-id="1ea63-114">Relationships</span></span>
<span data-ttu-id="1ea63-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1ea63-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1ea63-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1ea63-116">JSON Representation</span></span>
<span data-ttu-id="1ea63-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1ea63-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```



