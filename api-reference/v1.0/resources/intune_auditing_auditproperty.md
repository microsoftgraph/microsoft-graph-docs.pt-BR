# <a name="auditproperty-resource-type"></a><span data-ttu-id="fd4d6-101">Tipo de recurso auditProperty</span><span class="sxs-lookup"><span data-stu-id="fd4d6-101">auditProperty resource type</span></span>

> <span data-ttu-id="fd4d6-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fd4d6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd4d6-103">Uma classe que contém as propriedades para a Propriedade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="fd4d6-103">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="fd4d6-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fd4d6-104">Properties</span></span>
|<span data-ttu-id="fd4d6-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd4d6-105">Property</span></span>|<span data-ttu-id="fd4d6-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd4d6-106">Type</span></span>|<span data-ttu-id="fd4d6-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd4d6-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd4d6-108">displayName</span><span class="sxs-lookup"><span data-stu-id="fd4d6-108">displayName</span></span>|<span data-ttu-id="fd4d6-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd4d6-109">String</span></span>|<span data-ttu-id="fd4d6-110">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="fd4d6-110">Display name.</span></span>|
|<span data-ttu-id="fd4d6-111">oldValue</span><span class="sxs-lookup"><span data-stu-id="fd4d6-111">oldValue</span></span>|<span data-ttu-id="fd4d6-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd4d6-112">String</span></span>|<span data-ttu-id="fd4d6-113">Valor antigo.</span><span class="sxs-lookup"><span data-stu-id="fd4d6-113">Old value.</span></span>|
|<span data-ttu-id="fd4d6-114">newValue</span><span class="sxs-lookup"><span data-stu-id="fd4d6-114">newValue</span></span>|<span data-ttu-id="fd4d6-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd4d6-115">String</span></span>|<span data-ttu-id="fd4d6-116">Novo valor.</span><span class="sxs-lookup"><span data-stu-id="fd4d6-116">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd4d6-117">Relações</span><span class="sxs-lookup"><span data-stu-id="fd4d6-117">Relationships</span></span>
<span data-ttu-id="fd4d6-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fd4d6-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fd4d6-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fd4d6-119">JSON Representation</span></span>
<span data-ttu-id="fd4d6-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fd4d6-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditProperty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditProperty",
  "displayName": "String",
  "oldValue": "String",
  "newValue": "String"
}
```



