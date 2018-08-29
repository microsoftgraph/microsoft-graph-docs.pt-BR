# <a name="rolepermission-resource-type"></a><span data-ttu-id="f4fe4-101">Tipo de recurso rolePermission</span><span class="sxs-lookup"><span data-stu-id="f4fe4-101">rolePermission resource type</span></span>

> <span data-ttu-id="f4fe4-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f4fe4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f4fe4-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f4fe4-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="f4fe4-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f4fe4-104">Properties</span></span>
|<span data-ttu-id="f4fe4-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4fe4-105">Property</span></span>|<span data-ttu-id="f4fe4-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4fe4-106">Type</span></span>|<span data-ttu-id="f4fe4-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4fe4-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4fe4-108">resourceActions</span><span class="sxs-lookup"><span data-stu-id="f4fe4-108">resourceActions</span></span>|<span data-ttu-id="f4fe4-109">Coleção [resourceAction](../resources/intune_rbac_resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="f4fe4-109">[resourceAction](../resources/intune_rbac_resourceaction.md) collection</span></span>|<span data-ttu-id="f4fe4-110">Ações</span><span class="sxs-lookup"><span data-stu-id="f4fe4-110">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4fe4-111">Relações</span><span class="sxs-lookup"><span data-stu-id="f4fe4-111">Relationships</span></span>
<span data-ttu-id="f4fe4-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f4fe4-112">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f4fe4-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f4fe4-113">JSON Representation</span></span>
<span data-ttu-id="f4fe4-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f4fe4-114">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rolePermission"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rolePermission",
  "resourceActions": [
    {
      "@odata.type": "microsoft.graph.resourceAction",
      "allowedResourceActions": [
        "String"
      ],
      "notAllowedResourceActions": [
        "String"
      ]
    }
  ]
}
```



