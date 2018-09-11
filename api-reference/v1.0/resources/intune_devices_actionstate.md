# <a name="actionstate-enum-type"></a><span data-ttu-id="74c0c-101">tipo enumerado actionState</span><span class="sxs-lookup"><span data-stu-id="74c0c-101">actionState enum type</span></span>

> <span data-ttu-id="74c0c-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="74c0c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="74c0c-103">Estado da ação no dispositivo</span><span class="sxs-lookup"><span data-stu-id="74c0c-103">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="74c0c-104">Membros</span><span class="sxs-lookup"><span data-stu-id="74c0c-104">Members</span></span>
|<span data-ttu-id="74c0c-105">Membro</span><span class="sxs-lookup"><span data-stu-id="74c0c-105">Member</span></span>|<span data-ttu-id="74c0c-106">Valor</span><span class="sxs-lookup"><span data-stu-id="74c0c-106">Value</span></span>|<span data-ttu-id="74c0c-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="74c0c-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74c0c-108">none</span><span class="sxs-lookup"><span data-stu-id="74c0c-108">none</span></span>|<span data-ttu-id="74c0c-109">0</span><span class="sxs-lookup"><span data-stu-id="74c0c-109">0%</span></span>|<span data-ttu-id="74c0c-110">Não é um estado de ação válido</span><span class="sxs-lookup"><span data-stu-id="74c0c-110">Not a valid action state</span></span>|
|<span data-ttu-id="74c0c-111">pending</span><span class="sxs-lookup"><span data-stu-id="74c0c-111">pending</span></span>|<span data-ttu-id="74c0c-112">1</span><span class="sxs-lookup"><span data-stu-id="74c0c-112">-1</span></span>|<span data-ttu-id="74c0c-113">Ação está pendente</span><span class="sxs-lookup"><span data-stu-id="74c0c-113">Action is pending</span></span>|
|<span data-ttu-id="74c0c-114">canceled</span><span class="sxs-lookup"><span data-stu-id="74c0c-114">Canceled</span></span>|<span data-ttu-id="74c0c-115">2</span><span class="sxs-lookup"><span data-stu-id="74c0c-115">-2</span></span>|<span data-ttu-id="74c0c-116">Ação foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="74c0c-116">Action has been cancelled.</span></span>|
|<span data-ttu-id="74c0c-117">active</span><span class="sxs-lookup"><span data-stu-id="74c0c-117">Active</span></span>|<span data-ttu-id="74c0c-118">3</span><span class="sxs-lookup"><span data-stu-id="74c0c-118">-3</span></span>|<span data-ttu-id="74c0c-119">Ação está ativa.</span><span class="sxs-lookup"><span data-stu-id="74c0c-119">Action is active.</span></span>|
|<span data-ttu-id="74c0c-120">done</span><span class="sxs-lookup"><span data-stu-id="74c0c-120">done</span></span>|<span data-ttu-id="74c0c-121">4</span><span class="sxs-lookup"><span data-stu-id="74c0c-121">-4</span></span>|<span data-ttu-id="74c0c-122">Ação concluída sem erros.</span><span class="sxs-lookup"><span data-stu-id="74c0c-122">Action completed without errors.</span></span>|
|<span data-ttu-id="74c0c-123">failed</span><span class="sxs-lookup"><span data-stu-id="74c0c-123">Failed</span></span>|<span data-ttu-id="74c0c-124">5</span><span class="sxs-lookup"><span data-stu-id="74c0c-124">$-5</span></span>|<span data-ttu-id="74c0c-125">Falha na ação</span><span class="sxs-lookup"><span data-stu-id="74c0c-125">Action failed</span></span>|
|<span data-ttu-id="74c0c-126">notSupported</span><span class="sxs-lookup"><span data-stu-id="74c0c-126">notSupported</span></span>|<span data-ttu-id="74c0c-127">6</span><span class="sxs-lookup"><span data-stu-id="74c0c-127">-6</span></span>|<span data-ttu-id="74c0c-128">Não há suporte para a ação.</span><span class="sxs-lookup"><span data-stu-id="74c0c-128"> is not supported.</span></span>|








