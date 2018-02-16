# <a name="auditresource-resource-type"></a><span data-ttu-id="d46e9-101">Tipo de recurso auditResource</span><span class="sxs-lookup"><span data-stu-id="d46e9-101">auditResource resource type</span></span>

> <span data-ttu-id="d46e9-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d46e9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d46e9-103">Uma classe que contém as propriedades para o Recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="d46e9-103">A class containing the properties for Audit Resource.</span></span>
## <a name="properties"></a><span data-ttu-id="d46e9-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d46e9-104">Properties</span></span>
|<span data-ttu-id="d46e9-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d46e9-105">Property</span></span>|<span data-ttu-id="d46e9-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="d46e9-106">Type</span></span>|<span data-ttu-id="d46e9-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="d46e9-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d46e9-108">displayName</span><span class="sxs-lookup"><span data-stu-id="d46e9-108">displayName</span></span>|<span data-ttu-id="d46e9-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d46e9-109">String</span></span>|<span data-ttu-id="d46e9-110">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="d46e9-110">Display Name</span></span>|
|<span data-ttu-id="d46e9-111">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="d46e9-111">modifiedProperties</span></span>|<span data-ttu-id="d46e9-112">Conjunto [auditProperty](../resources/intune_auditing_auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="d46e9-112">[auditProperty](../resources/intune_auditing_auditproperty.md) collection</span></span>|<span data-ttu-id="d46e9-113">Lista de propriedades modificadas.</span><span class="sxs-lookup"><span data-stu-id="d46e9-113">List of modified properties.</span></span>|
|<span data-ttu-id="d46e9-114">tipo</span><span class="sxs-lookup"><span data-stu-id="d46e9-114">type</span></span>|<span data-ttu-id="d46e9-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d46e9-115">String</span></span>|<span data-ttu-id="d46e9-116">Tipo de recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="d46e9-116">Audit resource's type.</span></span>|
|<span data-ttu-id="d46e9-117">resourceId</span><span class="sxs-lookup"><span data-stu-id="d46e9-117">resourceId</span></span>|<span data-ttu-id="d46e9-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d46e9-118">String</span></span>|<span data-ttu-id="d46e9-119">ID do recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="d46e9-119">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d46e9-120">Relações</span><span class="sxs-lookup"><span data-stu-id="d46e9-120">Relationships</span></span>
<span data-ttu-id="d46e9-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d46e9-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d46e9-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d46e9-122">JSON Representation</span></span>
<span data-ttu-id="d46e9-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d46e9-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.auditResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditResource",
  "displayName": "String",
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.auditProperty",
      "displayName": "String",
      "oldValue": "String",
      "newValue": "String"
    }
  ],
  "type": "String",
  "resourceId": "String"
}
```



