# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="61124-101">Tipo de recurso windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="61124-101">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="61124-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="61124-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61124-103">Coleção de recursos da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="61124-103">Windows Information Protection Resource Collection</span></span>
## <a name="properties"></a><span data-ttu-id="61124-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="61124-104">Properties</span></span>
|<span data-ttu-id="61124-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61124-105">Property</span></span>|<span data-ttu-id="61124-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="61124-106">Type</span></span>|<span data-ttu-id="61124-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="61124-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61124-108">displayName</span><span class="sxs-lookup"><span data-stu-id="61124-108">displayName</span></span>|<span data-ttu-id="61124-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61124-109">String</span></span>|<span data-ttu-id="61124-110">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="61124-110">Display name</span></span>|
|<span data-ttu-id="61124-111">recursos</span><span class="sxs-lookup"><span data-stu-id="61124-111">resources</span></span>|<span data-ttu-id="61124-112">String collection</span><span class="sxs-lookup"><span data-stu-id="61124-112">String collection</span></span>|<span data-ttu-id="61124-113">Coleção de recursos</span><span class="sxs-lookup"><span data-stu-id="61124-113">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="61124-114">Relações</span><span class="sxs-lookup"><span data-stu-id="61124-114">Relationships</span></span>
<span data-ttu-id="61124-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="61124-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="61124-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="61124-116">JSON Representation</span></span>
<span data-ttu-id="61124-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="61124-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionResourceCollection",
  "displayName": "String",
  "resources": [
    "String"
  ]
}
```



