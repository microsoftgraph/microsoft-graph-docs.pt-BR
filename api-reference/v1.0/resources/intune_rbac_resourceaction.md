# <a name="resourceaction-resource-type"></a><span data-ttu-id="48a41-101">Tipo de recurso resourceAction</span><span class="sxs-lookup"><span data-stu-id="48a41-101">resourceAction resource type</span></span>

> <span data-ttu-id="48a41-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="48a41-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="48a41-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="48a41-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="48a41-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="48a41-104">Properties</span></span>
|<span data-ttu-id="48a41-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48a41-105">Property</span></span>|<span data-ttu-id="48a41-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="48a41-106">Type</span></span>|<span data-ttu-id="48a41-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="48a41-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48a41-108">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="48a41-108">allowedResourceActions</span></span>|<span data-ttu-id="48a41-109">String collection</span><span class="sxs-lookup"><span data-stu-id="48a41-109">String collection</span></span>|<span data-ttu-id="48a41-110">Ações permitidas</span><span class="sxs-lookup"><span data-stu-id="48a41-110">Allowed Actions</span></span>|
|<span data-ttu-id="48a41-111">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="48a41-111">notAllowedResourceActions</span></span>|<span data-ttu-id="48a41-112">String collection</span><span class="sxs-lookup"><span data-stu-id="48a41-112">String collection</span></span>|<span data-ttu-id="48a41-113">Ações não permitidas</span><span class="sxs-lookup"><span data-stu-id="48a41-113">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="48a41-114">Relações</span><span class="sxs-lookup"><span data-stu-id="48a41-114">Relationships</span></span>
<span data-ttu-id="48a41-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="48a41-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="48a41-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="48a41-116">JSON Representation</span></span>
<span data-ttu-id="48a41-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="48a41-117">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}-->
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








