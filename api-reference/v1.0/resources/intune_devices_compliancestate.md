# <a name="compliancestate-enum-type"></a><span data-ttu-id="81770-101">tipo enumerado complianceState</span><span class="sxs-lookup"><span data-stu-id="81770-101">complianceState enum type</span></span>

> <span data-ttu-id="81770-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="81770-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81770-103">Estado de conformidade.</span><span class="sxs-lookup"><span data-stu-id="81770-103">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="81770-104">Membros</span><span class="sxs-lookup"><span data-stu-id="81770-104">Members</span></span>
|<span data-ttu-id="81770-105">Membro</span><span class="sxs-lookup"><span data-stu-id="81770-105">Member</span></span>|<span data-ttu-id="81770-106">Valor</span><span class="sxs-lookup"><span data-stu-id="81770-106">Value</span></span>|<span data-ttu-id="81770-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="81770-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81770-108">unknown</span><span class="sxs-lookup"><span data-stu-id="81770-108">unknown</span></span>|<span data-ttu-id="81770-109">0</span><span class="sxs-lookup"><span data-stu-id="81770-109">0%</span></span>|<span data-ttu-id="81770-110">Desconhecido.</span><span class="sxs-lookup"><span data-stu-id="81770-110">Unknown</span></span>|
|<span data-ttu-id="81770-111">em conformidade</span><span class="sxs-lookup"><span data-stu-id="81770-111">Compliant</span></span>|<span data-ttu-id="81770-112">1</span><span class="sxs-lookup"><span data-stu-id="81770-112">-1</span></span>|<span data-ttu-id="81770-113">Em conformidade.</span><span class="sxs-lookup"><span data-stu-id="81770-113">Compliant</span></span>|
|<span data-ttu-id="81770-114">sem conformidade</span><span class="sxs-lookup"><span data-stu-id="81770-114">noncompliant</span></span>|<span data-ttu-id="81770-115">2</span><span class="sxs-lookup"><span data-stu-id="81770-115">-2</span></span>|<span data-ttu-id="81770-116">Dispositivo não está em conformidade e está bloqueado para recursos corporativos.</span><span class="sxs-lookup"><span data-stu-id="81770-116">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="81770-117">conflito</span><span class="sxs-lookup"><span data-stu-id="81770-117">Conflict</span></span>|<span data-ttu-id="81770-118">3</span><span class="sxs-lookup"><span data-stu-id="81770-118">-3</span></span>|<span data-ttu-id="81770-119">Conflito com outras regras.</span><span class="sxs-lookup"><span data-stu-id="81770-119">Conflict with other rules.</span></span>|
|<span data-ttu-id="81770-120">erro</span><span class="sxs-lookup"><span data-stu-id="81770-120">error</span></span>|<span data-ttu-id="81770-121">4</span><span class="sxs-lookup"><span data-stu-id="81770-121">-4</span></span>|<span data-ttu-id="81770-122">Erro</span><span class="sxs-lookup"><span data-stu-id="81770-122">Error.</span></span>|
|<span data-ttu-id="81770-123">prazo de tolerância</span><span class="sxs-lookup"><span data-stu-id="81770-123">inGracePeriod</span></span>|<span data-ttu-id="81770-124">254</span><span class="sxs-lookup"><span data-stu-id="81770-124">254</span></span>|<span data-ttu-id="81770-125">Dispositivo não está em conformidade, mas ainda tem acesso aos recursos corporativos</span><span class="sxs-lookup"><span data-stu-id="81770-125">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="81770-126">configManager</span><span class="sxs-lookup"><span data-stu-id="81770-126">configManager</span></span>|<span data-ttu-id="81770-127">255</span><span class="sxs-lookup"><span data-stu-id="81770-127">255 characters</span></span>|<span data-ttu-id="81770-128">Gerenciado pelo Gerenciador de configuração</span><span class="sxs-lookup"><span data-stu-id="81770-128">Managed by Config Manager</span></span>|








