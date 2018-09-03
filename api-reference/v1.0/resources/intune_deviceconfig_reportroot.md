# <a name="reportroot-resource-type"></a><span data-ttu-id="68291-101">Tipo de recurso reportRoot</span><span class="sxs-lookup"><span data-stu-id="68291-101">reportRoot resource type</span></span>

> <span data-ttu-id="68291-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="68291-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="68291-103">O recurso que representa uma instância dos Relatórios de históricos.</span><span class="sxs-lookup"><span data-stu-id="68291-103">The resource that represents an instance of History Reports.</span></span>
## <a name="methods"></a><span data-ttu-id="68291-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="68291-104">Methods</span></span>
|<span data-ttu-id="68291-105">Método</span><span class="sxs-lookup"><span data-stu-id="68291-105">Method</span></span>|<span data-ttu-id="68291-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="68291-106">Return Type</span></span>|<span data-ttu-id="68291-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="68291-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="68291-108">Obter reportRoot</span><span class="sxs-lookup"><span data-stu-id="68291-108">Get reportRoot</span></span>](../api/intune_deviceconfig_reportroot_get.md)|[<span data-ttu-id="68291-109">reportRoot</span><span class="sxs-lookup"><span data-stu-id="68291-109">reportRoot</span></span>](../resources/intune_deviceconfig_reportroot.md)|<span data-ttu-id="68291-110">Ler propriedades e relações de objetos de [reportRoot](../resources/intune_deviceconfig_reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="68291-110">Read properties and relationships of the [reportRoot](../resources/intune_deviceconfig_reportroot.md) object.</span></span>|
|[<span data-ttu-id="68291-111">Atualizar reportRoot</span><span class="sxs-lookup"><span data-stu-id="68291-111">Update reportRoot</span></span>](../api/intune_deviceconfig_reportroot_update.md)|[<span data-ttu-id="68291-112">reportRoot</span><span class="sxs-lookup"><span data-stu-id="68291-112">reportRoot</span></span>](../resources/intune_deviceconfig_reportroot.md)|<span data-ttu-id="68291-113">Atualizar as propriedades de um objeto de [reportRoot](../resources/intune_deviceconfig_reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="68291-113">Update the properties of a [reportRoot](../resources/intune_deviceconfig_reportroot.md) object.</span></span>|
|[<span data-ttu-id="68291-114">Função deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="68291-114">deviceConfigurationUserActivity function</span></span>](../api/intune_deviceconfig_reportroot_deviceconfigurationuseractivity.md)|[<span data-ttu-id="68291-115">relatório</span><span class="sxs-lookup"><span data-stu-id="68291-115">report</span></span>](../resources/intune_deviceconfig_report.md)|<span data-ttu-id="68291-116">Metadados para o Relatório de atividades do usuário de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="68291-116">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="68291-117">função deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="68291-117">deviceConfigurationDeviceActivity function</span></span>](../api/intune_deviceconfig_reportroot_deviceconfigurationdeviceactivity.md)|[<span data-ttu-id="68291-118">relatório</span><span class="sxs-lookup"><span data-stu-id="68291-118">report</span></span>](../resources/intune_deviceconfig_report.md)|<span data-ttu-id="68291-119">Metadados para o relatório de atividade do dispositivo de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="68291-119">Metadata for the device configuration device activity report</span></span>|

## <a name="relationships"></a><span data-ttu-id="68291-120">Relações</span><span class="sxs-lookup"><span data-stu-id="68291-120">Relationships</span></span>
<span data-ttu-id="68291-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="68291-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="68291-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="68291-122">JSON Representation</span></span>
<span data-ttu-id="68291-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="68291-123">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.reportRoot"
}-->
``` json
{
}
```

## <a name="example"></a><span data-ttu-id="68291-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="68291-124">Example</span></span>

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/reports
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.reportRoot"}-->
```json
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```
