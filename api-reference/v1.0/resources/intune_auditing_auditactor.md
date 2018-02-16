# <a name="auditactor-resource-type"></a><span data-ttu-id="c434d-101">Tipo de recurso auditActor</span><span class="sxs-lookup"><span data-stu-id="c434d-101">auditActor resource type</span></span>

> <span data-ttu-id="c434d-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c434d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c434d-103">Uma classe que contém as propriedades para Ator de auditoria.</span><span class="sxs-lookup"><span data-stu-id="c434d-103">A class containing the properties for Audit Actor.</span></span>
## <a name="properties"></a><span data-ttu-id="c434d-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c434d-104">Properties</span></span>
|<span data-ttu-id="c434d-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c434d-105">Property</span></span>|<span data-ttu-id="c434d-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="c434d-106">Type</span></span>|<span data-ttu-id="c434d-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="c434d-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c434d-108">type</span><span class="sxs-lookup"><span data-stu-id="c434d-108">type</span></span>|<span data-ttu-id="c434d-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c434d-109">String</span></span>|<span data-ttu-id="c434d-110">Tipo de ator.</span><span class="sxs-lookup"><span data-stu-id="c434d-110">Actor Type.</span></span>|
|<span data-ttu-id="c434d-111">permissões</span><span class="sxs-lookup"><span data-stu-id="c434d-111">permissions</span></span>|<span data-ttu-id="c434d-112">Conjunto de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c434d-112">String collection</span></span>|<span data-ttu-id="c434d-113">Lista de permissões de usuário de quando a auditoria foi executada.</span><span class="sxs-lookup"><span data-stu-id="c434d-113">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="c434d-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="c434d-114">userPermissions</span></span>|<span data-ttu-id="c434d-115">Conjunto de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c434d-115">String collection</span></span>|<span data-ttu-id="c434d-116">Lista de permissões de usuário de quando a auditoria foi executada.</span><span class="sxs-lookup"><span data-stu-id="c434d-116">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="c434d-117">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="c434d-117">applicationId</span></span>|<span data-ttu-id="c434d-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c434d-118">String</span></span>|<span data-ttu-id="c434d-119">ID do aplicativo AAD.</span><span class="sxs-lookup"><span data-stu-id="c434d-119">AAD Application Id.</span></span>|
|<span data-ttu-id="c434d-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="c434d-120">applicationDisplayName</span></span>|<span data-ttu-id="c434d-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c434d-121">String</span></span>|<span data-ttu-id="c434d-122">Nome do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c434d-122">Name of the Application.</span></span>|
|<span data-ttu-id="c434d-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c434d-123">userPrincipalName</span></span>|<span data-ttu-id="c434d-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c434d-124">String</span></span>|<span data-ttu-id="c434d-125">Nome principal do usuário (UPN).</span><span class="sxs-lookup"><span data-stu-id="c434d-125">User principal name (UPN)</span></span>|
|<span data-ttu-id="c434d-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="c434d-126">servicePrincipalName</span></span>|<span data-ttu-id="c434d-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c434d-127">String</span></span>|<span data-ttu-id="c434d-128">Nome da entidade de serviço (SPN).</span><span class="sxs-lookup"><span data-stu-id="c434d-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="c434d-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="c434d-129">ipAddress</span></span>|<span data-ttu-id="c434d-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c434d-130">String</span></span>|<span data-ttu-id="c434d-131">IPAddress.</span><span class="sxs-lookup"><span data-stu-id="c434d-131">IPAddress.</span></span>|
|<span data-ttu-id="c434d-132">userId</span><span class="sxs-lookup"><span data-stu-id="c434d-132">userId</span></span>|<span data-ttu-id="c434d-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c434d-133">String</span></span>|<span data-ttu-id="c434d-134">ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="c434d-134">User ID</span></span>|

## <a name="relationships"></a><span data-ttu-id="c434d-135">Relações</span><span class="sxs-lookup"><span data-stu-id="c434d-135">Relationships</span></span>
<span data-ttu-id="c434d-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c434d-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c434d-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c434d-137">JSON Representation</span></span>
<span data-ttu-id="c434d-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c434d-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.auditActor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditActor",
  "type": "String",
  "permissions": [
    "String"
  ],
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



