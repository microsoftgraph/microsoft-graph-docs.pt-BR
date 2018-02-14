# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="e3c18-101">Tipo de recurso exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e3c18-101">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="e3c18-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e3c18-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3c18-103">Representa um grupo que deve ser excluído de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="e3c18-103">Represents a group that should be excluded from an assignment.</span></span>

<span data-ttu-id="e3c18-104">Herda de [groupAssignmentTarget](../resources/intune_onboarding_groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="e3c18-104">Inherits from [groupAssignmentTarget](../resources/intune_onboarding_groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e3c18-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e3c18-105">Properties</span></span>
|<span data-ttu-id="e3c18-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3c18-106">Property</span></span>|<span data-ttu-id="e3c18-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3c18-107">Type</span></span>|<span data-ttu-id="e3c18-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3c18-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3c18-109">groupId</span><span class="sxs-lookup"><span data-stu-id="e3c18-109">groupId</span></span>|<span data-ttu-id="e3c18-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3c18-110">String</span></span>|<span data-ttu-id="e3c18-111">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="e3c18-111">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="e3c18-112">Herda de [groupAssignmentTarget](../resources/intune_onboarding_groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="e3c18-112">Inherited from [groupAssignmentTarget](../resources/intune_onboarding_groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3c18-113">Relações</span><span class="sxs-lookup"><span data-stu-id="e3c18-113">Relationships</span></span>
<span data-ttu-id="e3c18-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e3c18-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e3c18-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e3c18-115">JSON Representation</span></span>
<span data-ttu-id="e3c18-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e3c18-116">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.exclusionGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exclusionGroupAssignmentTarget",
  "groupId": "String"
}
```



