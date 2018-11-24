# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="c8636-101">Tipo de recurso groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c8636-101">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="c8636-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c8636-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8636-103">Representa uma atribuição para um grupo.</span><span class="sxs-lookup"><span data-stu-id="c8636-103">Represents an assignment to a group.</span></span>

<span data-ttu-id="c8636-104">Herda de [deviceAndAppManagementAssignmentTarget](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="c8636-104">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c8636-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c8636-105">Properties</span></span>
|<span data-ttu-id="c8636-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c8636-106">Property</span></span>|<span data-ttu-id="c8636-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8636-107">Type</span></span>|<span data-ttu-id="c8636-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8636-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8636-109">groupId</span><span class="sxs-lookup"><span data-stu-id="c8636-109">groupId</span></span>|<span data-ttu-id="c8636-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8636-110">String</span></span>|<span data-ttu-id="c8636-111">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="c8636-111">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8636-112">Relações</span><span class="sxs-lookup"><span data-stu-id="c8636-112">Relationships</span></span>
<span data-ttu-id="c8636-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c8636-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c8636-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c8636-114">JSON Representation</span></span>
<span data-ttu-id="c8636-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c8636-115">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupAssignmentTarget",
  "groupId": "String"
}
```



