# <a name="auditactor-resource-type"></a><span data-ttu-id="43059-101">Tipo de recurso auditActor</span><span class="sxs-lookup"><span data-stu-id="43059-101">auditActor resource type</span></span>

> <span data-ttu-id="43059-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="43059-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="43059-103">Uma classe que contém as propriedades para Ator de auditoria.</span><span class="sxs-lookup"><span data-stu-id="43059-103">A class containing the properties for Audit Actor.</span></span>
## <a name="properties"></a><span data-ttu-id="43059-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="43059-104">Properties</span></span>
|<span data-ttu-id="43059-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43059-105">Property</span></span>|<span data-ttu-id="43059-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="43059-106">Type</span></span>|<span data-ttu-id="43059-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="43059-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43059-108">type</span><span class="sxs-lookup"><span data-stu-id="43059-108">type</span></span>|<span data-ttu-id="43059-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43059-109">String</span></span>|<span data-ttu-id="43059-110">Tipo de ator.</span><span class="sxs-lookup"><span data-stu-id="43059-110">Actor Type.</span></span>|
|<span data-ttu-id="43059-111">userPermissions</span><span class="sxs-lookup"><span data-stu-id="43059-111">userPermissions</span></span>|<span data-ttu-id="43059-112">Conjunto de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43059-112">String collection</span></span>|<span data-ttu-id="43059-113">Lista de permissões de usuário de quando a auditoria foi executada.</span><span class="sxs-lookup"><span data-stu-id="43059-113">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="43059-114">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="43059-114">applicationId</span></span>|<span data-ttu-id="43059-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43059-115">String</span></span>|<span data-ttu-id="43059-116">ID do aplicativo AAD.</span><span class="sxs-lookup"><span data-stu-id="43059-116">AAD Application Id.</span></span>|
|<span data-ttu-id="43059-117">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="43059-117">applicationDisplayName</span></span>|<span data-ttu-id="43059-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43059-118">String</span></span>|<span data-ttu-id="43059-119">Nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="43059-119">Name of the Application.</span></span>|
|<span data-ttu-id="43059-120">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="43059-120">userPrincipalName</span></span>|<span data-ttu-id="43059-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43059-121">String</span></span>|<span data-ttu-id="43059-122">Nome principal do usuário (UPN).</span><span class="sxs-lookup"><span data-stu-id="43059-122">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="43059-123">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="43059-123">servicePrincipalName</span></span>|<span data-ttu-id="43059-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43059-124">String</span></span>|<span data-ttu-id="43059-125">Nome da entidade de serviço (SPN).</span><span class="sxs-lookup"><span data-stu-id="43059-125">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="43059-126">ipAddress</span><span class="sxs-lookup"><span data-stu-id="43059-126">ipAddress</span></span>|<span data-ttu-id="43059-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43059-127">String</span></span>|<span data-ttu-id="43059-128">IPAddress.</span><span class="sxs-lookup"><span data-stu-id="43059-128">IPAddress.</span></span>|
|<span data-ttu-id="43059-129">userId</span><span class="sxs-lookup"><span data-stu-id="43059-129">userId</span></span>|<span data-ttu-id="43059-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43059-130">String</span></span>|<span data-ttu-id="43059-131">ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="43059-131">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="43059-132">Relações</span><span class="sxs-lookup"><span data-stu-id="43059-132">Relationships</span></span>
<span data-ttu-id="43059-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="43059-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="43059-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="43059-134">JSON Representation</span></span>
<span data-ttu-id="43059-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="43059-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditActor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditActor",
  "type": "String",
  "userPermissions": [
    "String"
  ],
  "applicationId": "String",
  "applicationDisplayName": "String",
  "userPrincipalName": "String",
  "servicePrincipalName": "String",
  "ipAddress": "String",
  "userId": "String"
}
```



