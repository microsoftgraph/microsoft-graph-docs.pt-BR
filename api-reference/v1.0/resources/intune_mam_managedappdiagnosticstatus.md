# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="47303-101">Tipo de recurso managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="47303-101">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="47303-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="47303-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47303-103">Representa o status de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="47303-103">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="47303-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="47303-104">Properties</span></span>
|<span data-ttu-id="47303-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="47303-105">Property</span></span>|<span data-ttu-id="47303-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="47303-106">Type</span></span>|<span data-ttu-id="47303-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="47303-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47303-108">validationName</span><span class="sxs-lookup"><span data-stu-id="47303-108">validationName</span></span>|<span data-ttu-id="47303-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="47303-109">String</span></span>|<span data-ttu-id="47303-110">O nome amigável da validação</span><span class="sxs-lookup"><span data-stu-id="47303-110">The validation friendly name</span></span>|
|<span data-ttu-id="47303-111">estado</span><span class="sxs-lookup"><span data-stu-id="47303-111">state</span></span>|<span data-ttu-id="47303-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="47303-112">String</span></span>|<span data-ttu-id="47303-113">O estado da operação</span><span class="sxs-lookup"><span data-stu-id="47303-113">The state of the operation</span></span>|
|<span data-ttu-id="47303-114">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="47303-114">mitigationInstruction</span></span>|<span data-ttu-id="47303-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="47303-115">String</span></span>|<span data-ttu-id="47303-116">Instruções sobre como atenuar uma falha de validação</span><span class="sxs-lookup"><span data-stu-id="47303-116">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="47303-117">Relações</span><span class="sxs-lookup"><span data-stu-id="47303-117">Relationships</span></span>
<span data-ttu-id="47303-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="47303-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="47303-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="47303-119">JSON Representation</span></span>
<span data-ttu-id="47303-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="47303-120">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedAppDiagnosticStatus"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppDiagnosticStatus",
  "validationName": "String",
  "state": "String",
  "mitigationInstruction": "String"
}
```



