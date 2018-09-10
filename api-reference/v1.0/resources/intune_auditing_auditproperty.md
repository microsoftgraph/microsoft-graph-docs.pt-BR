# <a name="auditproperty-resource-type"></a><span data-ttu-id="4b173-101">Tipo de recurso auditProperty</span><span class="sxs-lookup"><span data-stu-id="4b173-101">auditProperty resource type</span></span>

> <span data-ttu-id="4b173-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4b173-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b173-103">Uma classe que contém as propriedades para a Propriedade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="4b173-103">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="4b173-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4b173-104">Properties</span></span>
|<span data-ttu-id="4b173-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b173-105">Property</span></span>|<span data-ttu-id="4b173-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b173-106">Type</span></span>|<span data-ttu-id="4b173-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b173-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b173-108">displayName</span><span class="sxs-lookup"><span data-stu-id="4b173-108">displayName</span></span>|<span data-ttu-id="4b173-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b173-109">String</span></span>|<span data-ttu-id="4b173-110">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="4b173-110">Display name.</span></span>|
|<span data-ttu-id="4b173-111">oldValue</span><span class="sxs-lookup"><span data-stu-id="4b173-111">oldValue</span></span>|<span data-ttu-id="4b173-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b173-112">String</span></span>|<span data-ttu-id="4b173-113">Valor antigo.</span><span class="sxs-lookup"><span data-stu-id="4b173-113">Old value.</span></span>|
|<span data-ttu-id="4b173-114">newValue</span><span class="sxs-lookup"><span data-stu-id="4b173-114">newValue</span></span>|<span data-ttu-id="4b173-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b173-115">String</span></span>|<span data-ttu-id="4b173-116">Novo valor.</span><span class="sxs-lookup"><span data-stu-id="4b173-116">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b173-117">Relações</span><span class="sxs-lookup"><span data-stu-id="4b173-117">Relationships</span></span>
<span data-ttu-id="4b173-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4b173-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4b173-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4b173-119">JSON Representation</span></span>
<span data-ttu-id="4b173-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4b173-120">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditProperty"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.auditProperty",
  "displayName": "String",
  "oldValue": "String",
  "newValue": "String"
}
```








