# <a name="auditactor-resource-type"></a><span data-ttu-id="de472-101">Tipo de recurso auditActor</span><span class="sxs-lookup"><span data-stu-id="de472-101">auditActor resource type</span></span>

> <span data-ttu-id="de472-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="de472-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="de472-103">Uma classe que contém as propriedades para Ator de auditoria.</span><span class="sxs-lookup"><span data-stu-id="de472-103">A class containing the properties for Audit Actor.</span></span>
## <a name="properties"></a><span data-ttu-id="de472-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="de472-104">Properties</span></span>
|<span data-ttu-id="de472-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de472-105">Property</span></span>|<span data-ttu-id="de472-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="de472-106">Type</span></span>|<span data-ttu-id="de472-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="de472-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de472-108">type</span><span class="sxs-lookup"><span data-stu-id="de472-108">type</span></span>|<span data-ttu-id="de472-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de472-109">String</span></span>|<span data-ttu-id="de472-110">Tipo de ator.</span><span class="sxs-lookup"><span data-stu-id="de472-110">Actor Type.</span></span>|
|<span data-ttu-id="de472-111">userPermissions</span><span class="sxs-lookup"><span data-stu-id="de472-111">userPermissions</span></span>|<span data-ttu-id="de472-112">Conjunto de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de472-112">String collection</span></span>|<span data-ttu-id="de472-113">Lista de permissões de usuário de quando a auditoria foi executada.</span><span class="sxs-lookup"><span data-stu-id="de472-113">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="de472-114">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="de472-114">applicationId</span></span>|<span data-ttu-id="de472-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de472-115">String</span></span>|<span data-ttu-id="de472-116">ID do aplicativo AAD.</span><span class="sxs-lookup"><span data-stu-id="de472-116">AAD Application Id.</span></span>|
|<span data-ttu-id="de472-117">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="de472-117">applicationDisplayName</span></span>|<span data-ttu-id="de472-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de472-118">String</span></span>|<span data-ttu-id="de472-119">Nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="de472-119">Name of the Application.</span></span>|
|<span data-ttu-id="de472-120">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="de472-120">userPrincipalName</span></span>|<span data-ttu-id="de472-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de472-121">String</span></span>|<span data-ttu-id="de472-122">Nome principal do usuário (UPN).</span><span class="sxs-lookup"><span data-stu-id="de472-122">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="de472-123">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="de472-123">servicePrincipalName</span></span>|<span data-ttu-id="de472-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de472-124">String</span></span>|<span data-ttu-id="de472-125">Nome da entidade de serviço (SPN).</span><span class="sxs-lookup"><span data-stu-id="de472-125">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="de472-126">ipAddress</span><span class="sxs-lookup"><span data-stu-id="de472-126">ipAddress</span></span>|<span data-ttu-id="de472-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de472-127">String</span></span>|<span data-ttu-id="de472-128">IPAddress.</span><span class="sxs-lookup"><span data-stu-id="de472-128">IPAddress.</span></span>|
|<span data-ttu-id="de472-129">userId</span><span class="sxs-lookup"><span data-stu-id="de472-129">userId</span></span>|<span data-ttu-id="de472-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de472-130">String</span></span>|<span data-ttu-id="de472-131">ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="de472-131">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de472-132">Relações</span><span class="sxs-lookup"><span data-stu-id="de472-132">Relationships</span></span>
<span data-ttu-id="de472-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="de472-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="de472-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="de472-134">JSON Representation</span></span>
<span data-ttu-id="de472-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="de472-135">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditActor"
}-->
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








