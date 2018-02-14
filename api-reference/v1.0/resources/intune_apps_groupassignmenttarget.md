# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="7bd2d-101">Tipo de recurso groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7bd2d-101">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="7bd2d-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7bd2d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7bd2d-103">Representa uma atribuição para um grupo.</span><span class="sxs-lookup"><span data-stu-id="7bd2d-103">Represents an assignment to a group.</span></span>

<span data-ttu-id="7bd2d-104">Herda de [deviceAndAppManagementAssignmentTarget](../resources/intune_apps_deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="7bd2d-104">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune_apps_deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7bd2d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7bd2d-105">Properties</span></span>
|<span data-ttu-id="7bd2d-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7bd2d-106">Property</span></span>|<span data-ttu-id="7bd2d-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="7bd2d-107">Type</span></span>|<span data-ttu-id="7bd2d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bd2d-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bd2d-109">groupId</span><span class="sxs-lookup"><span data-stu-id="7bd2d-109">groupId</span></span>|<span data-ttu-id="7bd2d-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7bd2d-110">String</span></span>|<span data-ttu-id="7bd2d-111">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="7bd2d-111">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7bd2d-112">Relações</span><span class="sxs-lookup"><span data-stu-id="7bd2d-112">Relationships</span></span>
<span data-ttu-id="7bd2d-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7bd2d-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7bd2d-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7bd2d-114">JSON Representation</span></span>
<span data-ttu-id="7bd2d-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7bd2d-115">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupAssignmentTarget",
  "groupId": "String"
}
```



