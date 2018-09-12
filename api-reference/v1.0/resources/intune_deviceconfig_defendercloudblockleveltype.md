# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="528af-101">tipo enumerado defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="528af-101">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="528af-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="528af-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="528af-103">Valores possíveis de nível de bloqueio na nuvem</span><span class="sxs-lookup"><span data-stu-id="528af-103">Possible values of Cloud Block Level</span></span>
## <a name="members"></a><span data-ttu-id="528af-104">Membros</span><span class="sxs-lookup"><span data-stu-id="528af-104">Members</span></span>
|<span data-ttu-id="528af-105">Membro</span><span class="sxs-lookup"><span data-stu-id="528af-105">Member</span></span>|<span data-ttu-id="528af-106">Valor</span><span class="sxs-lookup"><span data-stu-id="528af-106">Value</span></span>|<span data-ttu-id="528af-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="528af-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="528af-108">notConfigured</span><span class="sxs-lookup"><span data-stu-id="528af-108">notConfigured</span></span>|<span data-ttu-id="528af-109">0</span><span class="sxs-lookup"><span data-stu-id="528af-109">0%</span></span>|<span data-ttu-id="528af-110">Valor padrão, usa o padrão do nível de bloqueio do antivírus do Windows Defender e fornece detecção forte sem aumentar o risco de detecção de arquivos legítimos</span><span class="sxs-lookup"><span data-stu-id="528af-110">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="528af-111">high</span><span class="sxs-lookup"><span data-stu-id="528af-111">High.</span></span>|<span data-ttu-id="528af-112">1</span><span class="sxs-lookup"><span data-stu-id="528af-112">-1</span></span>|<span data-ttu-id="528af-113">Alto aplica um alto nível de detecção.</span><span class="sxs-lookup"><span data-stu-id="528af-113">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="528af-114">highPlus</span><span class="sxs-lookup"><span data-stu-id="528af-114">highPlus</span></span>|<span data-ttu-id="528af-115">2</span><span class="sxs-lookup"><span data-stu-id="528af-115">-2</span></span>|<span data-ttu-id="528af-116">Alto + usa o nível alto e aplica medidas de proteção adicionais</span><span class="sxs-lookup"><span data-stu-id="528af-116">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="528af-117">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="528af-117">zeroTolerance</span></span>|<span data-ttu-id="528af-118">3</span><span class="sxs-lookup"><span data-stu-id="528af-118">-3</span></span>|<span data-ttu-id="528af-119">Tolerância zero bloqueia todos os executáveis desconhecidos</span><span class="sxs-lookup"><span data-stu-id="528af-119">Zero tolerance blocks all unknown executables</span></span>|








