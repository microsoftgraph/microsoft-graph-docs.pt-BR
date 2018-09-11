# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="74f0c-101">Tipo enumerado defenderThreatAction</span><span class="sxs-lookup"><span data-stu-id="74f0c-101">defenderThreatAction enum type</span></span>

> <span data-ttu-id="74f0c-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="74f0c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="74f0c-103">Ação padrão do Defender para assumir as ameaças de malware detectadas.</span><span class="sxs-lookup"><span data-stu-id="74f0c-103">Defender’s default action to take on detected Malware threats.</span></span>
## <a name="members"></a><span data-ttu-id="74f0c-104">Membros</span><span class="sxs-lookup"><span data-stu-id="74f0c-104">Members</span></span>
|<span data-ttu-id="74f0c-105">Membro</span><span class="sxs-lookup"><span data-stu-id="74f0c-105">Member</span></span>|<span data-ttu-id="74f0c-106">Valor</span><span class="sxs-lookup"><span data-stu-id="74f0c-106">Value</span></span>|<span data-ttu-id="74f0c-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="74f0c-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74f0c-108">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="74f0c-108">deviceDefault</span></span>|<span data-ttu-id="74f0c-109">0</span><span class="sxs-lookup"><span data-stu-id="74f0c-109">0%</span></span>|<span data-ttu-id="74f0c-110">Aplique a ação com base na definição de atualização.</span><span class="sxs-lookup"><span data-stu-id="74f0c-110">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="74f0c-111">clean</span><span class="sxs-lookup"><span data-stu-id="74f0c-111">clean</span></span>|<span data-ttu-id="74f0c-112">1</span><span class="sxs-lookup"><span data-stu-id="74f0c-112">-1</span></span>|<span data-ttu-id="74f0c-113">Apague a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="74f0c-113">Clean the detected threat.</span></span>|
|<span data-ttu-id="74f0c-114">quarantine</span><span class="sxs-lookup"><span data-stu-id="74f0c-114">Quarantine</span></span>|<span data-ttu-id="74f0c-115">2</span><span class="sxs-lookup"><span data-stu-id="74f0c-115">-2</span></span>|<span data-ttu-id="74f0c-116">Coloque a ameaça detectada em quarentena.</span><span class="sxs-lookup"><span data-stu-id="74f0c-116">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="74f0c-117">remover</span><span class="sxs-lookup"><span data-stu-id="74f0c-117">remove</span></span>|<span data-ttu-id="74f0c-118">3</span><span class="sxs-lookup"><span data-stu-id="74f0c-118">-3</span></span>|<span data-ttu-id="74f0c-119">Remova a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="74f0c-119">Remove the detected threat.</span></span>|
|<span data-ttu-id="74f0c-120">allow</span><span class="sxs-lookup"><span data-stu-id="74f0c-120">Allow</span></span>|<span data-ttu-id="74f0c-121">4</span><span class="sxs-lookup"><span data-stu-id="74f0c-121">-4</span></span>|<span data-ttu-id="74f0c-122">Permita a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="74f0c-122">Allow the detected threat.</span></span>|
|<span data-ttu-id="74f0c-123">userDefined</span><span class="sxs-lookup"><span data-stu-id="74f0c-123">User-defined</span></span>|<span data-ttu-id="74f0c-124">5</span><span class="sxs-lookup"><span data-stu-id="74f0c-124">$-5</span></span>|<span data-ttu-id="74f0c-125">Permita que o usuário determine a ação a ser tomada para a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="74f0c-125">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="74f0c-126">bloqueio</span><span class="sxs-lookup"><span data-stu-id="74f0c-126">block</span></span>|<span data-ttu-id="74f0c-127">6</span><span class="sxs-lookup"><span data-stu-id="74f0c-127">-6</span></span>|<span data-ttu-id="74f0c-128">Bloqueie a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="74f0c-128">Block the detected threat.</span></span>|








