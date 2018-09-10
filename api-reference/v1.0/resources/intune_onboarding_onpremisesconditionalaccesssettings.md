# <a name="onpremisesconditionalaccesssettings-resource-type"></a><span data-ttu-id="0e2cf-101">Tipo de recurso onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="0e2cf-101">onPremisesConditionalAccessSettings resource type</span></span>

> <span data-ttu-id="0e2cf-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0e2cf-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0e2cf-103">Entidade singleton que representa as Configurações de acesso condicional do Exchange OnPremises para um locatário.</span><span class="sxs-lookup"><span data-stu-id="0e2cf-103">Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant.</span></span>
## <a name="methods"></a><span data-ttu-id="0e2cf-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="0e2cf-104">Methods</span></span>
|<span data-ttu-id="0e2cf-105">Método</span><span class="sxs-lookup"><span data-stu-id="0e2cf-105">Method</span></span>|<span data-ttu-id="0e2cf-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0e2cf-106">Return Type</span></span>|<span data-ttu-id="0e2cf-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e2cf-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0e2cf-108">Obter onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="0e2cf-108">Get onPremisesConditionalAccessSettings</span></span>](../api/intune_onboarding_onpremisesconditionalaccesssettings_get.md)|[<span data-ttu-id="0e2cf-109">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="0e2cf-109">onPremisesConditionalAccessSettings</span></span>](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)|<span data-ttu-id="0e2cf-110">Ler propriedades e relações de objetos de [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="0e2cf-110">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object.</span></span>|
|[<span data-ttu-id="0e2cf-111">Atualizar onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="0e2cf-111">Update onPremisesConditionalAccessSettings</span></span>](../api/intune_onboarding_onpremisesconditionalaccesssettings_update.md)|[<span data-ttu-id="0e2cf-112">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="0e2cf-112">onPremisesConditionalAccessSettings</span></span>](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)|<span data-ttu-id="0e2cf-113">Atualizar as propriedades de um objeto de [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="0e2cf-113">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0e2cf-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0e2cf-114">Properties</span></span>
|<span data-ttu-id="0e2cf-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0e2cf-115">Property</span></span>|<span data-ttu-id="0e2cf-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e2cf-116">Type</span></span>|<span data-ttu-id="0e2cf-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e2cf-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e2cf-118">id</span><span class="sxs-lookup"><span data-stu-id="0e2cf-118">id</span></span>|<span data-ttu-id="0e2cf-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e2cf-119">String</span></span>|<span data-ttu-id="0e2cf-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0e2cf-120">Not yet documented</span></span>|
|<span data-ttu-id="0e2cf-121">enabled</span><span class="sxs-lookup"><span data-stu-id="0e2cf-121">enabled</span></span>|<span data-ttu-id="0e2cf-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="0e2cf-122">Boolean</span></span>|<span data-ttu-id="0e2cf-123">Indica se o acesso condicional local está habilitado para esta organização</span><span class="sxs-lookup"><span data-stu-id="0e2cf-123">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="0e2cf-124">includedGroups</span><span class="sxs-lookup"><span data-stu-id="0e2cf-124">includedGroups</span></span>|<span data-ttu-id="0e2cf-125">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="0e2cf-125">Guid collection</span></span>|<span data-ttu-id="0e2cf-126">Grupos de usuários que serão direcionados pelo acesso condicional local.</span><span class="sxs-lookup"><span data-stu-id="0e2cf-126">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="0e2cf-127">Todos os usuários nesses grupos deverão ter dispositivos móveis gerenciados e compatíveis com o acesso a email.</span><span class="sxs-lookup"><span data-stu-id="0e2cf-127">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="0e2cf-128">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="0e2cf-128">excludedGroups</span></span>|<span data-ttu-id="0e2cf-129">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="0e2cf-129">Guid collection</span></span>|<span data-ttu-id="0e2cf-130">Grupos de usuários que estarão isentos ao acesso condicional local.</span><span class="sxs-lookup"><span data-stu-id="0e2cf-130">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="0e2cf-131">Todos os usuários desses grupos ficarão isentos da política de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="0e2cf-131">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="0e2cf-132">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="0e2cf-132">overrideDefaultRule</span></span>|<span data-ttu-id="0e2cf-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="0e2cf-133">Boolean</span></span>|<span data-ttu-id="0e2cf-134">Substitui as regras de acesso padrão ao permitir a um dispositivo que seja concedida a garantia de acesso.</span><span class="sxs-lookup"><span data-stu-id="0e2cf-134">Override the default access rule when allowing a device to ensure access is granted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e2cf-135">Relações</span><span class="sxs-lookup"><span data-stu-id="0e2cf-135">Relationships</span></span>
<span data-ttu-id="0e2cf-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0e2cf-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0e2cf-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0e2cf-137">JSON Representation</span></span>
<span data-ttu-id="0e2cf-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0e2cf-138">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onPremisesConditionalAccessSettings"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "String (identifier)",
  "enabled": true,
  "includedGroups": [
    "Guid"
  ],
  "excludedGroups": [
    "Guid"
  ],
  "overrideDefaultRule": true
}
```








